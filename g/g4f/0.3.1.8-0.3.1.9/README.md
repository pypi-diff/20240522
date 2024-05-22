# Comparing `tmp/g4f-0.3.1.8.tar.gz` & `tmp/g4f-0.3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.1.8.tar", last modified: Sun May 19 23:51:12 2024, max compression
+gzip compressed data, was "g4f-0.3.1.9.tar", last modified: Wed May 22 18:21:14 2024, max compression
```

## Comparing `g4f-0.3.1.8.tar` & `g4f-0.3.1.9.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.487223 g4f-0.3.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-19 23:51:09.000000 g4f-0.3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-19 23:51:09.000000 g4f-0.3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55979 2024-05-19 23:51:12.487223 g4f-0.3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    52783 2024-05-19 23:51:09.000000 g4f-0.3.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.447223 g4f-0.3.1.8/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.455223 g4f-0.3.1.8/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Reka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.459223 g4f-0.3.1.8/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.463223 g4f-0.3.1.8/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.463223 g4f-0.3.1.8/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.467223 g4f-0.3.1.8/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    33277 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/PerplexityApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.467223 g4f-0.3.1.8/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.471223 g4f-0.3.1.8/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.471223 g4f-0.3.1.8/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.471223 g4f-0.3.1.8/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.471223 g4f-0.3.1.8/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/openai/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/openai/proofofwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.471223 g4f-0.3.1.8/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.471223 g4f-0.3.1.8/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.471223 g4f-0.3.1.8/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.475223 g4f-0.3.1.8/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.475223 g4f-0.3.1.8/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.475223 g4f-0.3.1.8/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.475223 g4f-0.3.1.8/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    13418 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.443223 g4f-0.3.1.8/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.475223 g4f-0.3.1.8/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/css/dracula.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    21629 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.479223 g4f-0.3.1.8/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.479223 g4f-0.3.1.8/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    51445 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.479223 g4f-0.3.1.8/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.483223 g4f-0.3.1.8/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.483223 g4f-0.3.1.8/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.483223 g4f-0.3.1.8/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.483223 g4f-0.3.1.8/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.483223 g4f-0.3.1.8/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-19 23:51:09.000000 g4f-0.3.1.8/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:51:12.483223 g4f-0.3.1.8/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55979 2024-05-19 23:51:12.000000 g4f-0.3.1.8/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-19 23:51:12.000000 g4f-0.3.1.8/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 23:51:12.000000 g4f-0.3.1.8/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 23:51:12.000000 g4f-0.3.1.8/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-19 23:51:12.000000 g4f-0.3.1.8/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 23:51:12.000000 g4f-0.3.1.8/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 23:51:12.487223 g4f-0.3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-19 23:51:09.000000 g4f-0.3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.300294 g4f-0.3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-22 18:21:08.000000 g4f-0.3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 18:21:08.000000 g4f-0.3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55653 2024-05-22 18:21:14.300294 g4f-0.3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    52457 2024-05-22 18:21:08.000000 g4f-0.3.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.256293 g4f-0.3.1.9/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.268293 g4f-0.3.1.9/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.268293 g4f-0.3.1.9/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.276293 g4f-0.3.1.9/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.276293 g4f-0.3.1.9/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.276293 g4f-0.3.1.9/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33277 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/PerplexityApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.280293 g4f-0.3.1.9/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.280293 g4f-0.3.1.9/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.280293 g4f-0.3.1.9/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.280293 g4f-0.3.1.9/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.280293 g4f-0.3.1.9/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.280293 g4f-0.3.1.9/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.284293 g4f-0.3.1.9/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.284293 g4f-0.3.1.9/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.284293 g4f-0.3.1.9/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.284293 g4f-0.3.1.9/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.284293 g4f-0.3.1.9/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.288293 g4f-0.3.1.9/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    13418 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.252293 g4f-0.3.1.9/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.288293 g4f-0.3.1.9/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/css/dracula.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.288293 g4f-0.3.1.9/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.288293 g4f-0.3.1.9/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    51445 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.292293 g4f-0.3.1.9/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.292293 g4f-0.3.1.9/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.292293 g4f-0.3.1.9/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.292293 g4f-0.3.1.9/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.292293 g4f-0.3.1.9/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.296293 g4f-0.3.1.9/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-22 18:21:08.000000 g4f-0.3.1.9/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:14.296293 g4f-0.3.1.9/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55653 2024-05-22 18:21:14.000000 g4f-0.3.1.9/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-22 18:21:14.000000 g4f-0.3.1.9/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:21:14.000000 g4f-0.3.1.9/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 18:21:14.000000 g4f-0.3.1.9/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 18:21:14.000000 g4f-0.3.1.9/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 18:21:14.000000 g4f-0.3.1.9/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:21:14.300294 g4f-0.3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-22 18:21:08.000000 g4f-0.3.1.9/setup.py
```

### Comparing `g4f-0.3.1.8/LICENSE` & `g4f-0.3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/PKG-INFO` & `g4f-0.3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.8
+Version: 0.3.1.9
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -515,27 +515,14 @@
 | Gemini API | `g4f.Provider.GeminiPro` | ❌ | gemini-1.5-pro | [ai.google.dev](https://ai.google.dev) |
 | Meta AI | `g4f.Provider.MetaAI` | ✔️ | ❌ | [meta.ai](https://www.meta.ai) |
 | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
 | Reka | `g4f.Provider.Reka` | ❌ | ✔️ | [chat.reka.ai](https://chat.reka.ai/) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e-3| ✔️ | [you.com](https://you.com) |
 
-```python
-import requests
-from g4f.client import Client
-
-client = Client()
-image = requests.get("https://change_me.jpg", stream=True).raw
-response = client.chat.completions.create(
-    "",
-    messages=[{"role": "user", "content": "what is in this picture?"}],
-    image=image
-)
-print(response.choices[0].message.content)
-```
 
 ## 🔗 Powered by gpt4free
 
 <table>
   <thead align="center">
     <tr border: none;>
       <td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.8 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.9 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -391,19 +391,15 @@
 | `g4f.Provider.GeminiPro` | â | gemini-1.5-pro | [ai.google.dev](https://
 ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | âï¸ | â | [meta.ai]
 (https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
 3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Reka |
 `g4f.Provider.Reka` | â | âï¸ | [chat.reka.ai](https://chat.reka.ai/) | |
 Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b |
 [replicate.com](https://replicate.com) | | You.com | `g4f.Provider.You` | dall-
-e-3| âï¸ | [you.com](https://you.com) | ```python import requests from
-g4f.client import Client client = Client() image = requests.get("https://
-change_me.jpg", stream=True).raw response = client.chat.completions.create( "",
-messages=[{"role": "user", "content": "what is in this picture?"}], image=image
-) print(response.choices[0].message.content) ``` ## ð Powered by gpt4free
+e-3| âï¸ | [you.com](https://you.com) | ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
```

### Comparing `g4f-0.3.1.8/README.md` & `g4f-0.3.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -437,27 +437,14 @@
 | Gemini API | `g4f.Provider.GeminiPro` | ❌ | gemini-1.5-pro | [ai.google.dev](https://ai.google.dev) |
 | Meta AI | `g4f.Provider.MetaAI` | ✔️ | ❌ | [meta.ai](https://www.meta.ai) |
 | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
 | Reka | `g4f.Provider.Reka` | ❌ | ✔️ | [chat.reka.ai](https://chat.reka.ai/) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e-3| ✔️ | [you.com](https://you.com) |
 
-```python
-import requests
-from g4f.client import Client
-
-client = Client()
-image = requests.get("https://change_me.jpg", stream=True).raw
-response = client.chat.completions.create(
-    "",
-    messages=[{"role": "user", "content": "what is in this picture?"}],
-    image=image
-)
-print(response.choices[0].message.content)
-```
 
 ## 🔗 Powered by gpt4free
 
 <table>
   <thead align="center">
     <tr border: none;>
       <td>
```

#### html2text {}

```diff
@@ -349,19 +349,15 @@
 | `g4f.Provider.GeminiPro` | â | gemini-1.5-pro | [ai.google.dev](https://
 ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | âï¸ | â | [meta.ai]
 (https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
 3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Reka |
 `g4f.Provider.Reka` | â | âï¸ | [chat.reka.ai](https://chat.reka.ai/) | |
 Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b |
 [replicate.com](https://replicate.com) | | You.com | `g4f.Provider.You` | dall-
-e-3| âï¸ | [you.com](https://you.com) | ```python import requests from
-g4f.client import Client client = Client() image = requests.get("https://
-change_me.jpg", stream=True).raw response = client.chat.completions.create( "",
-messages=[{"role": "user", "content": "what is in this picture?"}], image=image
-) print(response.choices[0].message.content) ``` ## ð Powered by gpt4free
+e-3| âï¸ | [you.com](https://you.com) | ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
```

### Comparing `g4f-0.3.1.8/g4f/Provider/Aichatos.py` & `g4f-0.3.1.9/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Aura.py` & `g4f-0.3.1.9/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Bing.py` & `g4f-0.3.1.9/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/BingCreateImages.py` & `g4f-0.3.1.9/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Blackbox.py` & `g4f-0.3.1.9/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/ChatForAi.py` & `g4f-0.3.1.9/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.1.9/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/ChatgptAi.py` & `g4f-0.3.1.9/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/ChatgptFree.py` & `g4f-0.3.1.9/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/ChatgptNext.py` & `g4f-0.3.1.9/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/ChatgptX.py` & `g4f-0.3.1.9/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Cnote.py` & `g4f-0.3.1.9/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Cohere.py` & `g4f-0.3.1.9/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/DeepInfra.py` & `g4f-0.3.1.9/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.1.9/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.1.9/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Ecosia.py` & `g4f-0.3.1.9/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Feedough.py` & `g4f-0.3.1.9/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/FlowGpt.py` & `g4f-0.3.1.9/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.1.9/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/FreeGpt.py` & `g4f-0.3.1.9/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/GeminiPro.py` & `g4f-0.3.1.9/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/GeminiProChat.py` & `g4f-0.3.1.9/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/GigaChat.py` & `g4f-0.3.1.9/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/GptTalkRu.py` & `g4f-0.3.1.9/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/HuggingChat.py` & `g4f-0.3.1.9/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/HuggingFace.py` & `g4f-0.3.1.9/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Koala.py` & `g4f-0.3.1.9/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Liaobots.py` & `g4f-0.3.1.9/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Llama.py` & `g4f-0.3.1.9/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Local.py` & `g4f-0.3.1.9/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/MetaAI.py` & `g4f-0.3.1.9/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.1.9/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Ollama.py` & `g4f-0.3.1.9/g4f/Provider/Ollama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.1.9/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Pi.py` & `g4f-0.3.1.9/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Reka.py` & `g4f-0.3.1.9/g4f/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Replicate.py` & `g4f-0.3.1.9/g4f/Provider/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/ReplicateImage.py` & `g4f-0.3.1.9/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/Vercel.py` & `g4f-0.3.1.9/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.1.9/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/You.py` & `g4f-0.3.1.9/g4f/Provider/You.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import base64
 import uuid
 
 from ..typing import AsyncResult, Messages, ImageType, Cookies
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .helper import format_prompt
-from ..image import ImageResponse, ImagePreview, to_bytes, is_accepted_format
+from ..image import ImageResponse, ImagePreview, EXTENSIONS_MAP, to_bytes, is_accepted_format
 from ..requests import StreamSession, FormData, raise_for_status
 from .you.har_file import get_telemetry_ids
 from .. import debug
 
 class You(AsyncGeneratorProvider, ProviderModelMixin):
     label = "You.com"
     url = "https://you.com"
@@ -90,28 +90,30 @@
                 "Referer": f"{cls.url}/search?fromSearchBar=true&tbm=youchat",
             }
             data = {
                 "userFiles": upload,
                 "q": format_prompt(messages),
                 "domain": "youchat",
                 "selectedChatMode": chat_mode,
+                "conversationTurnId": str(uuid.uuid4()),
+                "chatId": str(uuid.uuid4()),
             }
             params = {
                 "userFiles": upload,
                 "selectedChatMode": chat_mode,
             }
             if chat_mode == "custom":
                 if debug.logging:
                     print(f"You model: {model}")
                 params["selectedAiModel"] = model.replace("-", "_")
 
             async with (session.post if chat_mode == "default" else session.get)(
                 f"{cls.url}/api/streamingSearch",
-                data=data,
-                params=params,
+                data=data if chat_mode == "default" else None,
+                params=params if chat_mode == "default" else data,
                 headers=headers,
                 cookies=cookies
             ) as response:
                 await raise_for_status(response)
                 async for line in response.iter_lines():
                     if line.startswith(b'event: '):
                         event = line[7:].decode()
@@ -138,15 +140,17 @@
         async with client.get(
             f"{cls.url}/api/get_nonce",
             cookies=cookies,
         ) as response:
             await raise_for_status(response)
             upload_nonce = await response.text()
         data = FormData()
-        data.add_field('file', file, content_type=is_accepted_format(file), filename=filename)
+        content_type = is_accepted_format(file)
+        filename = f"image.{EXTENSIONS_MAP[content_type]}" if filename is None else filename
+        data.add_field('file', file, content_type=content_type, filename=filename)
         async with client.post(
             f"{cls.url}/api/upload",
             data=data,
             headers={
                 "X-Upload-Nonce": upload_nonce,
             },
             cookies=cookies
```

### Comparing `g4f-0.3.1.8/g4f/Provider/__init__.py` & `g4f-0.3.1.9/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/bing/conversation.py` & `g4f-0.3.1.9/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/bing/create_images.py` & `g4f-0.3.1.9/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/bing/upload_image.py` & `g4f-0.3.1.9/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/V50.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.1.9/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.1.9/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/Gemini.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,29 +14,29 @@
     from selenium.webdriver.support.ui import WebDriverWait
     from selenium.webdriver.support import expected_conditions as EC
 except ImportError:
     pass
 
 from ... import debug
 from ...typing import Messages, Cookies, ImageType, AsyncResult, AsyncIterator
-from ..base_provider import AsyncGeneratorProvider
+from ..base_provider import AsyncGeneratorProvider, BaseConversation
 from ..helper import format_prompt, get_cookies
 from ...requests.raise_for_status import raise_for_status
 from ...errors import MissingAuthError, MissingRequirementsError
-from ...image import to_bytes, ImageResponse, ImageDataResponse
+from ...image import ImageResponse, to_bytes
 from ...webdriver import get_browser, get_driver_cookies
 
 REQUEST_HEADERS = {
     "authority": "gemini.google.com",
     "origin": "https://gemini.google.com",
     "referer": "https://gemini.google.com/",
     'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
     'x-same-domain': '1',
 }
-REQUEST_BL_PARAM = "boq_assistant-bard-web-server_20240421.18_p0"
+REQUEST_BL_PARAM = "boq_assistant-bard-web-server_20240519.16_p0"
 REQUEST_URL = "https://gemini.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate"
 UPLOAD_IMAGE_URL = "https://content-push.googleapis.com/upload/"
 UPLOAD_IMAGE_HEADERS = {
     "authority": "content-push.googleapis.com",
     "accept": "*/*",
     "accept-language": "en-US,en;q=0.7",
     "authorization": "Basic c2F2ZXM6cyNMdGhlNmxzd2F2b0RsN3J1d1U=",
@@ -53,14 +53,16 @@
 class Gemini(AsyncGeneratorProvider):
     url = "https://gemini.google.com"
     needs_auth = True
     working = True
     image_models = ["gemini"]
     default_vision_model = "gemini"
     _cookies: Cookies = None
+    _snlm0e: str = None
+    _sid: str = None
 
     @classmethod
     async def nodriver_login(cls, proxy: str = None) -> AsyncIterator[str]:
         try:
             import nodriver as uc
         except ImportError:
             return
@@ -113,87 +115,103 @@
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
-        api_key: str = None,
         cookies: Cookies = None,
         connector: BaseConnector = None,
         image: ImageType = None,
         image_name: str = None,
         response_format: str = None,
+        return_conversation: bool = False,
+        conversation: Conversation = None,
+        language: str = "en",
         **kwargs
     ) -> AsyncResult:
-        prompt = format_prompt(messages)
-        if api_key is not None:
-            if cookies is None:
-                cookies = {}
-            cookies["__Secure-1PSID"] = api_key
+        prompt = format_prompt(messages) if conversation is None else messages[-1]["content"]
         cls._cookies = cookies or cls._cookies or get_cookies(".google.com", False, True)
         base_connector = get_connector(connector, proxy)
         async with ClientSession(
             headers=REQUEST_HEADERS,
             connector=base_connector
         ) as session:
-            snlm0e  = await cls.fetch_snlm0e(session, cls._cookies) if cls._cookies else None
-            if not snlm0e:
+            if not cls._snlm0e:
+                await cls.fetch_snlm0e(session, cls._cookies) if cls._cookies else None
+            if not cls._snlm0e:
                 async for chunk in cls.nodriver_login(proxy):
                     yield chunk
                 if cls._cookies is None:
                     async for chunk in cls.webdriver_login(proxy):
                         yield chunk
-
-            if not snlm0e:
+            if not cls._snlm0e:
                 if cls._cookies is None or "__Secure-1PSID" not in cls._cookies:
                     raise MissingAuthError('Missing "__Secure-1PSID" cookie')
-                snlm0e = await cls.fetch_snlm0e(session, cls._cookies)
-            if not snlm0e:
+                await cls.fetch_snlm0e(session, cls._cookies)
+            if not cls._snlm0e:
                 raise RuntimeError("Invalid cookies. SNlM0e not found")
 
             image_url = await cls.upload_image(base_connector, to_bytes(image), image_name) if image else None
-        
+
             async with ClientSession(
                 cookies=cls._cookies,
                 headers=REQUEST_HEADERS,
                 connector=base_connector,
             ) as client:
                 params = {
                     'bl': REQUEST_BL_PARAM,
+                    'hl': language,
                     '_reqid': random.randint(1111, 9999),
-                    'rt': 'c'
+                    'rt': 'c',
+                    "f.sid": cls._sid,
                 }
                 data = {
-                    'at': snlm0e,
+                    'at': cls._snlm0e,
                     'f.req': json.dumps([None, json.dumps(cls.build_request(
                         prompt,
+                        language=language,
+                        conversation=conversation,
                         image_url=image_url,
                         image_name=image_name
                     ))])
                 }
                 async with client.post(
                     REQUEST_URL,
                     data=data,
                     params=params,
                 ) as response:
                     await raise_for_status(response)
-                    response = await response.text()
-                    response_part = json.loads(json.loads(response.splitlines()[-5])[0][2])
-                    if response_part[4] is None:
-                        response_part = json.loads(json.loads(response.splitlines()[-7])[0][2])
-
-                    content = response_part[4][0][1][0]
-                    image_prompt = None
-                    match = re.search(r'\[Imagen of (.*?)\]', content)
-                    if match:
-                        image_prompt = match.group(1)
-                        content = content.replace(match.group(0), '')
-
-                    yield content
+                    image_prompt = response_part = None
+                    last_content_len = 0
+                    async for line in response.content:
+                        try:
+                            try:
+                                line = json.loads(line)
+                            except ValueError:
+                                continue
+                            if not isinstance(line, list):
+                                continue
+                            if len(line[0]) < 3 or not line[0][2]:
+                                continue
+                            response_part = json.loads(line[0][2])
+                            if not response_part[4]:
+                                continue
+                            if return_conversation:
+                                yield Conversation(response_part[1][0], response_part[1][1], response_part[4][0][0])
+                            content = response_part[4][0][1][0]
+                        except (ValueError, KeyError, TypeError, IndexError) as e:
+                            print(f"{cls.__name__}:{e.__class__.__name__}:{e}")
+                            continue
+                        match = re.search(r'\[Imagen of (.*?)\]', content)
+                        if match:
+                            image_prompt = match.group(1)
+                            content = content.replace(match.group(0), '')
+                        yield content[last_content_len:]
+                        last_content_len = len(content)
                     if image_prompt:
                         images = [image[0][3][3] for image in response_part[4][0][12][7][0]]
                         if response_format == "b64_json":
                             yield ImageResponse(images, image_prompt, {"cookies": cls._cookies})
                         else:
                             resolved_images = []
                             preview = []
@@ -204,26 +222,32 @@
                                     image = fetch.headers["location"]
                                 resolved_images.append(image)
                                 preview.append(image.replace('=s512', '=s200'))
                             yield ImageResponse(resolved_images, image_prompt, {"orginal_links": images, "preview": preview})
 
     def build_request(
         prompt: str,
-        conversation_id: str = "",
-        response_id: str = "",
-        choice_id: str = "",
+        language: str,
+        conversation: Conversation = None,
         image_url: str = None,
         image_name: str = None,
         tools: list[list[str]] = []
     ) -> list:
         image_list = [[[image_url, 1], image_name]] if image_url else []
         return [
             [prompt, 0, None, image_list, None, None, 0],
-            ["en"],
-            [conversation_id, response_id, choice_id, None, None, []],
+            [language],
+            [
+                None if conversation is None else conversation.conversation_id,
+                None if conversation is None else conversation.response_id,
+                None if conversation is None else conversation.choice_id,
+                None,
+                None,
+                []
+            ],
             None,
             None,
             None,
             [1],
             0,
             [],
             tools,
@@ -261,11 +285,24 @@
                 await raise_for_status(response)
                 return await response.text()
 
     @classmethod
     async def fetch_snlm0e(cls, session: ClientSession, cookies: Cookies):
         async with session.get(cls.url, cookies=cookies) as response:
             await raise_for_status(response)
-            text = await response.text()
-        match = re.search(r'SNlM0e\":\"(.*?)\"', text)
+            response_text = await response.text()
+        match = re.search(r'SNlM0e\":\"(.*?)\"', response_text)
         if match:
-            return match.group(1)
+            cls._snlm0e = match.group(1)
+        sid_match = re.search(r'"FdrFJe":"([\d-]+)"', response_text)
+        if sid_match:
+            cls._sid = sid_match.group(1)
+
+class Conversation(BaseConversation):
+    def __init__(self,
+        conversation_id: str = "",
+        response_id: str = "",
+        choice_id: str = ""
+    ) -> None:
+        self.conversation_id = conversation_id
+        self.response_id = response_id
+        self.choice_id = choice_id
```

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/PerplexityApi.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/PerplexityApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.1.9/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.1.9/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.1.9/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.1.9/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.1.9/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.1.9/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.1.9/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.1.9/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.1.9/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.1.9/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.1.9/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.1.9/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.1.9/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.1.9/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.1.9/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.1.9/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/npm/package-lock.json` & `g4f-0.3.1.9/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/openai/crypt.py` & `g4f-0.3.1.9/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/openai/har_file.py` & `g4f-0.3.1.9/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/openai/proofofwork.py` & `g4f-0.3.1.9/g4f/Provider/openai/proofofwork.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.1.9/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/selenium/Bard.py` & `g4f-0.3.1.9/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.1.9/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.1.9/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/selenium/Phind.py` & `g4f-0.3.1.9/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.1.9/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.1.9/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.1.9/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.1.9/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.1.9/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/Provider/you/har_file.py` & `g4f-0.3.1.9/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/__init__.py` & `g4f-0.3.1.9/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/api/__init__.py` & `g4f-0.3.1.9/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/api/_logging.py` & `g4f-0.3.1.9/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/cli.py` & `g4f-0.3.1.9/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/client/async_client.py` & `g4f-0.3.1.9/g4f/client/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .image_models import ImageModels
 from .helper import filter_json, find_stop, filter_none, cast_iter_async
 from .service import get_last_provider, get_model_and_provider
 from ..Provider import ProviderUtils
 from ..typing import Union, Messages, AsyncIterator, ImageType
 from ..errors import NoImageResponseError, ProviderNotFoundError
 from ..requests.aiohttp import get_connector
+from ..providers.conversation import BaseConversation
 from ..image import ImageResponse as ImageProviderResponse, ImageDataResponse
 
 try:
     anext
 except NameError:
     async def anext(iter):
         async for chunk in iter:
@@ -38,14 +39,17 @@
     finish_reason = None
     completion_id = ''.join(random.choices(string.ascii_letters + string.digits, k=28))
     count: int = 0
     async for chunk in response:
         if isinstance(chunk, FinishReason):
             finish_reason = chunk.reason
             break
+        elif isinstance(chunk, BaseConversation):
+            yield chunk
+            continue
         content += str(chunk)
         count += 1
         if max_tokens is not None and count >= max_tokens:
             finish_reason = "length"
         first, content, chunk = find_stop(stop, content, chunk)
         if first != -1:
             finish_reason = "stop"
```

### Comparing `g4f-0.3.1.8/g4f/client/client.py` & `g4f-0.3.1.9/g4f/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import time
 import random
 import string
 
 from ..typing import Union, Iterator, Messages, ImageType
 from ..providers.types import BaseProvider, ProviderType, FinishReason
+from ..providers.conversation import BaseConversation
 from ..image import ImageResponse as ImageProviderResponse
 from ..errors import NoImageResponseError
 from .stubs import ChatCompletion, ChatCompletionChunk, Image, ImagesResponse
 from .image_models import ImageModels
 from .types import IterResponse, ImageProvider
 from .types import Client as BaseClient
 from .service import get_model_and_provider, get_last_provider
@@ -25,14 +26,17 @@
     content = ""
     finish_reason = None
     completion_id = ''.join(random.choices(string.ascii_letters + string.digits, k=28))
     for idx, chunk in enumerate(response):
         if isinstance(chunk, FinishReason):
             finish_reason = chunk.reason
             break
+        elif isinstance(chunk, BaseConversation):
+            yield chunk
+            continue
         content += str(chunk)
         if max_tokens is not None and idx + 1 >= max_tokens:
             finish_reason = "length"
         first, content, chunk = find_stop(stop, content, chunk if stream else None)
         if first != -1:
             finish_reason = "stop"
         if stream:
```

### Comparing `g4f-0.3.1.8/g4f/client/helper.py` & `g4f-0.3.1.9/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/client/image_models.py` & `g4f-0.3.1.9/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/client/service.py` & `g4f-0.3.1.9/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/client/stubs.py` & `g4f-0.3.1.9/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/client/types.py` & `g4f-0.3.1.9/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/cookies.py` & `g4f-0.3.1.9/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/errors.py` & `g4f-0.3.1.9/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/__init__.py` & `g4f-0.3.1.9/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/index.html` & `g4f-0.3.1.9/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/css/dracula.min.css` & `g4f-0.3.1.9/g4f/gui/client/static/css/dracula.min.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/css/style.css` & `g4f-0.3.1.9/g4f/gui/client/static/css/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -1139,8 +1139,11 @@
     .conversation .toolbar,
     .conversation .slide-systemPrompt,
     .message .count i,
     .message .assistant,
     .message .user {
         display: none;
     }
+    .message.regenerate {
+        opacity: 1;
+    }
 }
```

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.1.9/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.1.9/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.1.9/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.1.9/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.1.9/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/img/user.png` & `g4f-0.3.1.9/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.1.9/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.1.9/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.1.9/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/js/icons.js` & `g4f-0.3.1.9/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.1.9/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.1.9/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.1.9/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/server/android_gallery.py` & `g4f-0.3.1.9/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/server/api.py` & `g4f-0.3.1.9/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/server/backend.py` & `g4f-0.3.1.9/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/server/config.py` & `g4f-0.3.1.9/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/server/internet.py` & `g4f-0.3.1.9/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/server/js_api.py` & `g4f-0.3.1.9/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/server/website.py` & `g4f-0.3.1.9/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/gui/webview.py` & `g4f-0.3.1.9/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/image.py` & `g4f-0.3.1.9/g4f/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 except ImportError:
     has_requirements = False
 
 from .errors import MissingRequirementsError
 
 ALLOWED_EXTENSIONS = {'png', 'jpg', 'jpeg', 'gif', 'webp', 'svg'}
 
+EXTENSIONS_MAP: dict[str, str] = {
+    "image/png": "png",
+    "image/jpeg": "jpg",
+    "image/gif": "gif",
+    "image/webp": "webp",
+}
+
 def to_image(image: ImageType, is_svg: bool = False) -> Image:
     """
     Converts the input image to a PIL Image object.
 
     Args:
         image (Union[str, bytes, Image]): The input image.
```

### Comparing `g4f-0.3.1.8/g4f/local/__init__.py` & `g4f-0.3.1.9/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/locals/models.py` & `g4f-0.3.1.9/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/locals/provider.py` & `g4f-0.3.1.9/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/models.py` & `g4f-0.3.1.9/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/providers/base_provider.py` & `g4f-0.3.1.9/g4f/providers/base_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,21 @@
                 asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
     except ImportError:
         pass
 
 def get_running_loop(check_nested: bool) -> Union[AbstractEventLoop, None]:
     try:
         loop = asyncio.get_running_loop()
+        # Do not patch uvloop loop because its incompatible.
+        try:
+            import uvloop
+            if isinstance(loop, uvloop.Loop):
+                return loop
+        except (ImportError, ModuleNotFoundError):
+            pass
         if check_nested and not hasattr(loop.__class__, "_nest_patched"):
             try:
                 import nest_asyncio
                 nest_asyncio.apply(loop)
             except ImportError:
                 raise NestAsyncioError('Install "nest_asyncio" package')
         return loop
@@ -286,8 +293,8 @@
         if not model and cls.default_model is not None:
             model = cls.default_model
         elif model in cls.model_aliases:
             model = cls.model_aliases[model]
         elif model not in cls.get_models() and cls.models:
             raise ModelNotSupportedError(f"Model is not supported: {model} in: {cls.__name__}")
         debug.last_model = model
-        return model
+        return model
```

### Comparing `g4f-0.3.1.8/g4f/providers/create_images.py` & `g4f-0.3.1.9/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/providers/helper.py` & `g4f-0.3.1.9/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/providers/retry_provider.py` & `g4f-0.3.1.9/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/providers/types.py` & `g4f-0.3.1.9/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/requests/__init__.py` & `g4f-0.3.1.9/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/requests/aiohttp.py` & `g4f-0.3.1.9/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/requests/curl_cffi.py` & `g4f-0.3.1.9/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/requests/defaults.py` & `g4f-0.3.1.9/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/requests/raise_for_status.py` & `g4f-0.3.1.9/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/stubs.py` & `g4f-0.3.1.9/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/typing.py` & `g4f-0.3.1.9/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/version.py` & `g4f-0.3.1.9/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f/webdriver.py` & `g4f-0.3.1.9/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f.egg-info/PKG-INFO` & `g4f-0.3.1.9/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.8
+Version: 0.3.1.9
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -515,27 +515,14 @@
 | Gemini API | `g4f.Provider.GeminiPro` | ❌ | gemini-1.5-pro | [ai.google.dev](https://ai.google.dev) |
 | Meta AI | `g4f.Provider.MetaAI` | ✔️ | ❌ | [meta.ai](https://www.meta.ai) |
 | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
 | Reka | `g4f.Provider.Reka` | ❌ | ✔️ | [chat.reka.ai](https://chat.reka.ai/) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e-3| ✔️ | [you.com](https://you.com) |
 
-```python
-import requests
-from g4f.client import Client
-
-client = Client()
-image = requests.get("https://change_me.jpg", stream=True).raw
-response = client.chat.completions.create(
-    "",
-    messages=[{"role": "user", "content": "what is in this picture?"}],
-    image=image
-)
-print(response.choices[0].message.content)
-```
 
 ## 🔗 Powered by gpt4free
 
 <table>
   <thead align="center">
     <tr border: none;>
       <td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.8 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.9 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -391,19 +391,15 @@
 | `g4f.Provider.GeminiPro` | â | gemini-1.5-pro | [ai.google.dev](https://
 ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | âï¸ | â | [meta.ai]
 (https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
 3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Reka |
 `g4f.Provider.Reka` | â | âï¸ | [chat.reka.ai](https://chat.reka.ai/) | |
 Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b |
 [replicate.com](https://replicate.com) | | You.com | `g4f.Provider.You` | dall-
-e-3| âï¸ | [you.com](https://you.com) | ```python import requests from
-g4f.client import Client client = Client() image = requests.get("https://
-change_me.jpg", stream=True).raw response = client.chat.completions.create( "",
-messages=[{"role": "user", "content": "what is in this picture?"}], image=image
-) print(response.choices[0].message.content) ``` ## ð Powered by gpt4free
+e-3| âï¸ | [you.com](https://you.com) | ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
```

### Comparing `g4f-0.3.1.8/g4f.egg-info/SOURCES.txt` & `g4f-0.3.1.9/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/g4f.egg-info/requires.txt` & `g4f-0.3.1.9/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.8/setup.py` & `g4f-0.3.1.9/setup.py`

 * *Files identical despite different names*

