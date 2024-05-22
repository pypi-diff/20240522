# Comparing `tmp/mergify_cli-2024.4.9.11.31.tar.gz` & `tmp/mergify_cli-2024.5.21.17.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergify_cli-2024.4.9.11.31.tar", max compression
+gzip compressed data, was "mergify_cli-2024.5.21.17.47.tar", max compression
```

## Comparing `mergify_cli-2024.4.9.11.31.tar` & `mergify_cli-2024.5.21.17.47.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10143 2024-04-09 11:31:53.528693 mergify_cli-2024.4.9.11.31/LICENSE
--rw-r--r--   0        0        0     1127 2024-04-09 11:31:53.528693 mergify_cli-2024.4.9.11.31/README.md
--rwxr-xr-x   0        0        0    25342 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/hooks/commit-msg
--rw-r--r--   0        0        0        0 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/tests/__init__.py
--rw-r--r--   0        0        0    16292 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/tests/test_mergify_cli.py
--rw-r--r--   0        0        0     2339 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/tests/utils.py
--rw-r--r--   0        0        0     2598 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/pyproject.toml
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 mergify_cli-2024.4.9.11.31/PKG-INFO
+-rw-r--r--   0        0        0    10143 2024-05-21 17:47:39.128776 mergify_cli-2024.5.21.17.47/LICENSE
+-rw-r--r--   0        0        0     1127 2024-05-21 17:47:39.128776 mergify_cli-2024.5.21.17.47/README.md
+-rwxr-xr-x   0        0        0    27224 2024-05-21 17:47:39.128776 mergify_cli-2024.5.21.17.47/mergify_cli/__init__.py
+-rw-r--r--   0        0        0     1797 2024-05-21 17:47:39.128776 mergify_cli-2024.5.21.17.47/mergify_cli/hooks/commit-msg
+-rw-r--r--   0        0        0        0 2024-05-21 17:47:39.128776 mergify_cli-2024.5.21.17.47/mergify_cli/tests/__init__.py
+-rw-r--r--   0        0        0    18368 2024-05-21 17:47:39.128776 mergify_cli-2024.5.21.17.47/mergify_cli/tests/test_mergify_cli.py
+-rw-r--r--   0        0        0     2564 2024-05-21 17:47:39.128776 mergify_cli-2024.5.21.17.47/mergify_cli/tests/utils.py
+-rw-r--r--   0        0        0     2625 2024-05-21 17:47:39.128776 mergify_cli-2024.5.21.17.47/pyproject.toml
+-rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 mergify_cli-2024.5.21.17.47/PKG-INFO
```

### Comparing `mergify_cli-2024.4.9.11.31/LICENSE` & `mergify_cli-2024.5.21.17.47/LICENSE`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.4.9.11.31/README.md` & `mergify_cli-2024.5.21.17.47/README.md`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.4.9.11.31/mergify_cli/__init__.py` & `mergify_cli-2024.5.21.17.47/mergify_cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 import contextlib
 import dataclasses
 import importlib.metadata
 import os
 import pathlib
 import re
 import shutil
-import subprocess
 import sys
 import typing
 from urllib import parse
 
 import aiofiles
 import httpx
 import rich
 import rich.console
 
 
 VERSION = importlib.metadata.version("mergify-cli")
 
 CHANGEID_RE = re.compile(r"Change-Id: (I[0-9a-z]{40})")
+DEPENDS_ON_RE = re.compile(r"Depends-On: (#[0-9]*)")
 READY_FOR_REVIEW_TEMPLATE = 'mutation { markPullRequestReadyForReview(input: { pullRequestId: "%s" }) { clientMutationId } }'
 DRAFT_TEMPLATE = 'mutation { convertPullRequestToDraft(input: { pullRequestId: "%s" }) { clientMutationId } }'
 console = rich.console.Console(log_path=False, log_time=False)
 
 DEBUG = False
 TMP_STACK_BRANCH = "mergify-cli-tmp"
 
@@ -77,30 +77,42 @@
                 style="red",
             )
         sys.exit(1)
 
     response.raise_for_status()
 
 
-async def git(args: str) -> str:
+@dataclasses.dataclass
+class CommandError(Exception):
+    command_args: tuple[str, ...]
+    returncode: int | None
+    stdout: bytes
+
+    def __str__(self) -> str:
+        return f"failed to run `{' '.join(self.command_args)}`: {self.stdout.decode()}"
+
+
+async def _run_command(*args: str) -> str:
     if DEBUG:
