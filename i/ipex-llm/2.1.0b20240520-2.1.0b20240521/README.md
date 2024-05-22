# Comparing `tmp/ipex_llm-2.1.0b20240520-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240521-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5372996 bytes, number of entries: 192
+Zip file size: 5370551 bytes, number of entries: 192
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3232 b- defN 24-May-07 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,61 +38,61 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-May-20 15:07 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-May-20 15:07 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   473088 b- defN 24-May-20 15:07 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   854016 b- defN 24-May-20 15:07 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856576 b- defN 24-May-20 15:07 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   844800 b- defN 24-May-20 15:07 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-May-20 15:07 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   532992 b- defN 24-May-20 15:07 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   499712 b- defN 24-May-20 15:07 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   473600 b- defN 24-May-20 15:07 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   559104 b- defN 24-May-20 15:07 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   533504 b- defN 24-May-20 15:07 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   553472 b- defN 24-May-20 15:07 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   527872 b- defN 24-May-20 15:07 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   590848 b- defN 24-May-20 15:07 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   564736 b- defN 24-May-20 15:07 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-May-20 15:07 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   526848 b- defN 24-May-20 15:07 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-May-20 15:07 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726528 b- defN 24-May-20 15:07 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-May-20 15:07 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-May-20 15:07 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-May-20 15:07 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   126464 b- defN 24-May-20 15:07 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-May-20 15:07 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-May-20 15:07 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-May-20 15:07 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-May-20 15:07 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-May-20 15:07 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-May-20 15:07 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128512 b- defN 24-May-20 15:07 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-May-20 15:07 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   564224 b- defN 24-May-20 15:07 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-May-21 15:07 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-May-21 15:07 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   473088 b- defN 24-May-21 15:07 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   854016 b- defN 24-May-21 15:07 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856576 b- defN 24-May-21 15:07 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   844800 b- defN 24-May-21 15:07 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-May-21 15:07 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   532992 b- defN 24-May-21 15:07 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   499712 b- defN 24-May-21 15:07 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   473600 b- defN 24-May-21 15:07 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   559104 b- defN 24-May-21 15:07 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   533504 b- defN 24-May-21 15:07 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   553472 b- defN 24-May-21 15:07 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   527872 b- defN 24-May-21 15:07 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   590848 b- defN 24-May-21 15:07 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   564736 b- defN 24-May-21 15:07 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-May-21 15:07 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   526848 b- defN 24-May-21 15:07 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-May-21 15:07 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726528 b- defN 24-May-21 15:07 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-May-21 15:07 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-May-21 15:07 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-May-21 15:07 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   126464 b- defN 24-May-21 15:07 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-May-21 15:07 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-May-21 15:07 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-May-21 15:07 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-May-21 15:07 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-May-21 15:07 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-May-21 15:07 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128512 b- defN 24-May-21 15:07 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-May-21 15:07 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   564224 b- defN 24-May-21 15:07 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    19605 b- defN 24-May-20 15:06 ipex_llm/serving/fastchat/ipex_llm_worker.py
 -rw-------  2.0 unx    16649 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/model_worker.py
 -rw-------  2.0 unx     5918 b- defN 24-May-20 15:06 ipex_llm/serving/fastchat/tgi_api_protocol.py
 -rw-------  2.0 unx    27062 b- defN 24-May-20 15:06 ipex_llm/serving/fastchat/tgi_api_server.py
 -rw-------  2.0 unx    10801 b- defN 24-Apr-29 15:08 ipex_llm/serving/fastchat/vllm_worker.py
 -rw-------  2.0 unx     1005 b- defN 24-Mar-25 11:36 ipex_llm/transformers/__init__.py
 -rw-------  2.0 unx     1213 b- defN 24-Mar-25 11:36 ipex_llm/transformers/bmm.py
--rw-------  2.0 unx    74215 b- defN 24-May-20 15:06 ipex_llm/transformers/convert.py
+-rw-------  2.0 unx    74370 b- defN 24-May-21 15:06 ipex_llm/transformers/convert.py
 -rw-------  2.0 unx    14334 b- defN 24-Apr-26 15:08 ipex_llm/transformers/convert_ipex.py
 -rw-------  2.0 unx     4613 b- defN 24-Mar-25 11:36 ipex_llm/transformers/embedding.py
 -rw-------  2.0 unx     4247 b- defN 24-Apr-29 15:08 ipex_llm/transformers/kv.py
 -rw-------  2.0 unx     3289 b- defN 24-Apr-18 12:34 ipex_llm/transformers/lisa.py
 -rw-------  2.0 unx     6812 b- defN 24-May-13 15:08 ipex_llm/transformers/loader.py
 -rw-------  2.0 unx    15562 b- defN 24-May-16 02:22 ipex_llm/transformers/lookup.py
 -rw-------  2.0 unx    39885 b- defN 24-May-17 15:06 ipex_llm/transformers/low_bit_linear.py
@@ -153,17 +153,17 @@
 -rw-------  2.0 unx    54855 b- defN 24-May-14 15:08 ipex_llm/transformers/models/mistral.py
 -rw-------  2.0 unx    27151 b- defN 24-May-14 15:08 ipex_llm/transformers/models/mixtral.py
 -rw-------  2.0 unx     9540 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/mpt.py
 -rw-------  2.0 unx     7668 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/phi.py
 -rw-------  2.0 unx    11908 b- defN 24-May-17 15:06 ipex_llm/transformers/models/phi3.py
 -rw-------  2.0 unx     6268 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/phixtral.py
 -rw-------  2.0 unx    17305 b- defN 24-May-20 15:06 ipex_llm/transformers/models/qwen.py
--rw-------  2.0 unx    37312 b- defN 24-May-14 15:08 ipex_llm/transformers/models/qwen2.py
+-rw-------  2.0 unx    16252 b- defN 24-May-21 15:06 ipex_llm/transformers/models/qwen2.py
 -rw-------  2.0 unx    38469 b- defN 24-May-16 06:00 ipex_llm/transformers/models/qwen2_moe.py
--rw-------  2.0 unx    11712 b- defN 24-May-14 15:08 ipex_llm/transformers/models/qwen_vl.py
+-rw-------  2.0 unx     9163 b- defN 24-May-21 15:06 ipex_llm/transformers/models/qwen_vl.py
 -rw-------  2.0 unx     6135 b- defN 24-Mar-29 11:38 ipex_llm/transformers/models/rwkv4.py
 -rw-------  2.0 unx    10722 b- defN 24-Apr-09 15:06 ipex_llm/transformers/models/rwkv5.py
 -rw-------  2.0 unx    20911 b- defN 24-May-14 15:08 ipex_llm/transformers/models/stablelm.py
 -rw-------  2.0 unx     8805 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/starcoder2.py
 -rw-------  2.0 unx    19883 b- defN 24-May-17 15:06 ipex_llm/transformers/models/utils.py
 -rw-------  2.0 unx    20200 b- defN 24-Apr-26 15:08 ipex_llm/transformers/models/yuan.py
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/utils/__init__.py
@@ -180,15 +180,15 @@
 -rw-------  2.0 unx     1763 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/log4Error.py
 -rw-------  2.0 unx      585 b- defN 24-Apr-22 15:07 ipex_llm/vllm/__init__.py
 -rw-------  2.0 unx    18514 b- defN 24-Apr-26 15:08 ipex_llm/vllm/ipex_llm_gpu_executor.py
 -rw-------  2.0 unx     7208 b- defN 24-Apr-22 15:07 ipex_llm/vllm/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/__init__.py
 -rw-------  2.0 unx     5941 b- defN 24-Apr-26 15:08 ipex_llm/vllm/engine/engine.py
 -rw-------  2.0 unx    10564 b- defN 24-Apr-22 15:07 ipex_llm/vllm/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240520.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240520.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     4965 b- defN 24-May-20 15:07 ipex_llm-2.1.0b20240520.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-May-20 15:07 ipex_llm-2.1.0b20240520.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-May-20 15:07 ipex_llm-2.1.0b20240520.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-May-20 15:07 ipex_llm-2.1.0b20240520.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    18216 b- defN 24-May-20 15:07 ipex_llm-2.1.0b20240520.dist-info/RECORD
-192 files, 13318647 bytes uncompressed, 5343896 bytes compressed:  59.9%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240521.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240521.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     4965 b- defN 24-May-21 15:07 ipex_llm-2.1.0b20240521.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-May-21 15:07 ipex_llm-2.1.0b20240521.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-May-21 15:07 ipex_llm-2.1.0b20240521.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-May-21 15:07 ipex_llm-2.1.0b20240521.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    18215 b- defN 24-May-21 15:07 ipex_llm-2.1.0b20240521.dist-info/RECORD
+192 files, 13295192 bytes uncompressed, 5341451 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -549,29 +549,29 @@
 
 Filename: ipex_llm/vllm/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240520.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240521.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240520.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240521.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240520.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240521.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240520.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240521.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240520.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240521.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240520.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240521.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240520.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240521.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:44 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,16 +6375,16 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	adc    $0x66,%al
-   180005636:	rex.WXB
+   180005634:	(bad)
+   180005635:	mov    $0x4c,%bh
    180005637:	data16 add %al,(%rax)
    18000563a:	add    %al,(%rax)
    18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055a28
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:45 2024
+Time/Date		Tue May 21 15:03:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056000
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055a28
@@ -112394,17 +112394,19 @@
    18005e85d:	add    %al,(%rax)
    18005e85f:	add    %dh,0x76(%rax)
    18005e862:	add    $0x180,%eax
    18005e867:	add    %bh,0x76(%rax)
    18005e86a:	add    $0x180,%eax
    18005e86f:	add    %al,(%rax)
    18005e871:	add    %al,(%rax)
-   18005e873:	add    %dl,0x664b66(%rip)        # 0x1806c33df
-   18005e879:	add    %al,(%rax)
-   18005e87b:	add    %cl,0x50000000(%rip)        # 0x1d005e881
+   18005e873:	add    %dl,%ch
+   18005e875:	mov    $0x4c,%bh
+   18005e877:	data16 add %al,(%rax)
+   18005e87a:	add    %al,(%rax)
+   18005e87c:	or     $0x50000000,%eax
    18005e881:	add    (%rax),%eax
    18005e883:	add    %ah,-0x5ffffa0e(%rax)
    18005e889:	out    %al,$0x5
 	...
    18005e8ff:	add    %dl,(%rax)
    18005e901:	testb  $0x0,0x180(%rip)        # 0x18005ea88
    18005e908:	sbb    %dh,%dh
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:44 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,16 +5058,16 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	adc    $0x66,%al
-   1800049d6:	rex.WXB
+   1800049d4:	(bad)
+   1800049d5:	mov    $0x4c,%bh
    1800049d7:	data16 add %al,(%rax)
    1800049da:	add    %al,(%rax)
    1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d188
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:45 2024
+Time/Date		Tue May 21 15:03:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005da00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d188
@@ -123782,15 +123782,15 @@
    18006611d:	add    %al,(%rax)
    18006611f:	add    %bh,0x18005f6(%rax)
    180066125:	add    %al,(%rax)
    180066127:	add    %al,%al
    180066129:	testb  $0x0,0x180(%rip)        # 0x1800662b0
    180066130:	add    %al,(%rax)
    180066132:	add    %al,(%rax)
