# Comparing `tmp/cosmian_py_ggml-0.5.0-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/cosmian_py_ggml-1.0.0-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 315713 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 13:34 cosmian_py_ggml.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 13:34 cosmian_py_ggml-0.5.0.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 13:34 cosmian_py_ggml/
--rw-r--r--  2.0 unx     1793 b- defN 23-Jun-19 13:34 cosmian_py_ggml-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx     1064 b- defN 23-Jun-19 13:34 cosmian_py_ggml-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      676 b- defN 23-Jun-19 13:34 cosmian_py_ggml-0.5.0.dist-info/RECORD
--rw-r--r--  2.0 unx      165 b- defN 23-Jun-19 13:34 cosmian_py_ggml-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     4700 b- defN 23-Jun-19 13:34 cosmian_py_ggml/falcon.py
--rw-r--r--  2.0 unx     4681 b- defN 23-Jun-19 13:34 cosmian_py_ggml/gpt_neox.py
--rwxr-xr-x  2.0 unx   809592 b- defN 23-Jun-19 13:34 cosmian_py_ggml/libggml-bindings.so
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-19 13:34 cosmian_py_ggml/__init__.py
-11 files, 822671 bytes uncompressed, 314181 bytes compressed:  61.8%
+Zip file size: 315852 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 14:32 cosmian_py_ggml.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 14:32 cosmian_py_ggml-1.0.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 14:32 cosmian_py_ggml/
+-rw-r--r--  2.0 unx     1689 b- defN 23-Jun-20 14:32 cosmian_py_ggml-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx     1064 b- defN 23-Jun-20 14:32 cosmian_py_ggml-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      678 b- defN 23-Jun-20 14:32 cosmian_py_ggml-1.0.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      165 b- defN 23-Jun-20 14:32 cosmian_py_ggml-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     5068 b- defN 23-Jun-20 14:32 cosmian_py_ggml/falcon.py
+-rw-r--r--  2.0 unx     4989 b- defN 23-Jun-20 14:32 cosmian_py_ggml/gpt_neox.py
+-rwxr-xr-x  2.0 unx   809592 b- defN 23-Jun-20 14:32 cosmian_py_ggml/libggml-bindings.so
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-20 14:32 cosmian_py_ggml/__init__.py
+11 files, 823369 bytes uncompressed, 314320 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -1,26 +1,26 @@
 Filename: cosmian_py_ggml.libs/
 Comment: 
 
-Filename: cosmian_py_ggml-0.5.0.dist-info/
+Filename: cosmian_py_ggml-1.0.0.dist-info/
 Comment: 
 
 Filename: cosmian_py_ggml/
 Comment: 
 
-Filename: cosmian_py_ggml-0.5.0.dist-info/METADATA
+Filename: cosmian_py_ggml-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: cosmian_py_ggml-0.5.0.dist-info/LICENSE
+Filename: cosmian_py_ggml-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: cosmian_py_ggml-0.5.0.dist-info/RECORD
+Filename: cosmian_py_ggml-1.0.0.dist-info/RECORD
 Comment: 
 
-Filename: cosmian_py_ggml-0.5.0.dist-info/WHEEL
+Filename: cosmian_py_ggml-1.0.0.dist-info/WHEEL
 Comment: 
 
 Filename: cosmian_py_ggml/falcon.py
 Comment: 
 
 Filename: cosmian_py_ggml/gpt_neox.py
 Comment:
```

## cosmian_py_ggml/falcon.py

```diff
@@ -1,156 +1,147 @@
 # -*- coding: utf-8 -*-
 import pathlib
 import threading
 import time
-from ctypes import CDLL, POINTER, Structure, c_char_p, c_float, c_int32
+from ctypes import CDLL, POINTER, c_char_p, c_float, c_int32, c_void_p
 from typing import Callable, List, Optional
 
 library_path = pathlib.Path(__file__).parent.resolve() / "libggml-bindings.so"
 clibrary = CDLL(str(library_path))
 
 
-class falcon_model(Structure):
+class FalconModel:
     """
-    Falcon model in GGML backend.
+    Falcon model bindings for GGML.
     """
 