-        console.print(f"[purple]DEBUG: running: git {args} [/]")
-    proc = await asyncio.create_subprocess_shell(
-        f"git {args}",
+        console.print(f"[purple]DEBUG: running: git {' '.join(args)} [/]")
+    proc = await asyncio.create_subprocess_exec(
+        *args,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.STDOUT,
     )
     stdout, _ = await proc.communicate()
     if proc.returncode != 0:
-        console.log(f"fail to run `git {args}`:", style="red")
-        console.log(f"{stdout.decode()}", style="red")
-        sys.exit(1)
+        raise CommandError(args, proc.returncode, stdout)
     return stdout.decode().strip()
 
 
+async def git(*args: str) -> str:
+    return await _run_command("git", *args)
+
+
 def get_slug(url: str) -> tuple[str, str]:
     parsed = parse.urlparse(url)
     if not parsed.netloc:
         # Probably ssh
         _, _, path = parsed.path.partition(":")
     else:
         path = parsed.path[1:].rstrip("/")
@@ -108,15 +120,15 @@
     user, repo = path.split("/", 1)
     if repo.endswith(".git"):
         repo = repo[:-4]
     return user, repo
 
 
 async def do_setup() -> None:
-    hooks_dir = pathlib.Path((await git("rev-parse --git-path hooks")).strip())
+    hooks_dir = pathlib.Path(await git("rev-parse", "--git-path", "hooks"))
     installed_hook_file = hooks_dir / "commit-msg"
 
     new_hook_file = str(
         importlib.resources.files(__package__).joinpath("hooks/commit-msg"),
     )
 
     if installed_hook_file.exists():
@@ -145,14 +157,15 @@
     sha: str
 
 
 class PullRequest(typing.TypedDict):
     html_url: str
     number: str
     title: str
+    body: str
     head: HeadRef
     state: str
     draft: bool
     node_id: str
 
 
 class Comment(typing.TypedDict):
@@ -192,16 +205,16 @@
     commits: list[str],
     stack_prefix: str,
     known_changeids: KnownChangeIDs,
     create_as_draft: bool,
 ) -> list[Change]:
     changes = []
     for commit in commits:
-        message = await git(f"log -1 --format='%b' {commit}")
-        title = await git(f"log -1 --format='%s' {commit}")
+        message = await git("log", "-1", "--format='%b'", commit)
+        title = await git("log", "-1", "--format='%s'", commit)
         changeids = CHANGEID_RE.findall(message)
         if not changeids:
             console.print(
                 f"`Change-Id:` line is missing on commit {commit}",
                 style="red",
             )
             console.print(
@@ -235,15 +248,15 @@
         console.log(
             f"* [yellow]\\[{action}][/] '[red]{commit_info}[/] - [b]{title}[/]{draft} {url} - {changeid}",
         )
 
     return changes
 
 
-async def get_changeids_to_delete(
+def get_changeids_to_delete(
     changes: list[Change],
     known_changeids: KnownChangeIDs,
 ) -> set[ChangeId]:
     changeids_to_delete = set(known_changeids.keys()) - {
         changeid for changeid, commit, title, message in changes
     }
     for changeid in changeids_to_delete:
@@ -316,60 +329,75 @@
     remote: str,
     stacked_base_branch: str,
     stacked_dest_branch: str,
     changeid: ChangeId,
     commit: str,
     title: str,
     message: str,
+    depends_on: PullRequest | None,
     known_changeids: KnownChangeIDs,
     create_as_draft: bool,
     keep_pull_request_title_and_body: bool,
 ) -> tuple[PullRequest, str]:
     if changeid in known_changeids:
         pull = known_changeids.get(changeid)
         status_message = f"* updating stacked branch `{stacked_dest_branch}` ({commit[-7:]}) - {pull['html_url'] if pull else '<stack branch without associated pull>'})"
     else:
         status_message = (
             f"* creating stacked branch `{stacked_dest_branch}` ({commit[-7:]})"
         )
 
     with console.status(status_message):
-        await git(f"branch {TMP_STACK_BRANCH} {commit}")
+        await git("branch", TMP_STACK_BRANCH, commit)
         try:
-            await git(f"push -f {remote} {TMP_STACK_BRANCH}:{stacked_dest_branch}")
+            await git(
+                "push",
+                "-f",
+                remote,
+                TMP_STACK_BRANCH + ":" + stacked_dest_branch,
+            )
         finally:
-            await git(f"branch -D {TMP_STACK_BRANCH}")
+            await git("branch", "-D", TMP_STACK_BRANCH)
 
     pull = known_changeids.get(changeid)
     if pull and pull["head"]["sha"] == commit:
         action = "nothing"
     elif pull:
         action = "updated"
         with console.status(
             f"* updating pull request `{title}` (#{pull['number']}) ({commit[-7:]})",
         ):
             pull_changes = {
                 "head": stacked_dest_branch,
                 "base": stacked_base_branch,
             }
-            if not keep_pull_request_title_and_body:
-                pull_changes.update({"title": title, "body": message})
+            if keep_pull_request_title_and_body:
+                pull_changes.update(
+                    {"body": format_pull_description(pull["body"], depends_on)},
+                )
+            else:
+                pull_changes.update(
+                    {
+                        "title": title,
+                        "body": format_pull_description(message, depends_on),
+                    },
+                )
 
             r = await client.patch(f"pulls/{pull['number']}", json=pull_changes)
             check_for_status(r)
     else:
         action = "created"
         with console.status(
             f"* creating stacked pull request `{title}` ({commit[-7:]})",
         ):
             r = await client.post(
                 "pulls",
                 json={
                     "title": title,
-                    "body": message,
+                    "body": format_pull_description(message, depends_on),
                     "draft": create_as_draft,
                     "head": stacked_dest_branch,
                     "base": stacked_base_branch,
                 },
             )
             check_for_status(r)
             pull = typing.cast(PullRequest, r.json())
@@ -420,63 +448,72 @@
         )
     else:
         console.log(
             f"* [red]\\[deleted][/] '[red].......[/] - [b]<branch {stack_prefix}/{changeid}>[/] - {changeid}",
         )
 
 