-   180066134:	adc    $0x664b66,%eax
+   180066134:	{rex2 0xb7} cmovl 0x0(%r30),%r12d
    180066139:	add    %al,(%rax)
    18006613b:	add    %cl,0x50000000(%rip)        # 0x1d0066141
    180066141:	add    (%rax),%eax
    180066143:	add    %al,0x5b840006(%rbp,%rbp,2)
    18006614a:	(bad)
 	...
    18006617f:	add    %bh,%al
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005bba8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:03:47 2024
+Time/Date		Tue May 21 15:02:55 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c200
 SizeOfInitializedData	00000000000bfa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005bba8
@@ -117909,19 +117909,17 @@
    18006578d:	add    %al,(%rax)
    18006578f:	add    %dh,-0x1a(%rax)
    180065792:	add    $0x180,%eax
    180065797:	add    %bh,-0x1a(%rax)
    18006579a:	add    $0x180,%eax
    18006579f:	add    %al,(%rax)
    1800657a1:	add    %al,(%rax)
-   1800657a3:	add    %dl,0x66(%rbx)
-   1800657a6:	rex.WXB
-   1800657a7:	data16 add %al,(%rax)
-   1800657aa:	add    %al,(%rax)
-   1800657ac:	or     $0x50000000,%eax
+   1800657a3:	add    %bl,0x664cb7(%rdi)
+   1800657a9:	add    %al,(%rax)
+   1800657ab:	add    %cl,0x50000000(%rip)        # 0x1d00657b1
    1800657b1:	add    (%rax),%eax
    1800657b3:	add    %ah,-0x5ffff99f(%rax)
    1800657b9:	rex.RXB (bad)
 	...
    1800657ff:	add    %dl,(%rax)
    180065801:	gs (bad)
    180065803:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055c38
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:58 2024
+Time/Date		Tue May 21 15:03:00 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056200
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055c38
@@ -112482,17 +112482,15 @@
    18005f83a:	add    $0x180,%eax
    18005f83f:	add    %dh,-0x7a(%rax)
    18005f842:	add    $0x180,%eax
    18005f847:	add    %bh,-0x7a(%rax)
    18005f84a:	add    $0x180,%eax
    18005f84f:	add    %al,(%rax)
    18005f851:	add    %al,(%rax)
-   18005f853:	add    %ah,(%rdx)
-   18005f855:	data16 rex.WXB
-   18005f857:	data16 add %al,(%rax)
+   18005f853:	add    %ah,0x664c(%rdi,%rsi,4)
    18005f85a:	add    %al,(%rax)
    18005f85c:	or     $0x50000000,%eax
    18005f861:	add    (%rax),%eax
    18005f863:	add    %ah,(%rax)
    18005f865:	add    (%rsi),%al
    18005f867:	add    %ah,(%rax)
    18005f869:	call   0x18005f873
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063398
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:03:48 2024
+Time/Date		Tue May 21 15:02:55 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063c00
 SizeOfInitializedData	00000000000c6a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063398
@@ -129360,16 +129360,16 @@
    18006c057:	add    %al,%al
    18006c059:	push   %rsi
    18006c05a:	(bad)
    18006c05b:	addb   $0x0,(%rcx)
    18006c05e:	add    %al,(%rax)
    18006c060:	add    %al,(%rax)
    18006c062:	add    %al,(%rax)
-   18006c064:	push   %rsp
-   18006c065:	data16 rex.WXB
+   18006c064:	lahf
+   18006c065:	mov    $0x4c,%bh
    18006c067:	data16 add %al,(%rax)
    18006c06a:	add    %al,(%rax)
    18006c06c:	or     $0x50000000,%eax
    18006c071:	add    (%rax),%eax
    18006c073:	add    %al,-0x437bfffa(%rsp,%rcx,8)
    18006c07a:	(bad)
    18006c07b:	add    %al,(%rax)
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d398
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:58 2024
+Time/Date		Tue May 21 15:03:01 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005dc00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d398
@@ -123919,15 +123919,16 @@
    1800660fd:	add    %al,(%rax)
    1800660ff:	add    %bh,0x18005f6(%rax)
    180066105:	add    %al,(%rax)
    180066107:	add    %al,%al
    180066109:	testb  $0x0,0x180(%rip)        # 0x180066290
    180066110:	add    %al,(%rax)
    180066112:	add    %al,(%rax)
-   180066114:	and    0x4b(%rsi),%ah
+   180066114:	movsl  %ds:(%rsi),%es:(%rdi)
+   180066115:	mov    $0x4c,%bh
    180066117:	data16 add %al,(%rax)
    18006611a:	add    %al,(%rax)
    18006611c:	or     $0x50000000,%eax
    180066121:	add    (%rax),%eax
    180066123:	add    %al,0x5d840006(%rbp,%rbp,2)
    18006612a:	(bad)
 	...
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800620a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:03:48 2024
+Time/Date		Tue May 21 15:02:55 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000062800
 SizeOfInitializedData	00000000000c6800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000620a8
@@ -128089,16 +128089,16 @@
    18006b134:	add    %eax,(%rax)
    18006b136:	add    %al,(%rax)
    18006b138:	rolb   $1,0x6(%rsi)
    18006b13b:	addb   $0x0,(%rcx)
    18006b13e:	add    %al,(%rax)
    18006b140:	add    %al,(%rax)
    18006b142:	add    %al,(%rax)
-   18006b144:	push   %rsp
-   18006b145:	data16 rex.WXB
+   18006b144:	lahf
+   18006b145:	mov    $0x4c,%bh
    18006b147:	data16 add %al,(%rax)
    18006b14a:	add    %al,(%rax)
    18006b14c:	or     $0x50000000,%eax
    18006b151:	add    (%rax),%eax
    18006b153:	add    %al,-0x7ffff943(%rax)
    18006b159:	test   $0x6,%eax
 	...
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c0a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:58 2024
+Time/Date		Tue May 21 15:03:01 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c800
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c0a8
@@ -122582,19 +122582,17 @@
    1800651e0:	enter  $0x5e6,$0x80
    1800651e4:	add    %eax,(%rax)
    1800651e6:	add    %al,(%rax)
    1800651e8:	shl    $1,%dh
    1800651ea:	add    $0x180,%eax
    1800651ef:	add    %al,(%rax)
    1800651f1:	add    %al,(%rax)
-   1800651f3:	add    %ah,(%rdx)
-   1800651f5:	data16 rex.WXB
-   1800651f7:	data16 add %al,(%rax)
-   1800651fa:	add    %al,(%rax)
-   1800651fc:	or     $0x50000000,%eax
+   1800651f3:	add    %ah,0x664cb7(%rbp)
+   1800651f9:	add    %al,(%rax)
+   1800651fb:	add    %cl,0x50000000(%rip)        # 0x1d0065201
    180065201:	add    (%rax),%eax
    180065203:	add    %al,-0x7ffff9a2(%rax)
    180065209:	rex.WX (bad)
 	...
    18006527f:	add    %dh,%al
    180065281:	(bad)
    180065282:	(bad)
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180069508
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:03:48 2024
+Time/Date		Tue May 21 15:02:55 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000069c00
 SizeOfInitializedData	00000000000c8600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000069508
@@ -138530,16 +138530,16 @@
    180072c85:	add    %al,(%rax)
    180072c87:	add    %al,%al
    180072c89:	mov    $0x6,%dh
    180072c8b:	addb   $0x0,(%rcx)
    180072c8e:	add    %al,(%rax)
    180072c90:	add    %al,(%rax)
    180072c92:	add    %al,(%rax)
-   180072c94:	push   %rsp
-   180072c95:	data16 rex.WXB
+   180072c94:	lahf
+   180072c95:	mov    $0x4c,%bh
    180072c97:	data16 add %al,(%rax)
    180072c9a:	add    %al,(%rax)
    180072c9c:	or     $0x50000000,%eax
    180072ca1:	add    (%rax),%eax
    180072ca3:	add    %dl,0x3e(%rax)
    180072ca6:	(bad)
    180072ca7:	add    %dl,0x2e(%rax)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063598
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:58 2024
+Time/Date		Tue May 21 15:03:00 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063c00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063598
@@ -133187,15 +133187,16 @@
    18006cd57:	add    %al,%al
    18006cd59:	push   %rsi
    18006cd5a:	(bad)
    18006cd5b:	addb   $0x0,(%rcx)
    18006cd5e:	add    %al,(%rax)
    18006cd60:	add    %al,(%rax)
    18006cd62:	add    %al,(%rax)
-   18006cd64:	and    0x4b(%rsi),%ah
+   18006cd64:	movsb  %ds:(%rsi),%es:(%rdi)
+   18006cd65:	mov    $0x4c,%bh
    18006cd67:	data16 add %al,(%rax)
    18006cd6a:	add    %al,(%rax)
    18006cd6c:	or     $0x50000000,%eax
    18006cd71:	add    (%rax),%eax
    18006cd73:	add    %dl,%al
    18006cd75:	fiadds (%rsi)
    18006cd77:	add    %dl,%al
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:44 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,16 +5355,16 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	adc    $0x66,%al
-   180004a36:	rex.WXB
+   180004a34:	(bad)
+   180004a35:	mov    $0x4c,%bh
    180004a37:	data16 add %al,(%rax)
    180004a3a:	add    %al,(%rax)
    180004a3c:	or     $0xe0000000,%eax
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005be98
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:45 2024
+Time/Date		Tue May 21 15:03:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c600
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005be98
@@ -122479,17 +122479,19 @@
    180065200:	enter  $0x5e6,$0x80
    180065204:	add    %eax,(%rax)
    180065206:	add    %al,(%rax)
    180065208:	shl    $1,%dh
    18006520a:	add    $0x180,%eax
    18006520f:	add    %al,(%rax)
    180065211:	add    %al,(%rax)
-   180065213:	add    %dl,0x664b66(%rip)        # 0x1806c9d7f
-   180065219:	add    %al,(%rax)
-   18006521b:	add    %cl,0x50000000(%rip)        # 0x1d0065221
+   180065213:	add    %dl,%ch
+   180065215:	mov    $0x4c,%bh
+   180065217:	data16 add %al,(%rax)
+   18006521a:	add    %al,(%rax)
+   18006521c:	or     $0x50000000,%eax
    180065221:	add    (%rax),%eax
    180065223:	add    %al,-0x7ffff9a2(%rax)
    180065229:	rex.W (bad)
 	...
    18006527f:	add    %dh,%al
    180065281:	(bad)
    180065282:	(bad)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:45 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,17 +25509,19 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	adc    $0x664b66,%eax
-   140014ac9:	add    %al,(%rax)
-   140014acb:	add    %cl,0x20000000(%rip)        # 0x160014ad1
+   140014ac4:	(bad)
+   140014ac5:	mov    $0x4c,%bh
+   140014ac7:	data16 add %al,(%rax)
+   140014aca:	add    %al,(%rax)
+   140014acc:	or     $0x20000000,%eax
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
    140014ad9:	rex add %eax,(%rax)
 	...
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:03:34 2024
+Time/Date		Tue May 21 15:03:35 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cc000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189033,16 +189033,16 @@
    140093fa5:	add    %al,(%rax)
    140093fa7:	add    %al,(%rax)
    140093fa9:	cltd
    140093faa:	or     %al,0x1(%rax)
    140093fad:	add    %al,(%rax)
    140093faf:	add    %al,(%rax)
    140093fb1:	add    %al,(%rax)