-
-def load_model(model_path: str):
-    """
-    Load the Falcon model from the given model path.
-
-    Args:
-        model_path (str): Path to the model file.
-
-    Returns:
-        POINTER(falcon_model): Pointer to the loaded model.
-    """
-    func = clibrary.falcon_load_model
-    func.argtypes = [c_char_p]
-    func.restype = POINTER(falcon_model)
-
-    return func(model_path.encode("utf-8"))
-
-
-def free_model(model):
-    """
-    Free the memory allocated for the Falcon model.
-
-    Args:
-        model (POINTER(falcon_model)): Pointer to the model.
-
-    Returns:
-        int: Status code indicating success (0) or failure.
-    """
-
-    func = clibrary.falcon_free_model
-    func.argtypes = [POINTER(falcon_model)]
-    func.restype = c_int32
-
-    return func(model)
-
-
-def generate(
-    model,
-    tokens: List[int],
-    n_predict: int = 200,
-    n_threads: int = 6,
-    seed: int = -1,
-    n_batch: int = 8,
-    top_k: int = 40,
-    top_p: float = 0.9,
-    temp: float = 0.9,
-    eos_token: int = 11,
-    stream_callback: Optional[Callable[[List[int]], None]] = None,
-):
-    """
-    Generate tokens using the Falcon model.
-
-    Args:
-        model(POINTER(falcon_model)): The Falcon model.
-        tokens (List[int]): List of input tokens.
-        n_predict (int): Number of tokens to predict. Defaults to 200.
-        n_threads (int, optional): Number of threads to use for processing. Defaults to 6.
-        seed (int, optional): The seed for the random number generator. Defaults to -1.
-        n_batch (int, optional): Batch size for prompt processing. Defaults to 8.
-        top_k (int, optional): Top-k sampling parameter. Defaults to 40.
-        top_p (float, optional): Top-p sampling parameter. Defaults to 0.9.
-        temp (float, optional): Temperature parameter. Defaults to 0.9.
-        stream_callback (Optional[Callable[[List[int]], None]]): Optional callback function to receive generated tokens.
-
-    Returns:
-        List[int]: List of generated tokens.
-    """
-    func = clibrary.falcon_generate
-    func.argtypes = [
-        POINTER(falcon_model),  # model
-        POINTER(c_int32),  # input tokens array
-        c_int32,  # input tokens length
-        POINTER(c_int32),  # output tokens array
-        c_int32,  # n_predict
-        c_int32,  # n_threads
-        c_int32,  # seed
-        c_int32,  # n_batch
-        c_int32,  # top_k
-        c_float,  # top_p
-        c_float,  # temp
-    ]
-
-    # Convert input tokens to a C-compatible array
-    input_tokens_len = len(tokens)
-    input_tokens_arr = (c_int32 * input_tokens_len)()
-    for i in range(input_tokens_len):
-        input_tokens_arr[i] = tokens[i]
-
-    # Create an array for output tokens and initialize with zeros
-    # Add a last end_of_text token (0) at the end
-    output_tokens_len = n_predict + 1
-    output_tokens_arr = (c_int32 * (output_tokens_len))()
-    for i in range(output_tokens_len):
-        output_tokens_arr[i] = eos_token
-
-    # Initialize thread_stop_event if stream_callback is provided
-    thread_stop_event: Optional[threading.Event] = None
-    if stream_callback:
-        thread_stop_event = threading.Event()
-
-        # Define a thread to handle streaming of generated tokens
-        def stream_thread():
-            len = 0
-            while True:
-                time.sleep(0.5)
-                tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
-                curr_len = tokens.index(eos_token)
-                if curr_len > len:
-                    stream_callback(tokens[len:curr_len])
-                    len = curr_len
-
-                if thread_stop_event.is_set():
-                    break
-
-        # Start the stream_thread
-        threading.Thread(target=stream_thread).start()
-
-    # Start tokens generation on GGML backend
-    func(
-        model,
-        input_tokens_arr,
-        input_tokens_len,
-        output_tokens_arr,
-        n_predict,
-        n_threads,
-        seed,
-        n_batch,
-        top_k,
-        top_p,
-        temp,
-    )
-
-    # Stop the stream_thread if it was started
-    if thread_stop_event is not None:
-        time.sleep(1)
-        thread_stop_event.set()
-
-    # Retrieve the generated tokens and return them
-    output_tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
-    return output_tokens[: output_tokens.index(eos_token) + 1]
+    def __init__(self, model_path: str):
+        """
+        Load Falcon model from the given model path.
+
+        Args:
+            model_path (str): Path to the model file.
+
+        Returns:
+            FalconModel: Pointer to the loaded model.
+        """
+        func = clibrary.falcon_load_model
+        func.argtypes = [c_char_p]
+        func.restype = c_void_p
+
+        self.ggml_model = func(model_path.encode("utf-8"))
+
+    def __del__(self):
+        """
+        Free the memory allocated for the model.
+        """
+
+        func = clibrary.falcon_free_model
+        func.argtypes = [c_void_p]
+        func.restype = c_int32
+
+        func(self.ggml_model)
+
+    def __call__(
+        self,
+        tokens: List[int],
+        n_predict: int = 200,
+        n_threads: int = 6,
+        seed: int = -1,
+        n_batch: int = 8,
+        top_k: int = 40,
+        top_p: float = 0.9,
+        temp: float = 0.9,
+        eos_token_id: int = 11,
+        stream_callback: Optional[Callable[[List[int]], None]] = None,
+    ) -> List[int]:
+        """
+        Generate tokens using the Falcon model.
+
+        Args:
+            tokens (List[int]): List of input tokens.
+            n_predict (int): Number of tokens to predict. Defaults to 200.
+            n_threads (int, optional): Number of threads to use for processing. Defaults to 6.
+            seed (int, optional): The seed for the random number generator. Defaults to -1.
+            n_batch (int, optional): Batch size for prompt processing. Defaults to 8.
+            top_k (int, optional): Top-k sampling parameter. Defaults to 40.
+            top_p (float, optional): Top-p sampling parameter. Defaults to 0.9.
+            temp (float, optional): Temperature parameter. Defaults to 0.9.
+            eos_token_id (int, optional): End of text special token id. Defaults to 11.
+            stream_callback (Optional[Callable[[List[int]], None]]): Optional callback function to receive generated tokens.
+
+        Returns:
+            List[int]: List of generated tokens.
+        """
+        func = clibrary.falcon_generate
+        func.argtypes = [
+            c_void_p,  # model
+            POINTER(c_int32),  # input tokens array
+            c_int32,  # input tokens length
+            POINTER(c_int32),  # output tokens array
+            c_int32,  # n_predict
+            c_int32,  # n_threads
+            c_int32,  # seed
+            c_int32,  # n_batch
+            c_int32,  # top_k
+            c_float,  # top_p
+            c_float,  # temp
+        ]
+
+        # Convert input tokens to a C-compatible array
+        input_tokens_len = len(tokens)
+        input_tokens_arr = (c_int32 * input_tokens_len)()
+        for i in range(input_tokens_len):
+            input_tokens_arr[i] = tokens[i]
+
+        # Create an array for output tokens and initialize with zeros
+        # Add a last end_of_text token (0) at the end
+        output_tokens_len = n_predict + 1
+        output_tokens_arr = (c_int32 * (output_tokens_len))()
+        for i in range(output_tokens_len):
+            output_tokens_arr[i] = eos_token_id
+
+        # Initialize thread_stop_event if stream_callback is provided
+        thread_stop_event: Optional[threading.Event] = None
+        if stream_callback:
+            thread_stop_event = threading.Event()
+
+            # Define a thread to handle streaming of generated tokens
+            def stream_thread():
+                num_printed_tokens = 0
+                while True:
+                    time.sleep(0.5)
+                    tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
+                    curr_len = tokens.index(eos_token_id)
+                    if curr_len > num_printed_tokens:
+                        stream_callback(tokens[num_printed_tokens:curr_len])
+                        num_printed_tokens = curr_len
+
+                    if thread_stop_event.is_set():
+                        break
+
+            # Start the stream_thread
+            threading.Thread(target=stream_thread).start()
+
+        # Start tokens generation on GGML backend
+        func(
+            self.ggml_model,
+            input_tokens_arr,
+            input_tokens_len,
+            output_tokens_arr,
+            n_predict,
+            n_threads,
+            seed,
+            n_batch,
+            top_k,
+            top_p,
+            temp,
+        )
+
+        # Stop the stream_thread if it was started
+        if thread_stop_event is not None:
+            time.sleep(1)
+            thread_stop_event.set()
+
+        # Retrieve the generated tokens and return them
+        output_tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
+        return output_tokens[: output_tokens.index(eos_token_id) + 1]
```

## cosmian_py_ggml/gpt_neox.py

```diff
@@ -1,155 +1,144 @@
 # -*- coding: utf-8 -*-
 import pathlib
 import threading
 import time