-async def log_httpx_request(request: httpx.Request) -> None:
+def log_httpx_request(request: httpx.Request) -> None:
     console.print(
         f"[purple]DEBUG: request: {request.method} {request.url} - Waiting for response[/]",
     )
 
 
-async def log_httpx_response(response: httpx.Response) -> None:
+def log_httpx_response(response: httpx.Response) -> None:
     request = response.request
     console.print(
         f"[purple]DEBUG: response: {request.method} {request.url} - Status {response.status_code}[/]",
     )
 
 
-def get_trunk() -> str:
-    try:
-        trunk = subprocess.check_output(
-            "git config --get mergify-cli.stack-trunk",
-            shell=True,
-            text=True,
-        ).strip()
-    except subprocess.CalledProcessError:
-        trunk = ""
+async def git_get_branch_name() -> str:
+    return await git("rev-parse", "--abbrev-ref", "HEAD")
 
-    if not trunk:
-        try:
-            dest_branch = subprocess.check_output(
-                "git rev-parse --abbrev-ref HEAD",
-                shell=True,
-                text=True,
-            ).strip()
-        except subprocess.CalledProcessError:
-            return ""
 
-        try:
-            trunk = subprocess.check_output(
-                f"git for-each-ref --format='%(upstream:short)' refs/heads/{dest_branch}",
-                shell=True,
-                text=True,
-            ).strip()
-        except subprocess.CalledProcessError:
-            trunk = ""
+async def git_get_target_branch(branch: str) -> str:
+    return (await git("config", "--get", "branch." + branch + ".merge")).removeprefix(
+        "refs/heads/",
+    )
+
 
-    return trunk
+async def git_get_remote_for_branch(branch: str) -> str:
+    return await git("config", "--get", "branch." + branch + ".remote")
+
+
+async def get_trunk() -> str:
+    try:
+        branch_name = await git_get_branch_name()
+    except CommandError:
+        console.print("error: can't get the current branch", style="red")
+        raise
+    try:
+        target_branch = await git_get_target_branch(branch_name)
+    except CommandError:
+        # It's possible this has not been set; ignore
+        console.print("error: can't get the remote target branch", style="red")
+        console.print(
+            f"Please set the target branch with `git branch {branch_name} --set-upstream-to=<remote>/<branch>",
+            style="red",
+        )
+        raise
+    try:
+        remote = await git_get_remote_for_branch(target_branch)
+    except CommandError:
+        console.print(
+            f"error: can't get the remote for branch {target_branch}",
+            style="red",
+        )
+        raise
+    return f"{remote}/{target_branch}"
 
 
 def trunk_type(trunk: str) -> tuple[str, str]:
     result = trunk.split("/", maxsplit=1)
     if len(result) != 2:
-        msg = "stack-trunk is invalid. It must be origin/branch-name [/]"
+        msg = "Trunk is invalid. It must be origin/branch-name [/]"
         raise argparse.ArgumentTypeError(msg)
     return result[0], result[1]
 
 
 @dataclasses.dataclass
 class LocalBranchInvalidError(Exception):
     message: str
@@ -487,74 +524,76 @@
         r"I[0-9a-z]{40}$",
         branch_name,
     ):
         msg = "Local branch is a branch generated by Mergify CLI"
         raise LocalBranchInvalidError(msg)
 
 
-# TODO(charly): fix PLR0913,PLR0914,PLR0915,PLR0917 (number of arguments, local
-# variables and statements)
-async def stack(  # noqa: PLR0913,PLR0914,PLR0915,PLR0917
+# TODO(charly): fix code to conform to linter (number of arguments, local
+# variables, statements, positional arguments, branches)
+async def stack(  # noqa: PLR0913, PLR0914, PLR0915, PLR0917, PLR0912
     token: str,
     skip_rebase: bool,
     next_only: bool,
     branch_prefix: str,
     dry_run: bool,
     trunk: tuple[str, str],
     create_as_draft: bool = False,
     keep_pull_request_title_and_body: bool = False,
 ) -> None:
-    os.chdir((await git("rev-parse --show-toplevel")).strip())
-    dest_branch = await git("rev-parse --abbrev-ref HEAD")
+    os.chdir(await git("rev-parse", "--show-toplevel"))
+    dest_branch = await git("rev-parse", "--abbrev-ref", "HEAD")
 
     try:
         check_local_branch(branch_name=dest_branch, branch_prefix=branch_prefix)
     except LocalBranchInvalidError as e:
         console.log(f"[red] {e.message} [/]")
         console.log(
             "You should run `mergify stack` on the branch you created in the first place",
         )
         sys.exit(1)
 
     remote, base_branch = trunk
 
-    user, repo = get_slug(await git(f"config --get remote.{remote}.url"))
+    user, repo = get_slug(await git("config", "--get", f"remote.{remote}.url"))
 
     if base_branch == dest_branch:
         console.log("[red] base branch and destination branch are the same [/]")
         sys.exit(1)
 
     stack_prefix = f"{branch_prefix}/{dest_branch}"
 
     if not dry_run:
         if skip_rebase:
             console.log(f"branch `{dest_branch}` rebase skipped (--skip-rebase)")
         else:
             with console.status(
                 f"Rebasing branch `{dest_branch}` on `{remote}/{base_branch}`...",
             ):
-                await git(f"pull --rebase {remote} {base_branch}")
+                await git("pull", "--rebase", remote, base_branch)
             console.log(f"branch `{dest_branch}` rebased on `{remote}/{base_branch}`")
 
-    base_commit_sha = await git(f"merge-base --fork-point {remote}/{base_branch}")
+    base_commit_sha = await git("merge-base", "--fork-point", f"{remote}/{base_branch}")
     if not base_commit_sha:
         console.log(
             f"Common commit between `{remote}/{base_branch}` and `{dest_branch}` branches not found",
             style="red",
         )
         sys.exit(1)
 
     commits = [
         commit
         for commit in reversed(
-            (await git(f"log --format='%H' {base_commit_sha}..{dest_branch}")).split(
+            (
+                await git("log", "--format='%H'", f"{base_commit_sha}..{dest_branch}")
+            ).split(
                 "\n",
             ),
         )
-        if commit.strip()
+        if commit
     ]
 
     known_changeids = KnownChangeIDs({})
 
     if DEBUG:
         event_hooks = {"request": [log_httpx_request], "response": [log_httpx_response]}
     else:
@@ -592,15 +631,15 @@
             console.log("Stacked pull request plan:", style="green")
             changes = await get_local_changes(
                 commits,
                 stack_prefix,
                 known_changeids,
                 create_as_draft,
             )
-            changeids_to_delete = await get_changeids_to_delete(
+            changeids_to_delete = get_changeids_to_delete(
                 changes,
                 known_changeids,
             )
 
         if dry_run:
             console.log("[orange]Finished (dry-run mode) :tada:[/]")
             sys.exit(0)
@@ -617,25 +656,27 @@
                     client,
                     remote,
                     stacked_base_branch,
                     stacked_dest_branch,
                     changeid,
                     commit,
                     title,
-                    format_pull_description(message, depends_on),
+                    message,
+                    depends_on,
                     known_changeids,
                     create_as_draft,
                     keep_pull_request_title_and_body,
                 )
                 pulls.append(pull)
             else:
                 action = "skipped"
                 pull = known_changeids.get(changeid) or PullRequest(
                     {
                         "title": "<not yet created>",
+                        "body": "<not yet created>",
                         "html_url": "<no-yet-created>",
                         "number": "-1",
                         "node_id": "na",
                         "draft": True,
                         "state": "",
                         "head": {"sha": ""},
                     },
@@ -670,44 +711,49 @@
 
 def format_pull_description(message: str, depends_on: PullRequest | None) -> str:
     depends_on_header = ""
     if depends_on is not None:
         depends_on_header = f"\n\nDepends-On: #{depends_on['number']}"
 
     message = CHANGEID_RE.sub("", message).rstrip("\n")
+    message = DEPENDS_ON_RE.sub("", message).rstrip("\n")
 
     return message + depends_on_header
 
 
 def GitHubToken(v: str) -> str:  # noqa: N802
     if not v:
         raise ValueError
     return v
 
 
-def get_default_branch_prefix() -> str:
+async def get_default_branch_prefix() -> str:
     try:
-        result = subprocess.check_output(
-            "git config --get mergify-cli.stack-branch-prefix",
-            shell=True,
-        )
-    except subprocess.CalledProcessError:
-        result = b""
+        result = await git("config", "--get", "mergify-cli.stack-branch-prefix")
+    except CommandError:
+        result = ""
 
-    return result.decode().strip() or "mergify_cli"
+    return result or "mergify_cli"
 
 
-def get_default_token() -> str:
+async def get_default_keep_pr_title_body() -> bool:
+    try:
+        result = await git("config", "--get", "mergify-cli.stack-keep-pr-title-body")
+    except CommandError:
+        return False
+
+    return result == "true"
+
+
+async def get_default_token() -> str:
     token = os.environ.get("GITHUB_TOKEN", "")
     if not token:
         try:
-            token = (
-                subprocess.check_output("gh auth token", shell=True).decode().strip()
-            )
-        except subprocess.CalledProcessError:
+            token = await _run_command("gh", "auth", "token")
+        except CommandError:
             console.print(
                 "error: please make sure that gh client is installed and you are authenticated, or set the "
                 "'GITHUB_TOKEN' environment variable",
             )
     if DEBUG:
         console.print(f"[purple]DEBUG: token: {token}[/]")
     return token
@@ -726,34 +772,38 @@
         args.dry_run,
         args.trunk,
         args.draft,
         args.keep_pull_request_title_and_body,
     )
 
 
-def parse_args(args: typing.MutableSequence[str]) -> argparse.Namespace:
+async def parse_args(args: typing.MutableSequence[str]) -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--version",
         "-V",
         action="version",
         version=f"%(prog)s {VERSION}",
         help="display version",
     )
     parser.add_argument("--debug", action="store_true", help="debug mode")
     parser.add_argument(
         "--token",
-        default=get_default_token(),
+        default=await get_default_token(),
         type=GitHubToken,
         help="GitHub personal access token",
     )
     parser.add_argument("--dry-run", "-n", action="store_true")
     sub_parsers = parser.add_subparsers(dest="action")
 
-    stack_parser = sub_parsers.add_parser("stack", help="create a pull requests stack")
+    stack_parser = sub_parsers.add_parser(
+        "stack",
+        description="Stacked Pull Requests CLI",
+        help="Create a pull requests stack",
+    )
     stack_parser.set_defaults(func=stack_main)
     stack_parser.add_argument(
         "--setup",
         action="store_true",
         help="Initial installation of the required git commit-msg hook",
     )
     stack_parser.add_argument(
@@ -780,37 +830,44 @@
         action="store_true",
         help="Create stacked pull request as draft",
     )
     stack_parser.add_argument(
         "--keep-pull-request-title-and-body",
         "-k",
         action="store_true",
-        help="Don't update the title and body of already opened pull requests",
+        default=await get_default_keep_pr_title_body(),
+        help="Don't update the title and body of already opened pull requests. "
+        "Default fetched from git config if added with `git config --add mergify-cli.stack-keep-pr-title-body true`",
     )
     stack_parser.add_argument(
         "--trunk",
         "-t",
         type=trunk_type,
-        default=get_trunk(),
-        help="Change the target branch of the stack",
+        default=await get_trunk(),
+        help="Change the target branch of the stack.",
     )
     stack_parser.add_argument(
         "--branch-prefix",
-        default=get_default_branch_prefix(),
-        help="branch prefix used to create stacked PR",
+        default=await get_default_branch_prefix(),
+        help="Branch prefix used to create stacked PR. "
+        "Default fetched from git config if added with `git config --add mergify-cli.stack-branch-prefix some-prefix`",
     )
 
     known_args, _ = parser.parse_known_args(args)
     if known_args.action is None:
         args.insert(1, "stack")
 
     return parser.parse_args(args)
 
 
-def cli() -> None:
-    args = parse_args(sys.argv[1:])
+async def main() -> None:
+    args = await parse_args(sys.argv[1:])
 
     if args.debug:
         global DEBUG  # noqa: PLW0603
         DEBUG = True
 
-    asyncio.run(args.func(args))
+    await args.func(args)
+
+
+def cli() -> None:
+    asyncio.run(main())
```

### Comparing `mergify_cli-2024.4.9.11.31/mergify_cli/hooks/commit-msg` & `mergify_cli-2024.5.21.17.47/mergify_cli/hooks/commit-msg`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.4.9.11.31/mergify_cli/tests/test_mergify_cli.py` & `mergify_cli-2024.5.21.17.47/mergify_cli/tests/test_mergify_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
-
+import collections
 import json
 import pathlib
+import subprocess
 import typing
 from unittest import mock
 
 import pytest
 import respx
 
 import mergify_cli
@@ -32,45 +33,84 @@
 ) -> None:
     # Change working directory to avoid doing git commands in the current
     # repository
     monkeypatch.chdir(tmp_path)
 
 
 @pytest.fixture()
+def _git_repo() -> None:
+    subprocess.call(["git", "init", "--initial-branch=main"])
+    subprocess.call(["git", "config", "user.email", "test@example.com"])
+    subprocess.call(["git", "config", "user.name", "Test User"])
+    subprocess.call(["git", "commit", "--allow-empty", "-m", "Initial commit"])
+    subprocess.call(["git", "config", "--add", "branch.main.merge", "refs/heads/main"])
+    subprocess.call(["git", "config", "--add", "branch.main.remote", "origin"])
+
+
+@pytest.fixture()
 def git_mock(
     tmp_path: pathlib.Path,
 ) -> typing.Generator[test_utils.GitMock, None, None]:
     git_mock_object = test_utils.GitMock()
     # Top level directory is a temporary path
-    git_mock_object.mock("rev-parse --show-toplevel", str(tmp_path))
+    git_mock_object.mock("rev-parse", "--show-toplevel", output=str(tmp_path))
     # Name of the current branch
-    git_mock_object.mock("rev-parse --abbrev-ref HEAD", "current-branch")
+    git_mock_object.mock("rev-parse", "--abbrev-ref", "HEAD", output="current-branch")
     # URL of the GitHub repository
     git_mock_object.mock(
-        "config --get remote.origin.url",
-        "https://github.com/user/repo",
+        "config",
+        "--get",
+        "remote.origin.url",
+        output="https://github.com/user/repo",
     )
     # Mock pull and push commands
-    git_mock_object.mock("pull --rebase origin main", "")
-    git_mock_object.mock("push -f origin current-branch:/current-branch/aio", "")
+    git_mock_object.mock("pull", "--rebase", "origin", "main", output="")
+    git_mock_object.mock(
+        "push",
+        "-f",
+        "origin",
+        "current-branch:/current-branch/aio",
+        output="",
+    )
 
     with mock.patch("mergify_cli.git", git_mock_object):
         yield git_mock_object
 
 
-def test_cli_help(capsys: pytest.CaptureFixture[str]) -> None:
+@pytest.mark.usefixtures("_git_repo")
+async def test_cli_help(capsys: pytest.CaptureFixture[str]) -> None:
     with pytest.raises(SystemExit, match="0"):
-        mergify_cli.parse_args(["--help"])
+        await mergify_cli.parse_args(["--help"])
 
     stdout = capsys.readouterr().out
     assert "usage: " in stdout
     assert "positional arguments:" in stdout
     assert "options:" in stdout
 
 
+@pytest.mark.usefixtures("_git_repo")
+async def test_get_branch_name() -> None:
+    assert await mergify_cli.git_get_branch_name() == "main"
+
+
+@pytest.mark.usefixtures("_git_repo")
+async def test_get_target_branch() -> None:
+    assert await mergify_cli.git_get_target_branch("main") == "main"
+
+
+@pytest.mark.usefixtures("_git_repo")
+async def test_get_remote_for_branch() -> None:
+    assert await mergify_cli.git_get_remote_for_branch("main") == "origin"
+
+
+@pytest.mark.usefixtures("_git_repo")
+async def test_get_trunk() -> None:
+    assert await mergify_cli.get_trunk() == "origin/main"
+
+
 @pytest.mark.parametrize(
     "valid_branch_name",
     [
         ("my-branch"),
         ("prefix/my-branch"),
         ("my-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50"),
     ],
@@ -328,15 +368,15 @@
         token="",
         skip_rebase=True,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
     )
-    assert not git_mock.has_been_called_with("pull --rebase origin main")
+    assert not git_mock.has_been_called_with("pull", "--rebase", "origin", "main")
 
     # The pull request is updated
     assert len(patch_pull_mock.calls) == 1
     assert json.loads(patch_pull_mock.calls.last.request.content) == {
         "head": "/current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
         "base": "main",
         "title": "Title",
@@ -404,15 +444,15 @@
         token="",
         skip_rebase=False,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
     )
-    assert git_mock.has_been_called_with("pull --rebase origin main")
+    assert git_mock.has_been_called_with("pull", "--rebase", "origin", "main")
 
     # The pull request is updated
     assert len(patch_pull_mock.calls) == 1
     assert json.loads(patch_pull_mock.calls.last.request.content) == {
         "head": "/current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
         "base": "main",
         "title": "Title",
@@ -454,14 +494,15 @@
                 "html_url": "",
                 "number": "123",
                 "title": "Title",
                 "head": {"sha": "previous_commit_sha"},
                 "state": "open",
                 "draft": False,
                 "node_id": "",
+                "body": "DONT TOUCH ME\n\nDepends-On: #12345\n",
             },
         ],
     )
     patch_pull_mock = respx_mock.patch("/repos/user/repo/pulls/123").respond(
         200,
         json={},
     )
@@ -487,22 +528,23 @@
     )
 
     # The pull request is updated
     assert len(patch_pull_mock.calls) == 1
     assert json.loads(patch_pull_mock.calls.last.request.content) == {
         "head": "/current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
         "base": "main",
+        "body": "DONT TOUCH ME",
     }
 
 
 @pytest.mark.respx(base_url="https://api.github.com/")
 async def test_stack_on_destination_branch_raises_an_error(
     git_mock: test_utils.GitMock,
 ) -> None:
-    git_mock.mock("rev-parse --abbrev-ref HEAD", "main")
+    git_mock.mock("rev-parse", "--abbrev-ref", "HEAD", output="main")
 
     with pytest.raises(SystemExit, match="1"):
         await mergify_cli.stack(
             token="",
             skip_rebase=False,
             next_only=False,
             branch_prefix="",
@@ -511,18 +553,37 @@
         )
 
 
 @pytest.mark.respx(base_url="https://api.github.com/")
 async def test_stack_without_common_commit_raises_an_error(
     git_mock: test_utils.GitMock,
 ) -> None:
-    git_mock.mock("merge-base --fork-point origin/main", "")
+    git_mock.mock("merge-base", "--fork-point", "origin/main", output="")
 
     with pytest.raises(SystemExit, match="1"):
         await mergify_cli.stack(
             token="",
             skip_rebase=False,
             next_only=False,
             branch_prefix="",
             dry_run=False,
             trunk=("origin", "main"),
         )
+
+
+@pytest.mark.parametrize(
+    ("default_arg_fct", "config_get_result", "expected_default"),
+    [
+        (mergify_cli.get_default_keep_pr_title_body, "true", True),
+        (mergify_cli.get_default_branch_prefix, "dummy-prefix", "dummy-prefix"),
+    ],
+)
+async def test_defaults_config_args_set(
+    default_arg_fct: collections.abc.Callable[
+        [],
+        collections.abc.Awaitable[bool | str],
+    ],
+    config_get_result: bytes,
+    expected_default: bool,
+) -> None:
+    with mock.patch.object(mergify_cli, "_run_command", return_value=config_get_result):
+        assert (await default_arg_fct()) == expected_default
```

### Comparing `mergify_cli-2024.4.9.11.31/mergify_cli/tests/utils.py` & `mergify_cli-2024.5.21.17.47/mergify_cli/tests/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,48 +21,59 @@
     title: str
     message: str
     change_id: str
 
 
 @dataclasses.dataclass
 class GitMock:
-    _mocked: dict[str, str] = dataclasses.field(init=False, default_factory=dict)
+    _mocked: dict[tuple[str, ...], str] = dataclasses.field(
+        init=False,
+        default_factory=dict,
+    )
     _commits: list[Commit] = dataclasses.field(init=False, default_factory=list)
-    _called: list[str] = dataclasses.field(init=False, default_factory=list)
+    _called: list[tuple[str, ...]] = dataclasses.field(init=False, default_factory=list)
 
-    def mock(self, command: str, output: str) -> None:
-        self._mocked[command] = output
+    def mock(self, *args: str, output: str) -> None:
+        self._mocked[args] = output
 
-    def has_been_called_with(self, args: str) -> bool:
+    def has_been_called_with(self, *args: str) -> bool:
         return args in self._called
 
-    async def __call__(self, args: str) -> str:
+    async def __call__(self, *args: str) -> str:
         if args in self._mocked:
             self._called.append(args)
             return self._mocked[args]
 
         msg = f"git_mock called with `{args}`, not mocked!"
         raise AssertionError(msg)
 
     def commit(self, commit: Commit) -> None:
         self._commits.append(commit)
 
         # Base commit SHA
-        self.mock("merge-base --fork-point origin/main", "base_commit_sha")
+        self.mock("merge-base", "--fork-point", "origin/main", output="base_commit_sha")
         # Commit message
         self.mock(
-            f"log -1 --format='%b' {commit['sha']}",
-            f"{commit['message']}\n\nChange-Id: {commit['change_id']}",
+            "log",
+            "-1",
+            "--format='%b'",
+            commit["sha"],
+            output=f"{commit['message']}\n\nChange-Id: {commit['change_id']}",
         )
         # Commit title
-        self.mock(f"log -1 --format='%s' {commit['sha']}", commit["title"])
+        self.mock("log", "-1", "--format='%s'", commit["sha"], output=commit["title"])
         # List of commit SHAs
         self.mock(
-            "log --format='%H' base_commit_sha..current-branch",
-            "\n".join(c["sha"] for c in reversed(self._commits)),
+            "log",
+            "--format='%H'",
+            "base_commit_sha..current-branch",
+            output="\n".join(c["sha"] for c in reversed(self._commits)),
         )
-        self.mock(f"branch mergify-cli-tmp {commit['sha']}", "")
-        self.mock("branch -D mergify-cli-tmp", "")
+        self.mock("branch", "mergify-cli-tmp", commit["sha"], output="")
+        self.mock("branch", "-D", "mergify-cli-tmp", output="")
         self.mock(
-            f"push -f origin mergify-cli-tmp:/current-branch/{commit['change_id']}",
-            "",
+            "push",
+            "-f",
+            "origin",
+            f"mergify-cli-tmp:/current-branch/{commit['change_id']}",
+            output="",
         )
```

### Comparing `mergify_cli-2024.4.9.11.31/pyproject.toml` & `mergify_cli-2024.5.21.17.47/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.group.dev.dependencies]
 mypy = {version = ">=0.930"}
 mypy-extensions = "^1.0.0"