-   140093fb3:	add    %al,0x66(%rsi)
-   140093fb6:	rex.WXB
+   140093fb3:	add    %al,%bh
+   140093fb5:	mov    $0x4c,%bh
    140093fb7:	data16 add %al,(%rax)
    140093fba:	add    %al,(%rax)
    140093fbc:	or     $0xcc000000,%eax
    140093fc1:	add    (%rax),%eax
    140093fc3:	add    %dl,(%rax)
    140093fc5:	je     0x140093fd0
    140093fc7:	add    %dl,(%rax)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:45 2024
+Time/Date		Tue May 21 15:03:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,15 +24136,15 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	adc    $0x664b66,%eax
+   140013ef4:	{rex2 0xb7} cmovl 0x0(%r30),%r12d
    140013ef9:	add    %al,(%rax)
    140013efb:	add    %cl,-0x70000000(%rip)        # 0xd0013f01
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:44 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,16 +24679,16 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	adc    $0x66,%al
-   140013fc6:	rex.WXB
+   140013fc4:	(bad)
+   140013fc5:	mov    $0x4c,%bh
    140013fc7:	data16 add %al,(%rax)
    140013fca:	add    %al,(%rax)
    140013fcc:	or     $0x90000000,%eax
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:45 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,17 +40341,19 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %dl,0x664b66(%rip)        # 0x140683c8f
-   14001f129:	add    %al,(%rax)
-   14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
+   14001f123:	add    %dl,%ah
+   14001f125:	mov    $0x4c,%bh
+   14001f127:	data16 add %al,(%rax)
+   14001f12a:	add    %al,(%rax)
+   14001f12c:	or     $0x20000000,%eax
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
 	...
    14001f180:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:45 2024
+Time/Date		Tue May 21 15:03:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32234,17 +32234,19 @@
    140019225:	add    %al,(%rax)
    140019227:	add    %al,(%rax)
    140019229:	push   %rbp
    14001922a:	add    %eax,0x1(%rax)
    14001922d:	add    %al,(%rax)
    14001922f:	add    %al,(%rax)
    140019231:	add    %al,(%rax)
-   140019233:	add    %dl,0x664b66(%rip)        # 0x14067dd9f
-   140019239:	add    %al,(%rax)
-   14001923b:	add    %cl,0x20000000(%rip)        # 0x160019241
+   140019233:	add    %dl,%ch
+   140019235:	mov    $0x4c,%bh
+   140019237:	data16 add %al,(%rax)
+   14001923a:	add    %al,(%rax)
+   14001923c:	or     $0x20000000,%eax
    140019241:	add    (%rax),%eax
    140019243:	add    %dh,%al
    140019245:	movabs 0x18ff00001,%eax
 	...
    14001927e:	add    %al,(%rax)
    140019280:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:58 2024
+Time/Date		Tue May 21 15:03:00 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32372,17 +32372,15 @@
    140019205:	add    %al,(%rax)
    140019207:	add    %al,(%rax)
    140019209:	push   %rbp
    14001920a:	add    %eax,0x1(%rax)
    14001920d:	add    %al,(%rax)
    14001920f:	add    %al,(%rax)
    140019211:	add    %al,(%rax)
-   140019213:	add    %ah,(%rdx)
-   140019215:	data16 rex.WXB
-   140019217:	data16 add %al,(%rax)
+   140019213:	add    %ah,0x664c(%rdi,%rsi,4)
    14001921a:	add    %al,(%rax)
    14001921c:	or     $0x20000000,%eax
    140019221:	add    (%rax),%eax
    140019223:	add    %dh,%al
    140019225:	movabs 0x191f00001,%eax
 	...
    14001927e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:44 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27181,16 +27181,16 @@
    140016020:	push   $0x1400123
    140016025:	add    %al,(%rax)
    140016027:	add    %dh,0x23(%rax)
    14001602a:	add    %eax,0x1(%rax)
    14001602d:	add    %al,(%rax)
    14001602f:	add    %al,(%rax)
    140016031:	add    %al,(%rax)
-   140016033:	add    %dl,(%rsi,%riz,2)
-   140016036:	rex.WXB
+   140016033:	add    %dl,%ah
+   140016035:	mov    $0x4c,%bh
    140016037:	data16 add %al,(%rax)
    14001603a:	add    %al,(%rax)
    14001603c:	or     $0x90000000,%eax
    140016041:	add    (%rax),%eax
    140016043:	add    %ch,%al
    140016045:	add    %eax,%gs:(%rax)
    140016048:	call   0x1400161a0
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:56 2024
+Time/Date		Tue May 21 15:02:59 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27311,19 +27311,17 @@
    140016000:	push   $0x1400123
    140016005:	add    %al,(%rax)
    140016007:	add    %dh,0x23(%rax)
    14001600a:	add    %eax,0x1(%rax)
    14001600d:	add    %al,(%rax)
    14001600f:	add    %al,(%rax)
    140016011:	add    %al,(%rax)