-from ctypes import CDLL, POINTER, Structure, c_char_p, c_float, c_int32
+from ctypes import CDLL, POINTER, c_char_p, c_float, c_int32, c_void_p
 from typing import Callable, List, Optional
 
 library_path = pathlib.Path(__file__).parent.resolve() / "libggml-bindings.so"
 clibrary = CDLL(str(library_path))
 
 
-class gpt_neox_model(Structure):
+class GPTNeoX:
     """
-    GPT-NeoX model in GGML backend.
+    GPT-NeoX model bindings for GGML.
     """
 
-
-def load_model(model_path: str):
-    """
-    Load the GPT-NeoX model from the given model path.
-
-    Args:
-        model_path (str): Path to the model file.
-
-    Returns:
-        POINTER(gpt_neox_model): Pointer to the loaded model.
-    """
-    func = clibrary.gpt_neox_load_model
-    func.argtypes = [c_char_p]
-    func.restype = POINTER(gpt_neox_model)
-
-    return func(model_path.encode("utf-8"))
-
-
-def free_model(model):
-    """
-    Free the memory allocated for the GPT-NeoX model.
-
-    Args:
-        model (POINTER(gpt_neox_model)): Pointer to the model.
-
-    Returns:
-        int: Status code indicating success (0) or failure.
-    """
-
-    func = clibrary.gpt_neox_free_model
-    func.argtypes = [POINTER(gpt_neox_model)]
-    func.restype = c_int32
-
-    return func(model)
-
-
-def generate(
-    model,
-    tokens: List[int],
-    n_predict: int = 200,
-    n_threads: int = 6,
-    seed: int = -1,
-    n_batch: int = 8,
-    top_k: int = 40,
-    top_p: float = 0.9,
-    temp: float = 0.9,
-    stream_callback: Optional[Callable[[List[int]], None]] = None,
-):
-    """
-    Generate tokens using the GPT-NeoX model.
-
-    Args:
-        model(POINTER(gpt_neox_model)): The GPT-NeoX model.
-        tokens (List[int]): List of input tokens.
-        n_predict (int): Number of tokens to predict. Defaults to 200.
-        n_threads (int, optional): Number of threads to use for processing. Defaults to 6.
-        seed (int, optional): The seed for the random number generator. Defaults to -1.
-        n_batch (int, optional): Batch size for prompt processing. Defaults to 8.
-        top_k (int, optional): Top-k sampling parameter. Defaults to 40.
-        top_p (float, optional): Top-p sampling parameter. Defaults to 0.9.
-        temp (float, optional): Temperature parameter. Defaults to 0.9.
-        stream_callback (Optional[Callable[[List[int]], None]]): Optional callback function to receive generated tokens.
-
-    Returns:
-        List[int]: List of generated tokens.
-    """
-    func = clibrary.gpt_neox_generate
-    func.argtypes = [
-        POINTER(gpt_neox_model),  # model
-        POINTER(c_int32),  # input tokens array
-        c_int32,  # input tokens length
-        POINTER(c_int32),  # output tokens array
-        c_int32,  # n_predict
-        c_int32,  # n_threads
-        c_int32,  # seed
-        c_int32,  # n_batch
-        c_int32,  # top_k
-        c_float,  # top_p
-        c_float,  # temp
-    ]
-
-    # Convert input tokens to a C-compatible array
-    input_tokens_len = len(tokens)
-    input_tokens_arr = (c_int32 * input_tokens_len)()
-    for i in range(input_tokens_len):
-        input_tokens_arr[i] = tokens[i]
-
-    # Create an array for output tokens and initialize with zeros
-    # Add a last end_of_text token (0) at the end
-    output_tokens_len = n_predict + 1
-    output_tokens_arr = (c_int32 * (output_tokens_len))()
-    for i in range(output_tokens_len):
-        output_tokens_arr[i] = 0
-
-    # Initialize thread_stop_event if stream_callback is provided
-    thread_stop_event: Optional[threading.Event] = None
-    if stream_callback:
-        thread_stop_event = threading.Event()
-
-        # Define a thread to handle streaming of generated tokens
-        def stream_thread():
-            len = 0
-            while True:
-                time.sleep(0.5)
-                tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
-                curr_len = tokens.index(0)
-                if curr_len > len:
-                    stream_callback(tokens[len:curr_len])
-                    len = curr_len
-
-                if thread_stop_event.is_set():
-                    break
-
-        # Start the stream_thread
-        threading.Thread(target=stream_thread).start()
-
-    # Start tokens generation on GGML backend
-    func(
-        model,
-        input_tokens_arr,
-        input_tokens_len,
-        output_tokens_arr,
-        n_predict,
-        n_threads,
-        seed,
-        n_batch,
-        top_k,
-        top_p,
-        temp,
-    )
-
-    # Stop the stream_thread if it was started
-    if thread_stop_event is not None:
-        time.sleep(1)
-        thread_stop_event.set()
-
-    # Retrieve the generated tokens and return them
-    output_tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
-    return output_tokens[: output_tokens.index(0) + 1]
+    def __init__(self, model_path: str):
+        """
+        Load GPT-NeoX model from the given model path.
+
+        Args:
+            model_path (str): Path to the model file.
+        """
+        func = clibrary.gpt_neox_load_model
+        func.argtypes = [c_char_p]
+        func.restype = c_void_p
+
+        self.ggml_model = func(model_path.encode("utf-8"))
+
+    def __del__(self):
+        """
+        Free the memory allocated for the model.
+        """
+
+        func = clibrary.gpt_neox_free_model
+        func.argtypes = [c_void_p]
+        func.restype = c_int32
+
+        func(self.ggml_model)
+
+    def __call__(
+        self,
+        tokens: List[int],
+        n_predict: int = 200,
+        n_threads: int = 6,
+        seed: int = -1,
+        n_batch: int = 8,
+        top_k: int = 40,
+        top_p: float = 0.9,
+        temp: float = 0.9,
+        eos_token_id: int = 0,
+        stream_callback: Optional[Callable[[List[int]], None]] = None,
+    ):
+        """
+        Generate tokens using the GPT-NeoX model.
+
+        Args:
+            tokens (List[int]): List of input tokens.
+            n_predict (int): Number of tokens to predict. Defaults to 200.
+            n_threads (int, optional): Number of threads to use for processing. Defaults to 6.
+            seed (int, optional): The seed for the random number generator. Defaults to -1.
+            n_batch (int, optional): Batch size for prompt processing. Defaults to 8.
+            top_k (int, optional): Top-k sampling parameter. Defaults to 40.
+            top_p (float, optional): Top-p sampling parameter. Defaults to 0.9.
+            temp (float, optional): Temperature parameter. Defaults to 0.9.
+            eos_token_id (int, optional): End of text special token id. Defaults to 0.
+            stream_callback (Optional[Callable[[List[int]], None]]): Optional callback function to receive generated tokens.
+
+        Returns:
+            List[int]: List of generated tokens.
+        """
+        func = clibrary.gpt_neox_generate
+        func.argtypes = [
+            c_void_p,  # model
+            POINTER(c_int32),  # input tokens array
+            c_int32,  # input tokens length
+            POINTER(c_int32),  # output tokens array
+            c_int32,  # n_predict
+            c_int32,  # n_threads
+            c_int32,  # seed
+            c_int32,  # n_batch
+            c_int32,  # top_k
+            c_float,  # top_p
+            c_float,  # temp
+        ]
+
+        # Convert input tokens to a C-compatible array
+        input_tokens_len = len(tokens)
+        input_tokens_arr = (c_int32 * input_tokens_len)()
+        for i in range(input_tokens_len):
+            input_tokens_arr[i] = tokens[i]
+
+        # Create an array for output tokens and initialize with zeros
+        # Add a last end_of_text token (0) at the end
+        output_tokens_len = n_predict + 1
+        output_tokens_arr = (c_int32 * (output_tokens_len))()
+        for i in range(output_tokens_len):
+            output_tokens_arr[i] = eos_token_id
+
+        # Initialize thread_stop_event if stream_callback is provided
+        thread_stop_event: Optional[threading.Event] = None
+        if stream_callback:
+            thread_stop_event = threading.Event()
+
+            # Define a thread to handle streaming of generated tokens
+            def stream_thread():
+                num_printed_tokens = 0
+                while True:
+                    time.sleep(0.5)
+                    tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
+                    curr_len = tokens.index(eos_token_id)
+                    if curr_len > num_printed_tokens:
+                        stream_callback(tokens[num_printed_tokens:curr_len])
+                        num_printed_tokens = curr_len
+
+                    if thread_stop_event.is_set():
+                        break
+
+            # Start the stream_thread
+            threading.Thread(target=stream_thread).start()
+
+        # Start tokens generation on GGML backend
+        func(
+            self.ggml_model,
+            input_tokens_arr,
+            input_tokens_len,
+            output_tokens_arr,
+            n_predict,
+            n_threads,
+            seed,
+            n_batch,
+            top_k,
+            top_p,
+            temp,
+        )
+
+        # Stop the stream_thread if it was started
+        if thread_stop_event is not None:
+            time.sleep(1)
+            thread_stop_event.set()
+
+        # Retrieve the generated tokens and return them
+        output_tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
+        return output_tokens[: output_tokens.index(eos_token_id) + 1]
```

## cosmian_py_ggml/__init__.py

```diff
@@ -0,0 +1,8 @@
+00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
+00000010: 662d 3820 2d2a 2d0a 6672 6f6d 202e 6661  f-8 -*-.from .fa
+00000020: 6c63 6f6e 2069 6d70 6f72 7420 4661 6c63  lcon import Falc
+00000030: 6f6e 4d6f 6465 6c0a 6672 6f6d 202e 6770  onModel.from .gp
+00000040: 745f 6e65 6f78 2069 6d70 6f72 7420 4750  t_neox import GP
+00000050: 544e 656f 580a 0a5f 5f61 6c6c 5f5f 203d  TNeoX..__all__ =
+00000060: 205b 2246 616c 636f 6e4d 6f64 656c 222c   ["FalconModel",
+00000070: 2022 4750 544e 656f 5822 5d0a             "GPTNeoX"].
```

## Comparing `cosmian_py_ggml-0.5.0.dist-info/METADATA` & `cosmian_py_ggml-1.0.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmian-py-ggml
-Version: 0.5.0
+Version: 1.0.0
 Summary: Python bindings for GGML
 License: MIT
 Author: Hugo Rosenkranz-Costa
 Author-email: hugo.rosenkranz@cosmian.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,39 +21,35 @@
 This library provides python bindings for the [examples models](https://github.com/ggerganov/ggml/tree/master/examples) of ggml.
 
 ## Available models architecture
 
 - [gpt-neox](https://huggingface.co/docs/transformers/model_doc/gpt_neox)
 
 ```python
-from cosmian_py_ggml import gpt_neox
+from cosmian_py_ggml import GPTNeoX
 from transformers import AutoTokenizer
 
 tokenizer = AutoTokenizer.from_pretrained("EleutherAI/gpt-neox-20b")
-model = gpt_neox.load_model("ggml_model_path")
+model = GPTNeoX("ggml_model_path")
 
-res = gpt_neox.generate(model, tokenizer.encode(query))
+res = model(tokenizer.encode(query))
 print("Response:", tokenizer.decode(res))
-
-gpt_neox.free_model(model)
 ```
 
 - [falcon 7b](https://huggingface.co/blog/falcon)
 
 ```python
-from cosmian_py_ggml import falcon
+from cosmian_py_ggml import FalconModel
 from transformers import AutoTokenizer
 
 tokenizer = AutoTokenizer.from_pretrained("tiiuae/falcon-7b")
-model = falcon.load_model("ggml_model_path")
+model = FalconModel("ggml_model_path")
 
-res = falcon.generate(model, tokenizer.encode(query))
+res = model(tokenizer.encode(query))
 print("Response:", tokenizer.decode(res))
-
-falcon.free_model(model)
 ```
 
 ## Build from sources
 
 ```bash
 git clone --recursive git@github.com:Cosmian/cosmian_py_ggml.git
 scripts/build.sh
```

## Comparing `cosmian_py_ggml-0.5.0.dist-info/LICENSE` & `cosmian_py_ggml-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

