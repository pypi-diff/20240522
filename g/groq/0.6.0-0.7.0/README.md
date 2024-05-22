# Comparing `tmp/groq-0.6.0.tar.gz` & `tmp/groq-0.7.0.tar.gz`

## Comparing `groq-0.6.0.tar` & `groq-0.7.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/__init__.py
--rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_base_client.py
--rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_response.py
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_types.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/lib/.keep
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/lib/chat_completion_chunk.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/__init__.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/embeddings.py
--rw-r--r--   0        0        0     9563 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/models.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/audio/__init__.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/audio/audio.py
--rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/audio/transcriptions.py
--rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/audio/translations.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/chat/__init__.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/chat/chat.py
--rw-r--r--   0        0        0    18538 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/chat/completions.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/create_embedding_response.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/embedding.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/embedding_create_params.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/model.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/model_list.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/__init__.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/transcription.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/transcription_create_params.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/transcription_create_response.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/translation.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/translation_create_params.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/translation_create_response.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/chat/__init__.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/chat/chat_completion.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/chat/completion_create_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 groq-0.6.0/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 groq-0.6.0/LICENSE
--rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 groq-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 groq-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/__init__.py
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_base_client.py
+-rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_response.py
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_types.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/lib/.keep
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/lib/chat_completion_chunk.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/__init__.py
+-rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/embeddings.py
+-rw-r--r--   0        0        0     9563 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/models.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/audio/__init__.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/audio/audio.py
+-rw-r--r--   0        0        0    11437 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/audio/transcriptions.py
+-rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/audio/translations.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/chat/chat.py
+-rw-r--r--   0        0        0    31886 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/resources/chat/completions.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/create_embedding_response.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/embedding.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/embedding_create_params.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/model.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/model_list.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/audio/__init__.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/audio/transcription.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/audio/transcription_create_params.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/audio/transcription_create_response.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/audio/translation.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/audio/translation_create_params.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/audio/translation_create_response.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/chat/__init__.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/chat/chat_completion.py
+-rw-r--r--   0        0        0    14239 2020-02-02 00:00:00.000000 groq-0.7.0/src/groq/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 groq-0.7.0/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 groq-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 groq-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 groq-0.7.0/PKG-INFO
```

### Comparing `groq-0.6.0/src/groq/__init__.py` & `groq-0.7.0/src/groq/__init__.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_base_client.py` & `groq-0.7.0/src/groq/_base_client.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_client.py` & `groq-0.7.0/src/groq/_client.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_compat.py` & `groq-0.7.0/src/groq/_compat.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_exceptions.py` & `groq-0.7.0/src/groq/_exceptions.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_files.py` & `groq-0.7.0/src/groq/_files.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_models.py` & `groq-0.7.0/src/groq/_models.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_qs.py` & `groq-0.7.0/src/groq/_qs.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_resource.py` & `groq-0.7.0/src/groq/_resource.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_response.py` & `groq-0.7.0/src/groq/_response.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_streaming.py` & `groq-0.7.0/src/groq/_streaming.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_types.py` & `groq-0.7.0/src/groq/_types.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_utils/__init__.py` & `groq-0.7.0/src/groq/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_utils/_logs.py` & `groq-0.7.0/src/groq/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_utils/_proxy.py` & `groq-0.7.0/src/groq/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_utils/_sync.py` & `groq-0.7.0/src/groq/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_utils/_transform.py` & `groq-0.7.0/src/groq/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_utils/_typing.py` & `groq-0.7.0/src/groq/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/_utils/_utils.py` & `groq-0.7.0/src/groq/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/lib/chat_completion_chunk.py` & `groq-0.7.0/src/groq/lib/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/resources/__init__.py` & `groq-0.7.0/src/groq/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/resources/embeddings.py` & `groq-0.7.0/src/groq/resources/embeddings.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         return EmbeddingsWithStreamingResponse(self)
 
     def create(
         self,
         *,
         input: Union[str, List[str]],
         model: str,
-        dimensions: int | NotGiven = NOT_GIVEN,
         encoding_format: Literal["float", "base64"] | NotGiven = NOT_GIVEN,
         user: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -60,17 +59,15 @@
           input: Input text to embed, encoded as a string or array of tokens. To embed multiple
               inputs in a single request, pass an array of strings or array of token arrays.
               The input must not exceed the max input tokens for the model, cannot be an empty
               string, and any array must be 2048 dimensions or less.
 
           model: ID of the model to use.
 
-          dimensions: The number of dimensions to return the embeddings in.
-
-          encoding_format: The format to return the embeddings in.
+          encoding_format: The format to return the embeddings in. Can only be `float` or `base64`.
 
           user: A unique identifier representing your end-user, which can help us monitor and
               detect abuse.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -81,15 +78,14 @@
         """
         return self._post(
             "/openai/v1/embeddings",
             body=maybe_transform(
                 {
                     "input": input,
                     "model": model,
-                    "dimensions": dimensions,
                     "encoding_format": encoding_format,
                     "user": user,
                 },
                 embedding_create_params.EmbeddingCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -108,15 +104,14 @@
         return AsyncEmbeddingsWithStreamingResponse(self)
 
     async def create(
         self,
         *,
         input: Union[str, List[str]],
         model: str,
-        dimensions: int | NotGiven = NOT_GIVEN,
         encoding_format: Literal["float", "base64"] | NotGiven = NOT_GIVEN,
         user: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -129,17 +124,15 @@
           input: Input text to embed, encoded as a string or array of tokens. To embed multiple
               inputs in a single request, pass an array of strings or array of token arrays.
               The input must not exceed the max input tokens for the model, cannot be an empty
               string, and any array must be 2048 dimensions or less.
 
           model: ID of the model to use.
 
-          dimensions: The number of dimensions to return the embeddings in.
-
-          encoding_format: The format to return the embeddings in.
+          encoding_format: The format to return the embeddings in. Can only be `float` or `base64`.
 
           user: A unique identifier representing your end-user, which can help us monitor and
               detect abuse.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -150,15 +143,14 @@
         """
         return await self._post(
             "/openai/v1/embeddings",
             body=await async_maybe_transform(
                 {
                     "input": input,
                     "model": model,
-                    "dimensions": dimensions,
                     "encoding_format": encoding_format,
                     "user": user,
                 },
                 embedding_create_params.EmbeddingCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
```

### Comparing `groq-0.6.0/src/groq/resources/models.py` & `groq-0.7.0/src/groq/resources/models.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/resources/audio/__init__.py` & `groq-0.7.0/src/groq/resources/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/resources/audio/audio.py` & `groq-0.7.0/src/groq/resources/audio/audio.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/resources/audio/transcriptions.py` & `groq-0.7.0/src/groq/resources/audio/transcriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def create(
         self,
         *,
         file: FileTypes,
         model: Union[str, Literal["whisper-large-v3"]],
         language: str | NotGiven = NOT_GIVEN,
         prompt: str | NotGiven = NOT_GIVEN,
-        response_format: Literal["json", "text", "srt", "verbose_json", "vtt"] | NotGiven = NOT_GIVEN,
+        response_format: Literal["json", "text", "verbose_json"] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
         timestamp_granularities: List[Literal["word", "segment"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -71,16 +71,16 @@
               [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format will
               improve accuracy and latency.
 
           prompt: An optional text to guide the model's style or continue a previous audio
               segment. The [prompt](/docs/guides/speech-to-text/prompting) should match the
               audio language.
 
-          response_format: The format of the transcript output, in one of these options: `json`, `text`,
-              `srt`, `verbose_json`, or `vtt`.
+          response_format: The format of the transcript output, in one of these options: `json`, `text`, or
+              `verbose_json`.
 
           temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the
               output more random, while lower values like 0.2 will make it more focused and
               deterministic. If set to 0, the model will use
               [log probability](https://en.wikipedia.org/wiki/Log_probability) to
               automatically increase the temperature until certain thresholds are hit.
 
@@ -143,15 +143,15 @@
     async def create(
         self,
         *,
         file: FileTypes,
         model: Union[str, Literal["whisper-large-v3"]],
         language: str | NotGiven = NOT_GIVEN,
         prompt: str | NotGiven = NOT_GIVEN,
-        response_format: Literal["json", "text", "srt", "verbose_json", "vtt"] | NotGiven = NOT_GIVEN,
+        response_format: Literal["json", "text", "verbose_json"] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
         timestamp_granularities: List[Literal["word", "segment"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -171,16 +171,16 @@
               [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format will
               improve accuracy and latency.
 
           prompt: An optional text to guide the model's style or continue a previous audio
               segment. The [prompt](/docs/guides/speech-to-text/prompting) should match the
               audio language.
 
-          response_format: The format of the transcript output, in one of these options: `json`, `text`,
-              `srt`, `verbose_json`, or `vtt`.
+          response_format: The format of the transcript output, in one of these options: `json`, `text`, or
+              `verbose_json`.
 
           temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the
               output more random, while lower values like 0.2 will make it more focused and
               deterministic. If set to 0, the model will use
               [log probability](https://en.wikipedia.org/wiki/Log_probability) to
               automatically increase the temperature until certain thresholds are hit.
```

### Comparing `groq-0.6.0/src/groq/resources/audio/translations.py` & `groq-0.7.0/src/groq/resources/audio/translations.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def create(
         self,
         *,
         file: FileTypes,
         model: Union[str, Literal["whisper-large-v3"]],
         prompt: str | NotGiven = NOT_GIVEN,
-        response_format: str | NotGiven = NOT_GIVEN,
+        response_format: Literal["json", "text", "verbose_json"] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
@@ -64,16 +64,16 @@
 
           model: ID of the model to use. Only `whisper-large-v3` is currently available.
 
           prompt: An optional text to guide the model's style or continue a previous audio
               segment. The [prompt](/docs/guides/speech-to-text/prompting) should be in
               English.
 
-          response_format: The format of the transcript output, in one of these options: `json`, `text`,
-              `srt`, `verbose_json`, or `vtt`.
+          response_format: The format of the transcript output, in one of these options: `json`, `text`, or
+              `verbose_json`.
 
           temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the
               output more random, while lower values like 0.2 will make it more focused and
               deterministic. If set to 0, the model will use
               [log probability](https://en.wikipedia.org/wiki/Log_probability) to
               automatically increase the temperature until certain thresholds are hit.
 
@@ -127,15 +127,15 @@
 
     async def create(
         self,
         *,
         file: FileTypes,
         model: Union[str, Literal["whisper-large-v3"]],
         prompt: str | NotGiven = NOT_GIVEN,
-        response_format: str | NotGiven = NOT_GIVEN,
+        response_format: Literal["json", "text", "verbose_json"] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
@@ -149,16 +149,16 @@
 
           model: ID of the model to use. Only `whisper-large-v3` is currently available.
 
           prompt: An optional text to guide the model's style or continue a previous audio
               segment. The [prompt](/docs/guides/speech-to-text/prompting) should be in
               English.
 
-          response_format: The format of the transcript output, in one of these options: `json`, `text`,
-              `srt`, `verbose_json`, or `vtt`.
+          response_format: The format of the transcript output, in one of these options: `json`, `text`, or
+              `verbose_json`.
 
           temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the
               output more random, while lower values like 0.2 will make it more focused and
               deterministic. If set to 0, the model will use
               [log probability](https://en.wikipedia.org/wiki/Log_probability) to
               automatically increase the temperature until certain thresholds are hit.
```

### Comparing `groq-0.6.0/src/groq/resources/chat/__init__.py` & `groq-0.7.0/src/groq/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/resources/chat/chat.py` & `groq-0.7.0/src/groq/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/types/create_embedding_response.py` & `groq-0.7.0/src/groq/types/create_embedding_response.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/types/embedding.py` & `groq-0.7.0/src/groq/types/embedding.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/types/embedding_create_params.py` & `groq-0.7.0/src/groq/types/embedding_create_params.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,15 @@
     of token arrays. The input must not exceed the max input tokens for the model,
     cannot be an empty string, and any array must be 2048 dimensions or less.
     """
 
     model: Required[str]
     """ID of the model to use."""
 
-    dimensions: int
-    """The number of dimensions to return the embeddings in."""
-
     encoding_format: Literal["float", "base64"]
-    """The format to return the embeddings in."""
+    """The format to return the embeddings in. Can only be `float` or `base64`."""
 
     user: Optional[str]
     """
     A unique identifier representing your end-user, which can help us monitor and
     detect abuse.
     """
```

### Comparing `groq-0.6.0/src/groq/types/audio/__init__.py` & `groq-0.7.0/src/groq/types/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/types/audio/transcription_create_params.py` & `groq-0.7.0/src/groq/types/audio/transcription_create_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,18 +32,18 @@
     """An optional text to guide the model's style or continue a previous audio
     segment.
 
     The [prompt](/docs/guides/speech-to-text/prompting) should match the audio
     language.
     """
 
-    response_format: Literal["json", "text", "srt", "verbose_json", "vtt"]
+    response_format: Literal["json", "text", "verbose_json"]
     """
-    The format of the transcript output, in one of these options: `json`, `text`,
-    `srt`, `verbose_json`, or `vtt`.
+    The format of the transcript output, in one of these options: `json`, `text`, or
+    `verbose_json`.
     """
 
     temperature: float
     """The sampling temperature, between 0 and 1.
 
     Higher values like 0.8 will make the output more random, while lower values like
     0.2 will make it more focused and deterministic. If set to 0, the model will use
```

### Comparing `groq-0.6.0/src/groq/types/audio/transcription_create_response.py` & `groq-0.7.0/src/groq/types/audio/transcription_create_response.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/types/audio/translation_create_params.py` & `groq-0.7.0/src/groq/types/audio/translation_create_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     prompt: str
     """An optional text to guide the model's style or continue a previous audio
     segment.
 
     The [prompt](/docs/guides/speech-to-text/prompting) should be in English.
     """
 
-    response_format: str
+    response_format: Literal["json", "text", "verbose_json"]
     """
-    The format of the transcript output, in one of these options: `json`, `text`,
-    `srt`, `verbose_json`, or `vtt`.
+    The format of the transcript output, in one of these options: `json`, `text`, or
+    `verbose_json`.
     """
 
     temperature: float
     """The sampling temperature, between 0 and 1.
 
     Higher values like 0.8 will make the output more random, while lower values like
     0.2 will make it more focused and deterministic. If set to 0, the model will use
```

### Comparing `groq-0.6.0/src/groq/types/audio/translation_create_response.py` & `groq-0.7.0/src/groq/types/audio/translation_create_response.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/src/groq/types/chat/chat_completion.py` & `groq-0.7.0/src/groq/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/LICENSE` & `groq-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `groq-0.6.0/pyproject.toml` & `groq-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "groq"
-version = "0.6.0"
+version = "0.7.0"
 description = "The official Python library for the groq API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Groq", email = "support@groq.com" },
 ]
 dependencies = [
```

### Comparing `groq-0.6.0/PKG-INFO` & `groq-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: groq
-Version: 0.6.0
+Version: 0.7.0
 Summary: The official Python library for the groq API
 Project-URL: Homepage, https://github.com/groq/groq-python
 Project-URL: Repository, https://github.com/groq/groq-python
 Author-email: Groq <support@groq.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