-   140016013:	add    %ah,(%rax)
-   140016015:	data16 rex.WXB
-   140016017:	data16 add %al,(%rax)
-   14001601a:	add    %al,(%rax)
-   14001601c:	or     $0x90000000,%eax
+   140016013:	add    %ah,0x664cb7(%rbx)
+   140016019:	add    %al,(%rax)
+   14001601b:	add    %cl,-0x70000000(%rip)        # 0xd0016021
    140016021:	add    (%rax),%eax
    140016023:	add    %ch,%al
    140016025:	add    %eax,%gs:(%rax)
    140016028:	call   0x140016182
 	...
    14001607d:	add    %al,(%rax)
    14001607f:	add    %bl,0x1400169(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:44 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28460,16 +28460,16 @@
    1400170ed:	add    %al,(%rax)
    1400170ef:	add    %cl,0x1400133(%rax)
    1400170f5:	add    %al,(%rax)
    1400170f7:	add    %dl,0x1400133(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %al,(%rax)
    140017101:	add    %al,(%rax)
-   140017103:	add    %dl,(%rsi,%riz,2)
-   140017106:	rex.WXB
+   140017103:	add    %dl,%ah
+   140017105:	mov    $0x4c,%bh
    140017107:	data16 add %al,(%rax)
    14001710a:	add    %al,(%rax)
    14001710c:	or     $0x90000000,%eax
    140017111:	add    (%rax),%eax
    140017113:	add    %ch,%ah
    140017115:	jbe    0x140017118
    140017117:	add    %ch,%ah
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:56 2024
+Time/Date		Tue May 21 15:02:59 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28609,19 +28609,17 @@
    1400170cd:	add    %al,(%rax)
    1400170cf:	add    %cl,0x1400133(%rax)
    1400170d5:	add    %al,(%rax)
    1400170d7:	add    %dl,0x1400133(%rax)
    1400170dd:	add    %al,(%rax)
    1400170df:	add    %al,(%rax)
    1400170e1:	add    %al,(%rax)
-   1400170e3:	add    %ah,(%rax)
-   1400170e5:	data16 rex.WXB
-   1400170e7:	data16 add %al,(%rax)
-   1400170ea:	add    %al,(%rax)
-   1400170ec:	or     $0x90000000,%eax
+   1400170e3:	add    %ah,0x664cb7(%rbx)
+   1400170e9:	add    %al,(%rax)
+   1400170eb:	add    %cl,-0x70000000(%rip)        # 0xd00170f1
    1400170f1:	add    (%rax),%eax
    1400170f3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170f7:	add    %ch,0x1(%rsi,%riz,2)
    1400170fb:	add    %al,(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %ah,(%rax)
    140017101:	jp     0x140017104
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:45 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32579,17 +32579,19 @@
    140019325:	add    %al,(%rax)
    140019327:	add    %al,(%rax)
    140019329:	push   %rbp
    14001932a:	add    %eax,0x1(%rax)
    14001932d:	add    %al,(%rax)
    14001932f:	add    %al,(%rax)
    140019331:	add    %al,(%rax)
-   140019333:	add    %dl,0x664b66(%rip)        # 0x14067de9f
-   140019339:	add    %al,(%rax)
-   14001933b:	add    %cl,0x20000000(%rip)        # 0x160019341
+   140019333:	add    %dl,%ah
+   140019335:	mov    $0x4c,%bh
+   140019337:	data16 add %al,(%rax)
+   14001933a:	add    %al,(%rax)
+   14001933c:	or     $0x20000000,%eax
    140019341:	add    (%rax),%eax
    140019343:	add    %bh,%ah
    140019345:	movabs %al,0x192fc0001
 	...
    14001937e:	add    %al,(%rax)
    140019380:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 20 15:02:58 2024
+Time/Date		Tue May 21 15:03:00 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32702,17 +32702,15 @@
    140019305:	add    %al,(%rax)
    140019307:	add    %al,(%rax)
    140019309:	push   %rbp
    14001930a:	add    %eax,0x1(%rax)
    14001930d:	add    %al,(%rax)
    14001930f:	add    %al,(%rax)
    140019311:	add    %al,(%rax)
-   140019313:	add    %ah,(%rdx)
-   140019315:	data16 rex.WXB
-   140019317:	data16 add %al,(%rax)
+   140019313:	add    %ah,0x664c(%rdi,%rsi,4)
    14001931a:	add    %al,(%rax)
    14001931c:	or     $0x20000000,%eax
    140019321:	add    (%rax),%eax
    140019323:	add    %bh,%ah
    140019325:	movabs %al,0x194fc0001
 	...
    14001937e:	add    %al,(%rax)
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:44 2024
+Time/Date		Tue May 21 15:03:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,16 +4028,16 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	adc    $0x66,%al
-   180004606:	rex.WXB
+   180004604:	(bad)
+   180004605:	mov    $0x4c,%bh
    180004607:	data16 add %al,(%rax)
    18000460a:	add    %al,(%rax)
    18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063388
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May 20 15:02:45 2024
+Time/Date		Tue May 21 15:03:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063a00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063388
@@ -133095,15 +133095,15 @@
    18006cd77:	add    %al,%al
    18006cd79:	push   %rsi
    18006cd7a:	(bad)
    18006cd7b:	addb   $0x0,(%rcx)
    18006cd7e:	add    %al,(%rax)
    18006cd80:	add    %al,(%rax)
    18006cd82:	add    %al,(%rax)
-   18006cd84:	adc    $0x664b66,%eax
+   18006cd84:	{rex2 0xb7} cmovl 0x0(%r30),%r12d
    18006cd89:	add    %al,(%rax)
    18006cd8b:	add    %cl,0x50000000(%rip)        # 0x1d006cd91
    18006cd91:	add    (%rax),%eax
    18006cd93:	add    %dl,-0x21(%rax)
    18006cd96:	(bad)
    18006cd97:	add    %dl,-0x33(%rax)
    18006cd9a:	(bad)
```

## ipex_llm/transformers/convert.py

```diff
@@ -713,14 +713,18 @@
         model.apply(split_mlp)
     # for baichuan2
     if model.config.model_type == "baichuan" and model.config.vocab_size == 125696:
         if model.config.hidden_size in [4096, 2048]:
             # baichuan2-7B
             from ipex_llm.transformers.models.baichuan2 import pre_compute_inv_freq
             model.apply(pre_compute_inv_freq)
+    # for qwen2
+    if model.config.model_type == "qwen2":
+        from ipex_llm.transformers.models.qwen2 import merge_qkv
+        model.apply(merge_qkv)
     if model.config.model_type == "stablelm":
         # For stablelm-zephyr-3b and stablelm-2-zephyr-1_6b
         from ipex_llm.transformers.models.stablelm import merge_qkv
         model.apply(merge_qkv)
 
     return model
```

## ipex_llm/transformers/models/qwen2.py

```diff
@@ -38,84 +38,52 @@
 #
 
 import math
 import warnings
 from typing import TYPE_CHECKING, Optional, Tuple, Union, Callable, List
 
 import torch
-import torch.nn as nn
-import torch.nn.functional as F
+from torch.nn.functional import scaled_dot_product_attention as sdpa
 
-from ipex_llm.transformers.models.llama import repeat_kv
-from ipex_llm.transformers.models.utils import extend_kv_cache, append_kv_cache
+from ipex_llm.transformers.models.utils import should_use_fuse_rope
 from ipex_llm.transformers.models.utils import use_quantize_kv_cache, restore_fp8_kv_cache
-from ipex_llm.transformers.models.utils import is_enough_kv_cache_room_4_36
-from ipex_llm.transformers.models.utils import apply_rotary_pos_emb_cache_freq_xpu
-from ipex_llm.transformers.kv import DynamicFp8Cache
+from ipex_llm.transformers.models.utils import use_flash_attention, use_sdp, use_sdp_causal
+from ipex_llm.transformers.kv import DynamicFp8Cache, DynamicNormalCache
 from ipex_llm.utils.common import invalidInputError
-from ipex_llm.transformers.models.utils import use_flash_attention, use_sdp
-from transformers.models.qwen2.modeling_qwen2 import Qwen2Model, apply_rotary_pos_emb
+
+from transformers.models.qwen2.modeling_qwen2 import Qwen2Attention, apply_rotary_pos_emb, repeat_kv
 from transformers.models.qwen2.modeling_qwen2 import _prepare_4d_causal_attention_mask_for_sdpa
 from transformers.models.qwen2.modeling_qwen2 import _prepare_4d_causal_attention_mask
 from transformers.modeling_outputs import BaseModelOutputWithPast
-from ipex_llm.transformers.models.utils import use_decoding_fast_path
-
-try:
-    from transformers.cache_utils import Cache, DynamicCache
-except ImportError:
-    Cache = Tuple[torch.Tensor]
-import logging
+from transformers.cache_utils import Cache, DynamicCache
 from transformers import logging
 
 
 logger = logging.get_logger(__name__)
 
-import os
-
-KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
-
-
-def should_split_qkv_tensor(query_states, bsz, num_heads, q_len, kv_seq_len, output_attentions):
-    if not output_attentions:
-        if os.environ.get("IPEX_LLM_SPLIT_QKV", None) is not None:
-            return os.environ.get("IPEX_LLM_SPLIT_QKV", None) == "1"
-        elif query_states.dtype == torch.float16 and \
-                query_states.shape[2] >= 5000:
-            # split tensor for memory block limitation
-            # support fp16 and set input length threshold at 5000 for now
-            return True
-        elif query_states.element_size()*bsz*num_heads*q_len*kv_seq_len >= 4*1024**3:
-            # attn_weight size larger than memory block limitation 4GB
-            return True
-    return False
-
-
-def should_use_fuse_rope(self, query_states, position_ids):
-    use_fuse_rope = query_states.device.type == "xpu"
-    use_fuse_rope = use_fuse_rope and not (self.training and query_states.requires_grad)
-    use_fuse_rope = use_fuse_rope and position_ids is not None
-    return use_fuse_rope
-
 
 def qwen2_model_forward(
     self,
     input_ids: torch.LongTensor = None,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
     past_key_values: Optional[List[torch.FloatTensor]] = None,
     inputs_embeds: Optional[torch.FloatTensor] = None,
     use_cache: Optional[bool] = None,
     output_attentions: Optional[bool] = None,
     output_hidden_states: Optional[bool] = None,
     return_dict: Optional[bool] = None,
 ):
     use_cache = use_cache if use_cache is not None else self.config.use_cache
-    if use_cache and use_quantize_kv_cache(self.layers[0].mlp.up_proj, input_ids):
-        if not isinstance(past_key_values, DynamicFp8Cache):
+    use_quantize_kv = use_quantize_kv_cache(self.layers[0].mlp.up_proj, input_ids)
+    if use_cache:
+        if use_quantize_kv and not isinstance(past_key_values, DynamicFp8Cache):
             past_key_values = DynamicFp8Cache.from_legacy_cache(past_key_values)
+        if not use_quantize_kv and not isinstance(past_key_values, DynamicNormalCache):
+            past_key_values = DynamicNormalCache.from_legacy_cache(past_key_values)
     return qwen2_model_forward_internal(
         self=self,
         input_ids=input_ids,
         attention_mask=attention_mask,
         position_ids=position_ids,
         past_key_values=past_key_values,
         inputs_embeds=inputs_embeds,
@@ -244,21 +212,21 @@
                 attention_mask,
                 position_ids,
                 past_key_values,
                 output_attentions,
                 use_cache,
             )
         else:
-            # bigdl-llm changes
+            # ipex-llm changes
             curr_device = decoder_layer.input_layernorm.weight.device
             if attention_mask is not None:
                 attention_mask = attention_mask.to(curr_device)
             if position_ids is not None:
                 position_ids = position_ids.to(curr_device)
-            # bigdl-llm changes end
+            # ipex-llm changes end
             layer_outputs = decoder_layer(
                 hidden_states,
                 attention_mask=attention_mask,
                 position_ids=position_ids,
                 past_key_value=past_key_values,
                 output_attentions=output_attentions,
                 use_cache=use_cache,
@@ -290,514 +258,121 @@
         last_hidden_state=hidden_states,
         past_key_values=next_cache,
         hidden_states=all_hidden_states,
         attentions=all_self_attns,
     )
 
 
-def qwen2_attention_forward(
-    self,
-    hidden_states: torch.Tensor,
-    attention_mask: Optional[torch.Tensor] = None,
-    position_ids: Optional[torch.LongTensor] = None,
-    past_key_value: Optional[Tuple[torch.Tensor]] = None,
-    output_attentions: bool = False,
-    use_cache: bool = False,
-    **kwargs,
-) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
-    if use_quantize_kv_cache(self.q_proj, hidden_states):
-        forward_function = qwen2_attention_forward_quantized
-    elif hidden_states.device.type == "cpu":
-        forward_function = qwen2_sdpa_attention_forward
-    else:
-        forward_function = qwen2_attention_forward_origin
-    return forward_function(
-        self=self,
-        hidden_states=hidden_states,
-        attention_mask=attention_mask,
-        position_ids=position_ids,
-        past_key_value=past_key_value,
-        output_attentions=output_attentions,
-        use_cache=use_cache,
-        **kwargs,
-    )
+def merge_qkv(module: torch.nn.Module):
+    if isinstance(module, Qwen2Attention):
+        new_weight = torch.cat([
+            module.q_proj.weight.data,
+            module.k_proj.weight.data,
+            module.v_proj.weight.data,
+        ], dim=0)
+        new_bias = torch.cat([
+            module.q_proj.bias.data,
+            module.k_proj.bias.data,
+            module.v_proj.bias.data,
+        ], dim=-1)
+
+        qkv_proj = torch.nn.Linear(0, 0, bias=True)
+        qkv_proj.weight = torch.nn.Parameter(new_weight, requires_grad=False)
+        qkv_proj.bias = torch.nn.Parameter(new_bias, requires_grad=False)
+        qkv_proj.in_features = new_weight.size(1)
+        qkv_proj.out_features = new_weight.size(0)
+        module.qkv_proj = qkv_proj
+
+        del module.q_proj, module.k_proj, module.v_proj
 
 
-def qwen2_attention_forward_quantized(
+def qwen2_attention_forward(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
-    past_key_value: Optional[DynamicFp8Cache] = None,
+    past_key_value: Optional[Cache] = None,
     output_attentions: bool = False,
     use_cache: bool = False,
     **kwargs,
 ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
-    if "padding_mask" in kwargs:
-        warnings.warn(
-            "Passing `padding_mask` is deprecated and will be removed in v4.37. "
-            "Please make sure use `attention_mask` instead.`"
-        )
-    use_fuse_rope = should_use_fuse_rope(self, hidden_states, position_ids)
     bsz, q_len, _ = hidden_states.size()
+    device = hidden_states.device
 
-    query_states = self.q_proj(hidden_states)
-    key_states = self.k_proj(hidden_states)
-    value_states = self.v_proj(hidden_states)
-
-    query_states = query_states.view(bsz, q_len,
-                                     self.num_heads, self.head_dim).transpose(1, 2)
-    key_states = key_states.view(bsz, q_len,
-                                 self.num_key_value_heads, self.head_dim).transpose(1, 2)
-    value_states = value_states.view(bsz, q_len,
-                                     self.num_key_value_heads, self.head_dim).transpose(1, 2)
+    qkv = self.qkv_proj(hidden_states)
+    qkv = qkv.view(bsz, q_len, self.num_heads + 2 * self.num_key_value_heads, self.head_dim)
+    qkv = qkv.transpose(1, 2)
+    query_states, key_states, value_states = qkv.split([self.num_heads,
+                                                        self.num_key_value_heads,
+                                                        self.num_key_value_heads], dim=1)
 
     kv_seq_len = key_states.shape[-2]
     if past_key_value is not None:
-        invalidInputError(self.layer_idx is not None,
-                          "The cache structure has changed since version v4.36. "
-                          f"If you are using {self.__class__.__name__} "
-                          "for auto-regressive decoding with k/v caching, "
-                          "please make sure to initialize the attention class "
-                          "with a layer index.")
         kv_seq_len += past_key_value.get_usable_length(kv_seq_len, self.layer_idx)
-    cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
 
-    if use_fuse_rope:
-        query_states, key_states = apply_rotary_pos_emb_cache_freq_xpu(query_states, key_states,
-                                                                       sin, cos, "qwen2",
-                                                                       position_ids)
+    if should_use_fuse_rope(hidden_states, position_ids, self.training):
+        import linear_q4_0
+        linear_q4_0.rotary_half_inplaced(self.rotary_emb.inv_freq, position_ids,
+                                         query_states, key_states)
     else:
+        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
         query_states, key_states = apply_rotary_pos_emb(query_states, key_states,
                                                         cos, sin, position_ids)
 
     if past_key_value is not None:
-        cache_kwargs = {"sin": sin, "cos": cos}  # Specific to RoPE models
         key_states, value_states = past_key_value.update(key_states, value_states,
-                                                         self.layer_idx, cache_kwargs)
+                                                         self.layer_idx, None)
 
-    if q_len == 1 and query_states.device.type == 'xpu' and not self.training \
-            and not hidden_states.requires_grad:
+    attn_weights = None
+    if query_states.device.type == "cpu":
+        attn_output = sdpa(query_states,
+                           key_states,
+                           value_states,
+                           attn_mask=attention_mask,
+                           dropout_p=self.attention_dropout if self.training else 0.0,
+                           is_causal=self.is_causal and attention_mask is None and q_len > 1)
+    elif not self.training and not hidden_states.requires_grad and \
+            use_flash_attention(query_states, key_states, attention_mask):
+        attn_output = sdpa(query_states.to(device, dtype=torch.float16),
+                           key_states.to(device, dtype=torch.float16),
+                           value_states.to(device, dtype=torch.float16),
+                           is_causal=True).to(hidden_states.dtype)
+    elif use_sdp(q_len, kv_seq_len, self.head_dim, query_states):
         import linear_q4_0
-        attn_output = linear_q4_0.sdp_fp8(query_states, key_states, value_states,
-                                          attention_mask)
-        attn_weights = None
-    else:
-        key, value = restore_fp8_kv_cache(key_states, value_states, query_states.dtype)
-        key = repeat_kv(key, self.num_key_value_groups)
-        value = repeat_kv(value, self.num_key_value_groups)
-        if should_split_qkv_tensor(query_states, bsz, self.num_heads,
-                                   q_len, kv_seq_len, output_attentions):
-            attn_output, attn_weights = native_sdp_split_qkv_tensor(query_states, key,
-                                                                    value, attention_mask,
-                                                                    bsz, q_len, kv_seq_len,
-                                                                    self.head_dim, self.num_heads,
-                                                                    self.attention_dropout,
-                                                                    self.training)
+        if isinstance(past_key_value, DynamicFp8Cache):
+            attn_output = linear_q4_0.sdp_fp8(query_states, key_states, value_states,
+                                              attention_mask)
         else:
-            attn_weights = torch.matmul(query_states, key.transpose(2, 3))
-            attn_weights = attn_weights / math.sqrt(self.head_dim)
-
-            invalidInputError(attn_weights.size() == (bsz, self.num_heads, q_len, kv_seq_len),
-                              ("Attention weights should be of size "
-                               f"{(bsz, self.num_heads, q_len, kv_seq_len)},"
-                               "but is {attn_weights.size()}"))
-
-            if attention_mask is not None:
-                invalidInputError(attention_mask.size() == (bsz, 1, q_len, kv_seq_len),
-                                  (f"Attention mask should be of size "
-                                   f"{(bsz, 1, q_len, kv_seq_len)},"
-                                   f" but is {attention_mask.size()}"))
-
-                attn_weights = attn_weights + attention_mask
-
-            if kv_seq_len >= 2048 or bsz >= 64:
-                # for memory considerations, do not upcast attention to fp32
-                # for long sequences or large batches
-                attn_weights = nn.functional.softmax(attn_weights, dim=-1)
-            else:
-                # upcast attention to fp32
-                attn_weights = nn.functional.softmax(attn_weights, dim=-1,
-                                                     dtype=torch.float32).to(query_states.dtype)
-            attn_weights = nn.functional.dropout(attn_weights, p=self.attention_dropout,
-                                                 training=self.training)
-
-            attn_output = torch.matmul(attn_weights, value)
-
-    invalidInputError(attn_output.size() == (bsz, self.num_heads, q_len, self.head_dim),
-                      "`attn_output` should be of size "
-                      f"{(bsz, self.num_heads, q_len, self.head_dim)},"
-                      f" but is {attn_output.size()}")
-
-    attn_output = attn_output.transpose(1, 2).contiguous()
-    attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
-
-    attn_output = self.o_proj(attn_output)
-
-    if not output_attentions:
-        attn_weights = None
-
-    return attn_output, attn_weights, past_key_value
-from ipex_llm.ggml.quantize import ggml_tensor_qtype
-SYM_INT4 = ggml_tensor_qtype["sym_int4"]
-FP8E5 = ggml_tensor_qtype["fp8_e5m2"]
-
-
-def qwen2_attention_forward_origin(
-    self,
-    hidden_states: torch.Tensor,
-    attention_mask: Optional[torch.Tensor] = None,
-    position_ids: Optional[torch.LongTensor] = None,
-    past_key_value: Optional[Tuple[torch.Tensor]] = None,
-    output_attentions: bool = False,
-    use_cache: bool = False,
-    **kwargs,
-) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
-
-    use_fuse_rope = should_use_fuse_rope(self, hidden_states, position_ids)
-
-    if "padding_mask" in kwargs:
-        warnings.warn(
-            "Passing `padding_mask` is deprecated and will be removed in v4.37. "
-            "Please make sure use `attention_mask` instead.`"
-        )
-    bsz, q_len, _ = hidden_states.size()
-    device = hidden_states.device
-
-    enough_kv_room = is_enough_kv_cache_room_4_36(past_key_value, self.layer_idx)
-    decoding_fast_path = use_decoding_fast_path(self.q_proj,
-                                                use_fuse_rope,
-                                                enough_kv_room,
-                                                bsz * q_len)
-    if decoding_fast_path:
-        hidden_states = hidden_states.view(1, -1)
-        cache_k = past_key_value.key_cache[self.layer_idx]
-        cache_v = past_key_value.value_cache[self.layer_idx]
-        kv_seq_len = cache_k.shape[-2]
+            attn_output = linear_q4_0.sdp(query_states, key_states, value_states, attention_mask)
+    elif use_sdp_causal(q_len, kv_seq_len, self.head_dim, query_states, self.training):
         import linear_q4_0
-        args = [hidden_states, self.q_proj.weight, self.k_proj.weight, self.v_proj.weight,
-                self.q_proj.bias, self.k_proj.bias, self.v_proj.bias, position_ids, cache_k,
-                cache_v, self.q_proj.weight.qtype, self.v_proj.weight.qtype, kv_seq_len,
-                self.head_dim, self.rotary_emb.base]
-        query_states, key_states, value_states = linear_q4_0.forward_qkv_bias(*args)
-        kv_seq_len += 1
-        if self.layer_idx == 0:
-            past_key_value.seen_tokens = kv_seq_len
-        past_key_value.key_cache[self.layer_idx] = key_states
-        past_key_value.value_cache[self.layer_idx] = value_states
-
-    else:
-
-        query_states = self.q_proj(hidden_states)
-        key_states = self.k_proj(hidden_states)
-        value_states = self.v_proj(hidden_states)
-
-        query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-        key_states = \
-            key_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
-        value_states = \
-            value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
-
-        kv_seq_len = key_states.shape[-2]
-        if past_key_value is not None:
-            if self.layer_idx is None:
-                invalidInputError(
-                    False,
-                    "The cache structure has changed since version v4.36. "
-                    f"If you are using {self.__class__.__name__} "
-                    "for auto-regressive decoding with k/v caching, "
-                    "please make sure to initialize the attention class with a layer index."
-                )
-            kv_seq_len += past_key_value.get_usable_length(kv_seq_len, self.layer_idx)
-        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
-        if use_fuse_rope:
-            query_states, key_states = apply_rotary_pos_emb_cache_freq_xpu(query_states, key_states,
-                                                                           sin, cos, "qwen2",
-                                                                           position_ids)
+        if isinstance(past_key_value, DynamicFp8Cache):
+            attn_output = linear_q4_0.sdp_fp8_causal(query_states, key_states, value_states)
         else:
-            query_states, key_states = apply_rotary_pos_emb(query_states, key_states,
-                                                            cos, sin, position_ids)
-
-        if past_key_value is not None:
-            # update the number of seen tokens
-            if self.layer_idx == 0:
-                past_key_value.seen_tokens += key_states.shape[-2]
-
-            if len(past_key_value.key_cache) <= self.layer_idx:
-                past_key_value.key_cache.append(key_states)
-                past_key_value.value_cache.append(value_states)
-            else:
-                cache_k = past_key_value.key_cache[self.layer_idx]
-                cache_v = past_key_value.value_cache[self.layer_idx]
-
-                if not enough_kv_room:
-                    # allocate new
-                    new_c_k, new_c_v = extend_kv_cache(bsz,
-                                                       self.num_key_value_heads,  # Support GQA
-                                                       self.head_dim,
-                                                       cache_k.size(2),
-                                                       kv_seq_len + KV_CACHE_ALLOC_BLOCK_LENGTH,
-                                                       dtype=cache_k.dtype,
-                                                       device=device)
-
-                    new_c_k[:] = cache_k
-                    new_c_v[:] = cache_v
-                    cache_k = new_c_k
-                    cache_v = new_c_v
-
-                key_states, value_states = append_kv_cache(cache_k,
-                                                           cache_v,
-                                                           key_states,
-                                                           value_states)
-
-                # update past_key_value
-                past_key_value.key_cache[self.layer_idx] = key_states
-                past_key_value.value_cache[self.layer_idx] = value_states
-
-    # repeat k/v heads if n_kv_heads < n_heads
-    key_states = repeat_kv(key_states, self.num_key_value_groups)
-    value_states = repeat_kv(value_states, self.num_key_value_groups)
-
-    if not self.training and not hidden_states.requires_grad and \
-            use_flash_attention(query_states, key_states, attention_mask):
-        attn_output = F.scaled_dot_product_attention(query_states.to(device, dtype=torch.float16),
-                                                     key_states.to(device, dtype=torch.float16),
-                                                     value_states.to(device, dtype=torch.float16),
-                                                     is_causal=True)
-        attn_weights = None
-    elif not self.training and not hidden_states.requires_grad and \
-            use_sdp(q_len, key_states.shape[2], self.head_dim, query_states):
-        import linear_q4_0
-        attn_output = linear_q4_0.sdp(query_states, key_states, value_states, attention_mask)
-        attn_output = attn_output.view(query_states.shape)
-        attn_weights = None
+            attn_output = linear_q4_0.sdp_causal(query_states, key_states, value_states)
     else:
-        if should_split_qkv_tensor(query_states, bsz, self.num_heads,
-                                   q_len, kv_seq_len, output_attentions):
-            attn_output, attn_weights = native_sdp_split_qkv_tensor(query_states, key_states,
-                                                                    value_states, attention_mask,
-                                                                    bsz, q_len, kv_seq_len,
-                                                                    self.head_dim, self.num_heads,
-                                                                    self.attention_dropout,
-                                                                    self.training)
-        else:
-            attn_weights = torch.matmul(query_states,
-                                        key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
-
-            invalidInputError(attn_weights.size() == (bsz, self.num_heads, q_len, kv_seq_len),
-                              ("Attention weights should be of size "
-                               f"{(bsz, self.num_heads, q_len, kv_seq_len)},"
-                               "but is {attn_weights.size()}"))
+        if isinstance(past_key_value, DynamicFp8Cache):
+            key_states, value_states = restore_fp8_kv_cache(key_states, value_states,
+                                                            query_states.dtype)
+        # repeat k/v heads if n_kv_heads < n_heads
+        key_states = repeat_kv(key_states, self.num_key_value_groups)
+        value_states = repeat_kv(value_states, self.num_key_value_groups)
 
-            if attention_mask is not None:
-                invalidInputError(attention_mask.size() == (bsz, 1, q_len, kv_seq_len),
-                                  (f"Attention mask should be of size "
-                                   f"{(bsz, 1, q_len, kv_seq_len)},"
-                                   f" but is {attention_mask.size()}"))
-
-                attn_weights = attn_weights + attention_mask
-
-            if kv_seq_len >= 2048 or bsz >= 64:
-                # for memory considerations, do not upcast attention to fp32
-                # for long sequences or large batches
-                attn_weights = nn.functional.softmax(attn_weights, dim=-1)
-            else:
-                # upcast attention to fp32
-                attn_weights = nn.functional.softmax(attn_weights, dim=-1,
-                                                     dtype=torch.float32).to(query_states.dtype)
-            attn_weights = nn.functional.dropout(attn_weights,
-                                                 p=self.attention_dropout,
-                                                 training=self.training)
-            attn_output = torch.matmul(attn_weights, value_states)
-
-    invalidInputError(attn_output.size() == (bsz, self.num_heads, q_len, self.head_dim),
-                      "`attn_output` should be of size "
-                      f"{(bsz, self.num_heads, q_len, self.head_dim)},"
-                      f" but is {attn_output.size()}")
+        attn_weights = torch.matmul(query_states,
+                                    key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
+        if attention_mask is not None:
+            attn_weights = attn_weights + attention_mask
+        # upcast attention to fp32
+        attn_weights = torch.nn.functional.softmax(attn_weights, dim=-1,
+                                                   dtype=torch.float32).to(query_states.dtype)
+        attn_weights = torch.nn.functional.dropout(attn_weights, p=self.attention_dropout,
+                                                   training=self.training)
+        attn_output = torch.matmul(attn_weights, value_states)
 
     attn_output = attn_output.transpose(1, 2).contiguous()
     attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
 
     attn_output = self.o_proj(attn_output)
 
     if not output_attentions:
         attn_weights = None
-
-    return attn_output.to(hidden_states.dtype), attn_weights, past_key_value
-
-
-def qwen2_sdpa_attention_forward(
-    self,
-    hidden_states: torch.Tensor,
-    attention_mask: Optional[torch.Tensor] = None,
-    position_ids: Optional[torch.LongTensor] = None,
-    past_key_value: Optional[Tuple[torch.Tensor]] = None,
-    output_attentions: bool = False,
-    use_cache: bool = False,
-    **kwargs,
-) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
-
-    use_fuse_rope = should_use_fuse_rope(self, hidden_states, position_ids)
-
-    if "padding_mask" in kwargs:
-        warnings.warn(
-            "Passing `padding_mask` is deprecated and will be removed in v4.37. "
-            "Please make sure use `attention_mask` instead.`"
-        )
-    bsz, q_len, _ = hidden_states.size()
-    device = hidden_states.device
-
-    enough_kv_room = is_enough_kv_cache_room_4_36(past_key_value, self.layer_idx)
-    decoding_fast_path = use_decoding_fast_path(self.q_proj,
-                                                use_fuse_rope,
-                                                enough_kv_room,
-                                                bsz * q_len)
-    if decoding_fast_path:
-        hidden_states = hidden_states.view(1, -1)
-        cache_k = past_key_value.key_cache[self.layer_idx]
-        cache_v = past_key_value.value_cache[self.layer_idx]
-        kv_seq_len = cache_k.shape[-2]
-        import linear_q4_0
-        args = [hidden_states, self.q_proj.weight, self.k_proj.weight, self.v_proj.weight,
-                self.q_proj.bias, self.k_proj.bias, self.v_proj.bias, position_ids, cache_k,
-                cache_v, self.q_proj.weight.qtype, self.v_proj.weight.qtype, kv_seq_len,
-                self.head_dim, self.rotary_emb.base]
-        query_states, key_states, value_states = linear_q4_0.forward_qkv_bias(*args)
-        kv_seq_len += 1
-        if self.layer_idx == 0:
-            past_key_value.seen_tokens = kv_seq_len
-        past_key_value.key_cache[self.layer_idx] = key_states
-        past_key_value.value_cache[self.layer_idx] = value_states
-
-    else:
-
-        query_states = self.q_proj(hidden_states)
-        key_states = self.k_proj(hidden_states)
-        value_states = self.v_proj(hidden_states)
-
-        query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-        key_states = \
-            key_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
-        value_states = \
-            value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
-
-        kv_seq_len = key_states.shape[-2]
-        if past_key_value is not None:
-            if self.layer_idx is None:
-                invalidInputError(
-                    False,
-                    "The cache structure has changed since version v4.36. "
-                    f"If you are using {self.__class__.__name__} "
-                    "for auto-regressive decoding with k/v caching, "
-                    "please make sure to initialize the attention class with a layer index."
-                )
-            kv_seq_len += past_key_value.get_usable_length(kv_seq_len, self.layer_idx)
-        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
-        if use_fuse_rope:
-            query_states, key_states = apply_rotary_pos_emb_cache_freq_xpu(query_states, key_states,
-                                                                           sin, cos, "qwen2",
-                                                                           position_ids)
-        else:
-            query_states, key_states = apply_rotary_pos_emb(query_states, key_states,
-                                                            cos, sin, position_ids)
-
-        if past_key_value is not None:
-            # update the number of seen tokens
-            if self.layer_idx == 0:
-                past_key_value.seen_tokens += key_states.shape[-2]
-
-            if len(past_key_value.key_cache) <= self.layer_idx:
-                past_key_value.key_cache.append(key_states)
-                past_key_value.value_cache.append(value_states)
-            else:
-                cache_k = past_key_value.key_cache[self.layer_idx]
-                cache_v = past_key_value.value_cache[self.layer_idx]
-
-                if not enough_kv_room:
-                    # allocate new
-                    new_c_k, new_c_v = extend_kv_cache(bsz,
-                                                       self.num_key_value_heads,  # Support GQA
-                                                       self.head_dim,
-                                                       cache_k.size(2),
-                                                       kv_seq_len + KV_CACHE_ALLOC_BLOCK_LENGTH,
-                                                       dtype=cache_k.dtype,
-                                                       device=device)
-
-                    new_c_k[:] = cache_k
-                    new_c_v[:] = cache_v
-                    cache_k = new_c_k
-                    cache_v = new_c_v
-
-                key_states, value_states = append_kv_cache(cache_k,
-                                                           cache_v,
-                                                           key_states,
-                                                           value_states)
-
-                # update past_key_value
-                past_key_value.key_cache[self.layer_idx] = key_states
-                past_key_value.value_cache[self.layer_idx] = value_states
-
-    # repeat k/v heads if n_kv_heads < n_heads
-    key_states = repeat_kv(key_states, self.num_key_value_groups)
-    value_states = repeat_kv(value_states, self.num_key_value_groups)
-
-    attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
-
-    invalidInputError(attn_weights.size() == (bsz, self.num_heads, q_len, kv_seq_len),
-                      ("Attention weights should be of size "
-                       f"{(bsz, self.num_heads, q_len, kv_seq_len)},"
-                       "but is {attn_weights.size()}"))
-
-    if attention_mask is not None:
-        invalidInputError(attention_mask.size() == (bsz, 1, q_len, kv_seq_len),
-                          (f"Attention mask should be of size {(bsz, 1, q_len, kv_seq_len)}"
-                           f" but is {attention_mask.size()}"))
-
-        attn_weights = attn_weights + attention_mask
-
-    from torch.nn.functional import scaled_dot_product_attention as sdpa
-    attn_output = sdpa(query_states,
-                       key_states,
-                       value_states,
-                       attn_mask=attention_mask,
-                       dropout_p=self.attention_dropout if self.training else 0.0,
-                       is_causal=self.is_causal and attention_mask is None and q_len > 1)
-
-    attn_output = attn_output.transpose(1, 2).contiguous()
-    attn_output = attn_output.view(bsz, q_len, self.hidden_size)
-
-    attn_output = self.o_proj(attn_output)
-
-    return attn_output, None, past_key_value
-
-
-def native_sdp_split_qkv_tensor(query, key, value, attention_mask,
-                                bsz, q_len, kv_seq_len, head_dim, num_heads,
-                                attention_dropout, training):
-    block_size = 8
-    query_split = torch.split(query, block_size, dim=1)
-    key_split = torch.split(key.transpose(2, 3), block_size, dim=1)
-    value_split = torch.split(value, block_size, dim=1)
-    attn_outputs = []
-    for q, k, v in zip(query_split, key_split, value_split):
-        attn_weights_split = torch.matmul(q, k) / math.sqrt(head_dim)
-        block_actual_size = attn_weights_split.size(1)
-        attn_weights_split_size = (bsz, block_actual_size, q_len, kv_seq_len)
-        if attn_weights_split.size() != attn_weights_split_size:
-            invalidInputError(False,
-                              f"Splitted attention weights should be of size "
-                              f"{attn_weights_split_size}, but is {attn_weights_split.size()}")
-
-        if attention_mask is not None:
-            attn_mask_size = (bsz, 1, q_len, kv_seq_len)
-            if attention_mask.size() != attn_mask_size:
-                invalidInputError(False,
-                                  f"Attention mask should be of size {attn_mask_size}, "
-                                  f"but is {attention_mask.size()}")
-            attn_weights_split = attn_weights_split + attention_mask
-        attn_weights_split = nn.functional.softmax(attn_weights_split, dim=-1)
-        attn_weights_split = nn.functional.dropout(attn_weights_split,
-                                                   p=attention_dropout,
-                                                   training=training)
-        attn_outputs.append(torch.matmul(attn_weights_split, v))
-    attn_output = torch.cat(attn_outputs, dim=1)
-    return attn_output, None
+    return attn_output, attn_weights, past_key_value
```

## ipex_llm/transformers/models/qwen_vl.py

```diff
@@ -29,15 +29,14 @@
 import torch
 import torch.nn.functional as F
 import torch.utils.checkpoint
 from transformers.utils import logging
 from ipex_llm.transformers.models.utils import extend_kv_cache, init_kv_cache, append_kv_cache
 from ipex_llm.transformers.models.utils import rotate_half
 from ipex_llm.transformers.models.utils import use_sdp
-from ipex_llm.transformers.models.utils import use_decoding_fast_path
 
 import os
 
 KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def apply_rotary_pos_emb(t, freqs):
@@ -87,96 +86,55 @@
 
     kv_seq_len = hidden_states.size()[1]
 
     bsz, q_len, _ = hidden_states.size()
     device = hidden_states.device
 
     use_fuse_rope = should_use_fuse_rope(self, hidden_states)
-    decoding_fast_path = use_decoding_fast_path(self.q_proj,
-                                                use_fuse_rope,
-                                                True,
-                                                bsz * q_len)
-    if decoding_fast_path:
-        hidden_states = hidden_states.view(1, -1)
-        cache_k, cache_v = layer_past[0], layer_past[1]
-        cache_k = cache_k.transpose(1, 2)
-        cache_v = cache_v.transpose(1, 2)
-
-        kv_seq_len = cache_k.shape[-2]
-        self.position_ids = self.position_ids.to(device)
-        position_ids = self.position_ids[kv_seq_len]
-        base = self.rope_base
-        if is_enough_kv_cache_room(layer_past, kv_seq_len):
+    mixed_x_layer = self.c_attn(hidden_states)
+    query, key, value = mixed_x_layer.split(self.split_size, dim=2)
+
+    query = self._split_heads(query, self.num_heads, self.head_dim)
+    key = self._split_heads(key, self.num_heads, self.head_dim)
+    value = self._split_heads(value, self.num_heads, self.head_dim)
+    if rotary_pos_emb is not None:
+        cur_len = query.shape[1]
+        rotary_pos_emb = [i[:, -cur_len:, :, :] for i in rotary_pos_emb]
+        rotary_pos_emb = (rotary_pos_emb,) * 2
+        q_pos_emb, k_pos_emb = rotary_pos_emb
+        # Slice the pos emb for current inference
+        query = apply_rotary_pos_emb(query, q_pos_emb)
+        key = apply_rotary_pos_emb(key, k_pos_emb)
+    query_size, key_size = query.size(1), key.size(1)
+
+    if layer_past is not None:
+        kv_seq_len += layer_past[0].shape[1]
+        # past_key, past_value = layer_past[0], layer_past[1]
+        # key = torch.cat((past_key, key), dim=1)
+        # value = torch.cat((past_value, value), dim=1)
+        cache_k = layer_past[0].transpose(1, 2)
+        cache_v = layer_past[1].transpose(1, 2)
+        if cache_k.stride()[1] < kv_seq_len * cache_k.size(3):
+            # allocate new
             new_cache_k, new_cache_v = extend_kv_cache(bsz,
                                                        self.num_heads,
                                                        self.head_dim,
                                                        cache_k.size(2),
                                                        kv_seq_len + KV_CACHE_ALLOC_BLOCK_LENGTH,
                                                        dtype=cache_k.dtype,
                                                        device=hidden_states.device)
             new_cache_k[:] = cache_k
             new_cache_v[:] = cache_v
             cache_k = new_cache_k
             cache_v = new_cache_v
 
-        args = [hidden_states, self.q_proj.weight.data, self.k_proj.weight.data,
-                self.v_proj.weight.data, self.q_proj.bias.data, self.k_proj.bias.data,
-                self.v_proj.bias.data, position_ids, cache_k, cache_v, self.q_proj.weight.qtype,
-                self.v_proj.weight.qtype, kv_seq_len, self.head_dim, base]
-        import linear_q4_0
-        query, key, value = linear_q4_0.forward_qkv_bias(*args)
-        kv_seq_len += 1
-        query_size, key_size = 1, 1
-    else:
-        query = self.q_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim)
-        key = self.k_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim)
-        value = self.v_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim)
-        # TODO: speed up
-        # mixed_x_layer = self.c_attn(hidden_states)
-        # query, key, value = mixed_x_layer.split(self.split_size, dim=2)
-
-        # query = self._split_heads(query, self.num_heads, self.head_dim)
-        # key = self._split_heads(key, self.num_heads, self.head_dim)
-        # value = self._split_heads(value, self.num_heads, self.head_dim)
-        if rotary_pos_emb is not None:
-            cur_len = query.shape[1]
-            rotary_pos_emb = [i[:, -cur_len:, :, :] for i in rotary_pos_emb]
-            rotary_pos_emb = (rotary_pos_emb,) * 2
-            q_pos_emb, k_pos_emb = rotary_pos_emb
-            # Slice the pos emb for current inference
-            query = apply_rotary_pos_emb(query, q_pos_emb)
-            key = apply_rotary_pos_emb(key, k_pos_emb)
-        query_size, key_size = query.size(1), key.size(1)
-
-    if layer_past is not None:
-        if not decoding_fast_path:
-            kv_seq_len += layer_past[0].shape[1]
-            # past_key, past_value = layer_past[0], layer_past[1]
-            # key = torch.cat((past_key, key), dim=1)
-            # value = torch.cat((past_value, value), dim=1)
-            cache_k = layer_past[0].transpose(1, 2)
-            cache_v = layer_past[1].transpose(1, 2)
-            if cache_k.stride()[1] < kv_seq_len * cache_k.size(3):
-                # allocate new
-                new_cache_k, new_cache_v = extend_kv_cache(bsz,
-                                                           self.num_heads,
-                                                           self.head_dim,
-                                                           cache_k.size(2),
-                                                           kv_seq_len + KV_CACHE_ALLOC_BLOCK_LENGTH,
-                                                           dtype=cache_k.dtype,
-                                                           device=hidden_states.device)
-                new_cache_k[:] = cache_k
-                new_cache_v[:] = cache_v
-                cache_k = new_cache_k
-                cache_v = new_cache_v
-
-            key_states, value_states = append_kv_cache(cache_k, cache_v,
-                                                       key.transpose(1, 2), value.transpose(1, 2))
-            key = key_states
-            value = value_states
+        key_states, value_states = append_kv_cache(cache_k, cache_v,
+                                                   key.transpose(1, 2), value.transpose(1, 2))
+        key = key_states
+        value = value_states
     elif use_cache:
         max_cache_length = kv_seq_len + KV_CACHE_ALLOC_BLOCK_LENGTH
         new_key_states, new_value_states = init_kv_cache(bsz,
                                                          self.num_heads,
                                                          self.head_dim,
                                                          kv_seq_len,
                                                          max_cache_length,
@@ -188,18 +146,14 @@
         value = new_value_states
 
     if use_cache:
         present = (key.transpose(1, 2), value.transpose(1, 2))
     else:
         present = None
 
-    if decoding_fast_path:
-        # change to (bsz, q_len, num_heads, head_dim)
-        query = query.transpose(1, 2)
-
     if self.use_logn_attn and not self.training:
         if self.logn_tensor.device != query.device or self.logn_tensor.dtype != query.dtype:
             self.logn_tensor = self.logn_tensor.to(query.device).type_as(query)
         seq_start = key_size - key_size
         seq_end = key_size
         logn_tensor = self.logn_tensor[:, seq_start:seq_end, :, :]
         query = query * logn_tensor.expand_as(query)
```

## Comparing `ipex_llm-2.1.0b20240520.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240521.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240520.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240521.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240520.dist-info/METADATA` & `ipex_llm-2.1.0b20240521.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240520
+Version: 2.1.0b20240521
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Requires-Dist: torch (==2.1.2+cpu) ; (platform_system == "Linux") and extra == 'all'
 Requires-Dist: torch (==2.1.2) ; (platform_system == "Windows") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240520) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240521) ; extra == 'cpp'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
@@ -55,31 +55,31 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240520) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240520) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240521) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240521) ; extra == 'xpu'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240520) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240520) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240521) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240521) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu'
```

## Comparing `ipex_llm-2.1.0b20240520.dist-info/RECORD` & `ipex_llm-2.1.0b20240521.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -38,60 +38,60 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=EUvt0NDtMAJXLYeAxC24GERdORf6Tg6zdFds_rkAkrU,36352
-ipex_llm/libs/bloom.dll,sha256=tTetuiGPoYYs6u7f4Zn-alF96Q_1h0dDenKWDCF7Mfw,473088
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=WtCDrzLHnWqIY7KLKIV6rqx71ebJCX_AQZPmmEIi4E4,854016
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=x8JYBsJOinXFFOtybSqJwrDXzM0X6M1URtUswKEb7A0,856576
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=nBbG0JpPGtfgjSrcXTpCxfnLyqbKFnAUxal5sN-ySk0,844800
-ipex_llm/libs/gptneox-api.dll,sha256=tPMaXhY48R2BiQonQW25w3i2ja01JwkSLGfw-6kob9U,24576
-ipex_llm/libs/gptneox.dll,sha256=s9HnEmvXYJk-3jVqm-vcipnUHWIVEOJQgAuT5-EX4Fo,532992
-ipex_llm/libs/libbloom_avx.dll,sha256=tSm_4efNBiNNKeh9NSBYjhnEUxAgODshK2aXxpn2A68,499712
-ipex_llm/libs/libbloom_vnni.dll,sha256=nVTuguLtiyVVlsNCnlkGUr4MthNkFjah4CK8jI0RgVg,473600
-ipex_llm/libs/libgptneox_avx.dll,sha256=6Rpnp32dp042MK9Xcof186hEo3U63WYY0vfcIGKHAPc,559104
-ipex_llm/libs/libgptneox_vnni.dll,sha256=9vuUbXKh6OlEaz0CsjSV_-GZQ9qLTbgj8UD7B8oT-7g,533504
-ipex_llm/libs/libllama_avx.dll,sha256=oVwT1M1zV0VTkuDHDj6gFX_UeX0IuS__inmwdLD9fhY,553472
-ipex_llm/libs/libllama_vnni.dll,sha256=LbTYCdQXTAx6uIVYhirHC4W7HOE27Y21pnaSsXsLiYo,527872
-ipex_llm/libs/libstarcoder_avx.dll,sha256=Rxwc2YhutLzrlT0YyORCDlexBXZbINrmGYZshkth47k,590848
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=KEZH4UZ1CKnstZEtNSUwKNPW7WEbMpxi4LYLomFkUw0,564736
-ipex_llm/libs/llama-api.dll,sha256=SLJaNYcEgE7wGVT0FZN8RPB-of862HhwJyMEqzjT4BU,25088
-ipex_llm/libs/llama.dll,sha256=3e9E6f934aGGOIe2wsTkjpBxtSHTZ8Z3qJ9C3PsYBrk,526848
-ipex_llm/libs/main-bloom.exe,sha256=lcYNDW15yobaiXDStEkUrWKvqQzXDnSmGDtKBRfvFj0,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=QzXNok8Dl0Xs0Mv-YDMiIaS8WScbbQFe30VazcCCWu0,726528
-ipex_llm/libs/main-gptneox.exe,sha256=nCcYurba3_fv465Xm8Nyq6jk44EAUUjdhBhmgLnx9-g,98816
-ipex_llm/libs/main-llama.exe,sha256=IGDWYhoEz_O5ACDvUSkJYxche7PFVYlt3VnImSnKtGI,99840
-ipex_llm/libs/main-starcoder.exe,sha256=QRQMCulca2UAMwOJBD_BnJIpiEcl5B6kveVmFY6ELpA,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=w3j-1FKRzOvob24lzIfh4uMTvdZ3g9wSSs2ZfxF8_-M,126464
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=JjjNCclzcTh3I-A1SNJIZWV63Gi9C1KIQrsog4xbTdM,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=WuyTBMG2NidARfnscDOWgQ-LzTd-UjwHzCZBXifbbC4,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=SqI9i0u1mfa0WbiAn7JBKDkASeZzYj4smNEzcxpPcqc,104448
-ipex_llm/libs/quantize-llama.exe,sha256=EeR0XU9N6WLlO-7NGEEYDPGBoJH16GtmyVOX6Nd54dc,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=vDur4x2i_Y4muIZy3ZNgvDc2_kxmctAseaxYyN37i7U,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=cr217t0bCQ0AmsXrAolRWPFy1oE-T0Y6SBOQBl54N7k,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=-KfyXkjwQTnYAga4BgF_nAi_93yXLlIZM93Y3hY10Us,128512
-ipex_llm/libs/starcoder-api.dll,sha256=h_ElTdVLTKe30VWumKEndgbFqgolRDQeF-O8gcm_p38,21504
-ipex_llm/libs/starcoder.dll,sha256=LI3R0-e5aJBGolEGj7zY6lD1m60BYFmuqPD_4n2F1qM,564224
+ipex_llm/libs/bloom-api.dll,sha256=m04mt1V_AzL7Hw07_stnCnfPhUq0ADi42VIYEW7Qxyc,36352
+ipex_llm/libs/bloom.dll,sha256=KQ4CPcVrd9JeQmdEft71VZa7pqD6be_l_uaV3JIb6cE,473088
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=5t4AjOPlvi5Ci8H7bLlO6vhl0xk-Y9lmOAepa-9_630,854016
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=8s9peWG2g7_n6Sfr5PxFUBpNHAUJew9xngfSS9s8d-E,856576
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=Php6bRMfDd2q8t9oChw6lHmLDGMHMYI8Fgy020um8oM,844800
+ipex_llm/libs/gptneox-api.dll,sha256=MZSZn2RGXOzL7KGnF7UACvtmHDdEN8-S6TljT0oZ8eQ,24576
+ipex_llm/libs/gptneox.dll,sha256=UHn8S0jrj1CtSKPr2l0alIseevN9BP9BNHXSFZCv4YM,532992
+ipex_llm/libs/libbloom_avx.dll,sha256=IN4x1KT1ylQVXFUeAvZm_30f0P_XHF1GGWdDR9QmqA0,499712
+ipex_llm/libs/libbloom_vnni.dll,sha256=pivN3c228tsqzmVoikl7lKeMUI2lK7YWWFuFDEtoRr0,473600
+ipex_llm/libs/libgptneox_avx.dll,sha256=eBI4mSPAZiM6LFCuN6Tagg86uDs1svuVcSgRYkALnWE,559104
+ipex_llm/libs/libgptneox_vnni.dll,sha256=O4aWVe0aZDnEXFsXP2njJrpkXGYy-upk3y0f1lN_fqw,533504
+ipex_llm/libs/libllama_avx.dll,sha256=69Qs_XLDme-3J2md11BGOveYISCaq5OHSvutg2AyAbQ,553472
+ipex_llm/libs/libllama_vnni.dll,sha256=Lq3nHYOV8HQ9HWkG2_mhT7gwKsJ56HUoCo9pZkbXHQw,527872
+ipex_llm/libs/libstarcoder_avx.dll,sha256=9kePoV-r7XSjBCF5CwHLzYY_TZY0LyvWVcohpDT1auc,590848
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=yYkLW_avjVEIQqdm6UssTMNWUtNB8jGnc9V486rSuu0,564736
+ipex_llm/libs/llama-api.dll,sha256=taKzk0Mhe-l8humy8AdPItuET1Qlc5xORsQqiTGkfEc,25088
+ipex_llm/libs/llama.dll,sha256=wS7CouImbXsPPsSRJndqr-WsVK08sKxrTqZ_mY_hZ8c,526848
+ipex_llm/libs/main-bloom.exe,sha256=pfVomQd03uFqB0jRKDcMiuEQj6kab0drA56-8PzUo-E,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=cwF8gtubdpoIiXdAcuYyaDROr5OuWnW26SEQFHZjtHM,726528
+ipex_llm/libs/main-gptneox.exe,sha256=OgKlw1O2q4PClKlMxfuM-g4dBx54D76PRNoZyNoo4OA,98816
+ipex_llm/libs/main-llama.exe,sha256=a-zhMmHOqEoj_TIUJCeqNyJYGGfYDr6Dz7YuplS8L7M,99840
+ipex_llm/libs/main-starcoder.exe,sha256=RcLitqLB_rIMF0KI69Y1ztxwDYnrHTWlklDVO28WFMQ,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=d1U2KFyDS2551yW33REaZSZd7-grPCF4IeU-_kvABBs,126464
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=F0_Lqg0EDx-aR-h8Qcee2Q6yqYXy53uLlmxAbdYmQ24,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=hbbfNYou5ixjZwcncQUaPL_PLkBH7k6D3SH2RYSC8AE,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=DOVBBngyqPWu4ZLL-bgNjRtjnOwFcYiSqjy-JSmgXKw,104448
+ipex_llm/libs/quantize-llama.exe,sha256=gFy7fMDOY2Svgt7yXiOxLZ2vmHvK9MZpySwuqtYmHTU,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=xdFv_x4LqPWe0nD5ZTl-Vapq6qv9fkPuvyRx5ii3NsE,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=754UAvyZz7_R5Xfn6JEEQsL4lK6A9d50kmhtiurj450,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=G5tOSilsJ7K8Hau_8ZQbTNhrm4o2SEwidbQ5SdQpuLg,128512
+ipex_llm/libs/starcoder-api.dll,sha256=Dn6sYWSpP8m8VipacFWiEyNEewmqv9DeRxO_j0kFFMo,21504
+ipex_llm/libs/starcoder.dll,sha256=dr8XLPKWNj3r6ll5jKSDfcRPy1H1UYS2_OydOiQdzIQ,564224
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=-nDeJIrGneosxjidzcQBMMkByLsRAM8kV70F5v8Kl10,19605
 ipex_llm/serving/fastchat/model_worker.py,sha256=qJSLyWNkP6z70ysq4AV5SqHzXPJJiX2tz7AORB6jEvM,16649
 ipex_llm/serving/fastchat/tgi_api_protocol.py,sha256=brT3k3-V0NJrU4fRqUwWjC0O3iOitdttDfduXXEefh0,5918
 ipex_llm/serving/fastchat/tgi_api_server.py,sha256=2RNVAhd3tH4yH7F7WootcKg9usXaK0OZ6SdTUamrI_I,27062
 ipex_llm/serving/fastchat/vllm_worker.py,sha256=r_2yiI4v69w8teNzh8mZrKMsJ0l6NvWFl8TxEkvq0ug,10801
 ipex_llm/transformers/__init__.py,sha256=8zrY1AGBb2_AeKGDWHY4PCJyzelYA4KwahD54jPoiPg,1005
 ipex_llm/transformers/bmm.py,sha256=BlYrXqeJuw-m136Nf_ST9i6WtZrX6BiTG_psTe1M3Y0,1213