-ruff = ">=0.0.277,<0.3.6"
+ruff = ">=0.0.277,<0.4.5"
 pytest = {version = ">=6.2.5"}
-poethepoet = ">=0.21,<0.26"
+poethepoet = ">=0.21,<0.27"
 pytest-asyncio = "^0.23.2"
 respx = ">=0.20.2,<0.22.0"
 types-aiofiles = "^23.2.0.20240106"
 
 [tool.poetry.scripts]
 mergify = 'mergify_cli:cli'
 
@@ -102,16 +102,16 @@
 ]
 
 ignore = [
     # NOTE(charly): line-length is up to the formatter
     "E501",
     # NOTE(charly): `subprocess` module is possibly insecure
     "S404",
-    # NOTE(charly): `subprocess` call with `shell=True`
-    "S602",
+    # NOTE(jd): likely a false positive https://github.com/PyCQA/bandit/issues/333
+    "S603",
     # NOTE(charly): Starting a process with a partial executable path
     "S607",
     # NOTE(charly): Boolean-typed positional argument in function definition.
     # Interesting, but require some work.
     "FBT001",
     # NOTE(charly): Boolean default positional argument in function definition.
     # Interesting, but require some work.
```

### Comparing `mergify_cli-2024.4.9.11.31/PKG-INFO` & `mergify_cli-2024.5.21.17.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergify_cli
-Version: 2024.4.9.11.31
+Version: 2024.5.21.17.47
 Summary: Mergify CLI is a tool that automates the creation and management of stacked pull requests on GitHub
 License: Apache License
 Author: Mehdi Abaakouk
 Author-email: sileht@mergify.com
 Requires-Python: >=3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