-ipex_llm/transformers/convert.py,sha256=VtVf6V30wbMPP2UyRR81_KdL9zaUQoVb6hWht1Vw-xo,74215
+ipex_llm/transformers/convert.py,sha256=-j-k7pBkW_SH__fsSWTmMX6NhS-BOy-E9Y6566UVc7o,74370
 ipex_llm/transformers/convert_ipex.py,sha256=iKXo0n8fVFTOA2fNYYrByMFK0dovL-kLd2sVDk88AlQ,14334
 ipex_llm/transformers/embedding.py,sha256=f3crD31fEq0pT-d4FV_fS_9uLhgW64BofAxhHSO1QbE,4613
 ipex_llm/transformers/kv.py,sha256=PDdcXWElpiPvzVJQdkkx6Vez0mhROW4K59sngYaX0yY,4247
 ipex_llm/transformers/lisa.py,sha256=F5WxbtXQ7RdKulj83h_2DnEIgKiKGZf7zvOmg6QBl2s,3289
 ipex_llm/transformers/loader.py,sha256=0wMJ9NM0QKRB3AgVRGLmOKcSHYlQ40Rj6UXba513NG0,6812
 ipex_llm/transformers/lookup.py,sha256=OBFFNkuSHP9lK6ePTnNFieKs4_vRs83mECrJj0_XoCU,15562
 ipex_llm/transformers/low_bit_linear.py,sha256=rDaUatzS44m259dtBEFq9KHjZbp121-y6ZhQ6wii7_Y,39885
@@ -152,17 +152,17 @@
 ipex_llm/transformers/models/mistral.py,sha256=wT9ojpt1AisVpAfENDbAVFhCsIqXKOo4CppdwWIb9r0,54855
 ipex_llm/transformers/models/mixtral.py,sha256=dcat_zQLYsQ04Akc1HfZ9AnuzyhjJccPdOR-UiuIcoU,27151
 ipex_llm/transformers/models/mpt.py,sha256=z02NwHogJZVh-Mk4sYoIzR90SFIKhoNN_-ifsD907TQ,9540
 ipex_llm/transformers/models/phi.py,sha256=7TG4NZrQY7L8ONeYv7Rav1-ogFtQl4vd_cl5GndUmcE,7668
 ipex_llm/transformers/models/phi3.py,sha256=PVWI-xKZMWr3qFLs_FTnwvxay4qMcnU-7WK9dvc9450,11908
 ipex_llm/transformers/models/phixtral.py,sha256=4B_2iE26GlzTVdaemd6mwYQ8mp4Yo4Yq9DgSFkF0yvc,6268
 ipex_llm/transformers/models/qwen.py,sha256=jKFrg13JXcGVTYhuh6aescz81xuy7Fw_Qb_ISgA8Iwc,17305
-ipex_llm/transformers/models/qwen2.py,sha256=3QRW9-km30lfyzfNVFIWmy6Gqm6o-dis7wDdUCvGgqs,37312
+ipex_llm/transformers/models/qwen2.py,sha256=LwI20a6e9ikjSgppB4cFqrMV4CYBgTuObQtmzzO6tus,16252
 ipex_llm/transformers/models/qwen2_moe.py,sha256=QQjr5ZMsGg8CUg7hA_WT2ZSEhRRn-vcVLX_pr_foJQk,38469
-ipex_llm/transformers/models/qwen_vl.py,sha256=hU7AKxdlEuFgHFguVH_NmUjkchcQ2UxwDoQPjvuXo4o,11712
+ipex_llm/transformers/models/qwen_vl.py,sha256=CsM0xERvgNgb3tPeuVNgQG1JpYgoSnzeV2QaxgGmcjs,9163
 ipex_llm/transformers/models/rwkv4.py,sha256=Kzu6QlEi0KDXiJrfoZ71TI_D2nju2-sOeaKSZqdJz8U,6135
 ipex_llm/transformers/models/rwkv5.py,sha256=nNtWQROVAUc82SClzHrbaYVsr6CALnlVos0I2TX0YUc,10722
 ipex_llm/transformers/models/stablelm.py,sha256=obstiFzu-QoSEux7Mqfvzv5rQBeHpEaqFMir5dw-hLc,20911
 ipex_llm/transformers/models/starcoder2.py,sha256=mGmsVfjOhezAiB2xmQRwUSb_uvI1ejvQBwTpMcNJRZ8,8805
 ipex_llm/transformers/models/utils.py,sha256=aodLWXGFyLfFn2GeE_LwGC6PQcWAfZDcUsZ6AZRS6is,19883
 ipex_llm/transformers/models/yuan.py,sha256=eRKyROYIPWpn8e9AmIK0V0XiiyWJpj8PekB_pihTfQU,20200
 ipex_llm/utils/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
@@ -179,14 +179,14 @@
 ipex_llm/utils/common/log4Error.py,sha256=8UgIpEJYQasQO4gMOWO22nsOgr14w1emAJy4ts1VOb0,1763
 ipex_llm/vllm/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/ipex_llm_gpu_executor.py,sha256=pY-8XxRRX1_9MTW0TUTidxHmjmXKGsvs1AIIVWU21yM,18514
 ipex_llm/vllm/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
 ipex_llm/vllm/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/engine/engine.py,sha256=mVuCyoTcCX7KnK819-8fL_rNAu05WF_gql6jEcZ9bn8,5941
 ipex_llm/vllm/entrypoints/openai/api_server.py,sha256=luEdC8lW0UZuFx_cWF13Yz7s1wUrvNhHnhAW_rHa1Ps,10564
-ipex_llm-2.1.0b20240520.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240520.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240520.dist-info/METADATA,sha256=VsPCu2UHDQiaZ2aocoEHL-ZKdQDE36bUQaBFOKZ63lU,4965
-ipex_llm-2.1.0b20240520.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240520.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240520.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240520.dist-info/RECORD,,
+ipex_llm-2.1.0b20240521.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240521.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240521.dist-info/METADATA,sha256=_LPlrhirr4Veba4RCWuYuR-RnaYWfZvaMC-ho_ll9KY,4965
+ipex_llm-2.1.0b20240521.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240521.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240521.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240521.dist-info/RECORD,,
```

