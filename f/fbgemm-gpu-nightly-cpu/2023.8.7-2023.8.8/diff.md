# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.8.7-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.8.8-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,43 +1,43 @@
-Zip file size: 3286043 bytes, number of entries: 41
--rw-r--r--  2.0 unx      567 b- defN 23-Aug-07 12:58 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14920 b- defN 23-Aug-07 12:58 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2747 b- defN 23-Aug-07 12:58 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      818 b- defN 23-Aug-07 12:58 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10915464 b- defN 23-Aug-07 12:58 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5648 b- defN 23-Aug-07 12:58 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2339 b- defN 23-Aug-07 12:58 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2737 b- defN 23-Aug-07 12:58 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-Aug-07 12:58 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4005 b- defN 23-Aug-07 12:58 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5745 b- defN 23-Aug-07 12:58 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     6661 b- defN 23-Aug-07 12:58 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      525 b- defN 23-Aug-07 12:58 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    19833 b- defN 23-Aug-07 12:58 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Aug-07 12:58 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3433 b- defN 23-Aug-07 12:58 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    60371 b- defN 23-Aug-07 12:58 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    80930 b- defN 23-Aug-07 12:58 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    39550 b- defN 23-Aug-07 12:58 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      910 b- defN 23-Aug-07 12:58 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1603 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4076 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     3291 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     2775 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     1906 b- defN 23-Aug-07 12:53 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3291 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3040 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     2316 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2996 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     2996 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     4320 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6067 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     2768 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4602 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     3658 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx      635 b- defN 23-Aug-07 12:53 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6136 b- defN 23-Aug-07 12:56 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx     2933 b- defN 23-Aug-07 12:58 fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Aug-07 12:58 fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Aug-07 12:58 fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4530 b- defN 23-Aug-07 12:58 fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/RECORD
-41 files, 11241110 bytes uncompressed, 3278413 bytes compressed:  70.8%
+Zip file size: 3286035 bytes, number of entries: 41
+-rw-r--r--  2.0 unx      567 b- defN 23-Aug-08 12:59 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14920 b- defN 23-Aug-08 12:59 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-Aug-08 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Aug-08 12:59 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10915464 b- defN 23-Aug-08 12:59 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5648 b- defN 23-Aug-08 12:59 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-Aug-08 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2737 b- defN 23-Aug-08 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-Aug-08 12:59 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-Aug-08 12:59 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5745 b- defN 23-Aug-08 12:59 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     6661 b- defN 23-Aug-08 12:59 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      525 b- defN 23-Aug-08 12:59 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    19833 b- defN 23-Aug-08 12:59 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Aug-08 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3433 b- defN 23-Aug-08 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    60371 b- defN 23-Aug-08 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    80930 b- defN 23-Aug-08 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    39550 b- defN 23-Aug-08 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      910 b- defN 23-Aug-08 12:59 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1603 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4076 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     3291 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     2775 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     1906 b- defN 23-Aug-08 12:53 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3291 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     2316 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2996 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     2996 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     4320 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6067 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     2768 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4602 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     3658 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx      635 b- defN 23-Aug-08 12:53 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6136 b- defN 23-Aug-08 12:56 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     2933 b- defN 23-Aug-08 12:59 fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Aug-08 12:59 fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Aug-08 12:59 fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4530 b- defN 23-Aug-08 12:59 fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/RECORD
+41 files, 11241110 bytes uncompressed, 3278405 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -105,20 +105,20 @@
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### strings --all --bytes=8 {}

```diff
@@ -15302,31 +15302,31 @@
 QualifiedName
 basic_string::substr
 ArrayRef: invalid slice, N = 
 ; size = 
 defineMethod
 Default values must be specified for none or all arguments
 /github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/custom_class.h
-isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2308, please report a bug to PyTorch. 
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1951, please report a bug to PyTorch. 
+isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2311, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1954, please report a bug to PyTorch. 
 vector::_M_range_check: __n (which is %zu) >= this->size() (which is %zu)
 __getstate__ should take exactly one argument: self. Got: 
 self argument of __getstate__ must be the custom class type. Got 
 __getstate__ should return exactly one value for serialization. Got: 
 __getstate__'s return type should be a subtype of input argument of __setstate__. Got 
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/embedding_forward_quantized_host_cpu.cpp
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function shouldn't be called for CPU; it is only for GPU.
 int_nbit_split_embedding_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, int total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment = None, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1) -> Tensor
 int_nbit_split_embedding_codegen_lookup_function
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, int total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights=None, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment=-1, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1, Tensor? cache_hash_size_cumsum=None, int? total_cache_hash_size=-1, Tensor? cache_index_table_map=None, Tensor? lxu_cache_state=None, Tensor? lxu_state=None) -> Tensor
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function
 pruned_hashmap_insert(Tensor indices, Tensor dense_indices, Tensor offsets, Tensor(a!) hash_table, Tensor hash_table_offsets) -> ()
 pruned_hashmap_lookup(Tensor indices, Tensor offsets, Tensor hash_table, Tensor hash_table_offsets) -> Tensor
 pruned_array_lookup(Tensor indices, Tensor offsets, Tensor index_remappings, Tensor index_remappings_offsets) -> Tensor
-isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2067, please report a bug to PyTorch. 
+isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2070, please report a bug to PyTorch. 
 Expected a 0-dim Tensor, but got Tensor with dimensions: 
 tensor.dim() == 0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":326, please report a bug to PyTorch. 
 /github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h
  in its first dimension, but got Tensor with size 
 tensor.sizes()[0] == (int64_t)init_list_.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":333, please report a bug to PyTorch. 
 TensorDataContainer is already a Tensor type, `fill_tensor` should not be called
 false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":347, please report a bug to PyTorch. 
@@ -15577,15 +15577,15 @@
 fbgemm::jagged_to_padded_dense_backward
 fbgemm::jagged_to_padded_dense_forward
 Expected values.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected offsets.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_L > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_lengths.size() == x_offsets.size() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected SymIntList or IntList but got 
-isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1963, please report a bug to PyTorch. 
+isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1966, please report a bug to PyTorch. 
 /github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h
 Expected dense_values_grad.sym_sizes() == dense_shape to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 fbgemm::jagged_dense_dense_elementwise_add_jagged_output_forward
 fbgemm::jagged_dense_elementwise_mul_backward
 fbgemm::jagged_dense_elementwise_mul_forward
 fbgemm::batched_dense_vec_jagged_2d_mul_backward
 fbgemm::batched_dense_vec_jagged_2d_mul_forward
@@ -15612,21 +15612,21 @@
 /github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
 Tried to cast a List<
 > to a List<
 >. Types mismatch.
 toTypedList
 /github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/List_inl.h
 Expected GenericList but got 
-isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2051, please report a bug to PyTorch. 
+isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2054, please report a bug to PyTorch. 
 Expected TensorList but got 
 toTensorList
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2023, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2026, please report a bug to PyTorch. 
 isDouble() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":542, please report a bug to PyTorch. 
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1947, please report a bug to PyTorch. 
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2019, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1950, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2022, please report a bug to PyTorch. 
 toDouble
 isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":237, please report a bug to PyTorch. 
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EERKN3c108ArrayRefINS8_6SymIntEEEdE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EERKN3c106SymIntEE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EES2_S2_E
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EES2_E
 FSt5tupleIJN2at6TensorES1_EERKS1_RKSt6vectorIS1_SaIS1_EES4_S4_E
@@ -16246,15 +16246,15 @@
 pruned_array_lookup_from_row_idx_cpu_kernel
 pruned_array_lookup_from_row_idx
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_S5_S5_S5_S5_S5_lNS_8optionalIS5_EES7_EXadL_ZN10fbgemm_gpu28embedding_inplace_update_cpuES5_S5_S5_S5_S5_S5_S5_S5_S5_S5_lS7_S7_EEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_S5_S5_S5_S5_S5_lS7_S7_EEEEE
 FvN2at6TensorES0_S0_S0_S0_S0_S0_S0_S0_S0_lN3c108optionalIS0_EES3_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_EXadL_ZN10fbgemm_gpu36pruned_array_lookup_from_row_idx_cpuES7_S7_S7_S7_EEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_EEEEE
 pruned_array_lookup_from_row_idx(Tensor update_row_indices, Tensor update_table_index_remappings, Tensor index_remappings_offsetbatch_index_select_dim0
 batch_index_select_dim0_cpu
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1955, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1958, please report a bug to PyTorch. 
 toIntVector
 batch_index_select_dim0(    Tensor inputs,    Tensor indices,    int[] input_num_indices,    int[] input_rows,    int[] input_columns,    bool permute_output_dim_0_1=False) -> Tensor
 [batch_index_select_dim0] input_rows must have the same length as input_num_indices.
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/batch_index_select_dim0_cpu_host.cpp
 [batch_index_select_dim0] input_columns must have the same length as input_num_indices.
 Currently batch_index_select only supports 16-byte align input tensors
 [batch_index_select_dim0] All input_columns must be the same.
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -153717,15 +153717,15 @@
 	mov    %rbx,%rdx
 	mov    %r15,%rsi
 	mov    %r12,%rdi
 	mov    %rax,0x48(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r12,%r8
 	lea    0x79afa5(%rip),%rcx        
-	mov    $0x904,%edx
+	mov    $0x907,%edx
 	lea    0x79a879(%rip),%rsi        
 	lea    0x799cc2(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	lea    0x40(%rsp),%rbx
 	mov    0x8(%rbp),%esi
 	mov    %rbx,%rdi
 	call   528160 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, long)>()@@Base+0x390>
@@ -153734,15 +153734,15 @@
 	mov    %rbx,%rdx
 	mov    %r15,%rdi
 	mov    %r12,%rsi
 	mov    %rax,0x38(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r15,%r8
 	lea    0x79b00c(%rip),%rcx        
-	mov    $0x79f,%edx
+	mov    $0x7a2,%edx
 	lea    0x79a828(%rip),%rsi        
 	lea    0x799c97(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	test   %dl,%dl
 	je     1fe18f <torch::autograd::Node::compiled_args(torch::dynamo::autograd::CompiledNodeArgs&)@@Base+0x9d58f>
 	mov    (%rdi),%rsi
 	mov    %r12,%rdi
@@ -888882,15 +888882,15 @@
 	mov    %r13,%rsi
 	mov    %r14,%rdi
 	lea    0x46e2bc(%rip),%rax        
 	mov    %rax,0xa0(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r14,%r8
 	lea    0x46f58e(%rip),%rcx        
-	mov    $0x904,%edx
+	mov    $0x907,%edx
 	lea    0x46ee62(%rip),%rsi        
 	lea    0x46e2ab(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    %r13,%rsi
 	call   527ef0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, long)>()@@Base+0x120>
 	jmp    5299b8 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<at::Tensor>)@@Base+0x6e8>
@@ -889943,15 +889943,15 @@
 	mov    %r12,%rsi
 	mov    %r14,%rdi
 	lea    0x46cd8d(%rip),%rax        
 	mov    %rax,0x40(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r14,%r8
 	lea    0x46e062(%rip),%rcx        
-	mov    $0x904,%edx
+	mov    $0x907,%edx
 	lea    0x46d936(%rip),%rsi        
 	lea    0x46cd7f(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	xchg   %ax,%ax
 	mov    %r12,%rsi
 	call   527ef0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, long)>()@@Base+0x120>
 	jmp    52af00 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<at::Tensor>)@@Base+0x1c30>
@@ -890551,15 +890551,15 @@
 	lea    0x46c4c4(%rip),%rax        
 	mov    %r14,%rsi
 	mov    %r13,%rdi
 	mov    %rax,0x20(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r13,%r8
 	lea    0x46e0fd(%rip),%rcx        
-	mov    $0x813,%edx
+	mov    $0x816,%edx
 	lea    0x46cf41(%rip),%rsi        
 	lea    0x46c4b5(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopl   0x0(%rax,%rax,1)
 	mov    0x10(%rsp),%rax
 	mov    0x10(%rax),%rax
 	cmp    $0x1,%rax
@@ -916766,15 +916766,15 @@
 	mov    %rbx,%rsi
 	call   1577d0 <__cxa_atexit@plt>
 	mov    %r14,%rdi
 	call   15a210 <__cxa_guard_release@plt>
 	jmp    545b37 <c10::intrusive_ptr<PrunedMapCPU, c10::detail::intrusive_target_default_null_type<PrunedMapCPU> > c10::IValue::toCustomClass<PrunedMapCPU>() &&@@Base+0x57>
 	cs nopw 0x0(%rax,%rax,1)
 	lea    0x4554a1(%rip),%rcx        
-	mov    $0x6e7,%edx
+	mov    $0x6ea,%edx
 	lea    0x452dc5(%rip),%rsi        
 	lea    0x455596(%rip),%rdi        
 	call   155ed0 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nop
 	lea    0x4554d1(%rip),%rcx        
 	mov    $0xe1,%edx
 	lea    0x452da5(%rip),%rsi        
@@ -917244,15 +917244,15 @@
 	mov    %rbx,%rsi
 	call   1577d0 <__cxa_atexit@plt>
 	mov    %r14,%rdi
 	call   15a210 <__cxa_guard_release@plt>
 	jmp    5462a7 <c10::intrusive_ptr<AtomicCounter, c10::detail::intrusive_target_default_null_type<AtomicCounter> > c10::IValue::toCustomClass<AtomicCounter>() &&@@Base+0x57>
 	cs nopw 0x0(%rax,%rax,1)
 	lea    0x454d31(%rip),%rcx        
-	mov    $0x6e7,%edx
+	mov    $0x6ea,%edx
 	lea    0x452655(%rip),%rsi        
 	lea    0x454e26(%rip),%rdi        
 	call   155ed0 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nop
 	lea    0x454d61(%rip),%rcx        
 	mov    $0xe1,%edx
 	lea    0x452635(%rip),%rsi        
@@ -917670,15 +917670,15 @@
 	mov    %rbx,%rsi
 	call   1577d0 <__cxa_atexit@plt>
 	mov    %r14,%rdi
 	call   15a210 <__cxa_guard_release@plt>
 	jmp    5468e7 <c10::intrusive_ptr<TensorQueue, c10::detail::intrusive_target_default_null_type<TensorQueue> > c10::IValue::toCustomClass<TensorQueue>() &&@@Base+0x57>
 	cs nopw 0x0(%rax,%rax,1)
 	lea    0x4546f1(%rip),%rcx        
-	mov    $0x6e7,%edx
+	mov    $0x6ea,%edx
 	lea    0x452015(%rip),%rsi        
 	lea    0x4547e6(%rip),%rdi        
 	call   155ed0 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nop
 	lea    0x454721(%rip),%rcx        
 	mov    $0xe1,%edx
 	lea    0x451ff5(%rip),%rsi        
@@ -945123,15 +945123,15 @@
 	lea    -0x100(%rbp),%rax
 	mov    %r15,%rdi
 	mov    %rax,%rsi
 	mov    %rax,-0x1c8(%rbp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r15,%r8
 	lea    0x43c5e3(%rip),%rcx        # 9a0598 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1f58>
-	mov    $0x7ab,%edx
+	mov    $0x7ae,%edx
 	lea    0x434af7(%rip),%rsi        
 	lea    0x43a826(%rip),%rdi        # 99e7ee <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1ae>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopl   (%rax)
 	lea    -0xa0(%rbp),%rsi
 	call   55a280 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0xd50>
 	jmp    563553 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xe23>
@@ -945976,15 +945976,15 @@
 	lea    -0x100(%rbp),%rax
 	mov    %r14,%rdi
 	mov    %rax,%rsi
 	mov    %rax,-0x1d0(%rbp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r14,%r8
 	lea    0x43b5a8(%rip),%rcx        # 9a0598 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1f58>
-	mov    $0x7ab,%edx
+	mov    $0x7ae,%edx
 	lea    0x433abc(%rip),%rsi        
 	lea    0x4397eb(%rip),%rdi        # 99e7ee <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1ae>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopl   0x0(%rax,%rax,1)
 	lea    0x43b159(%rip),%rcx        # 9a0170 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1b30>
 	mov    $0x130,%edx
 	lea    0x43b09d(%rip),%rsi        # 9a00c0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1a80>
@@ -964871,15 +964871,15 @@
 	mov    %rbx,%rdx
 	mov    %r12,%rdi
 	mov    %r14,%rsi
 	mov    %rax,0x10(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r12,%r8
 	lea    0x41ddbf(%rip),%rcx        
-	mov    $0x79f,%edx
+	mov    $0x7a2,%edx
 	lea    0x41d5db(%rip),%rsi        
 	lea    0x41ca4a(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopl   0x0(%rax)
 	test   %rdi,%rdi
 	je     57b3df <c10::IValue::IValue<c10::SymInt, decltype(nullptr)>(c10::ArrayRef<c10::SymInt>)@@Base+0x26f>
 	jmp    57b45c <c10::IValue::IValue<c10::SymInt, decltype(nullptr)>(c10::ArrayRef<c10::SymInt>)@@Base+0x2ec>
@@ -964904,15 +964904,15 @@
 	mov    %rbx,%rdx
 	mov    %r15,%rdi
 	mov    %r14,%rsi
 	mov    %rax,0x10(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r15,%r8
 	lea    0x42595a(%rip),%rcx        # 9a0ed0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2890>
-	mov    $0x803,%edx
+	mov    $0x806,%edx
 	lea    0x41d536(%rip),%rsi        
 	lea    0x42593d(%rip),%rdi        # 9a0ec6 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2886>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	mov    0x4e727b(%rip),%r15        
 	jmp    57b1f7 <c10::IValue::IValue<c10::SymInt, decltype(nullptr)>(c10::ArrayRef<c10::SymInt>)@@Base+0x87>
 	mov    %rax,%rbp
 	jmp    57b5b0 <c10::IValue::IValue<c10::SymInt, decltype(nullptr)>(c10::ArrayRef<c10::SymInt>)@@Base+0x440>
@@ -966067,15 +966067,15 @@
 	mov    %r15,%rdx
 	mov    %rbx,%rsi
 	mov    %r12,%rdi
 	mov    %rax,0x10(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r12,%r8
 	lea    0x4248b0(%rip),%rcx        # 9a0fb0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2970>
-	mov    $0x7e7,%edx
+	mov    $0x7ea,%edx
 	lea    0x41c3ac(%rip),%rsi        
 	lea    0x424890(%rip),%rdi        # 9a0fa3 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2963>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopl   0x0(%rax,%rax,1)
 	test   %rdi,%rdi
 	je     57c63c <c10::IValue::IValue<at::Tensor, decltype(nullptr)>(std::vector<at::Tensor, std::allocator<at::Tensor> > const&)@@Base+0x1ac>
 	jmp    57c69c <c10::IValue::IValue<at::Tensor, decltype(nullptr)>(std::vector<at::Tensor, std::allocator<at::Tensor> > const&)@@Base+0x20c>
@@ -968951,15 +968951,15 @@
 	lea    0x418947(%rip),%rax        
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	mov    %rax,0x28(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r15,%r8
 	lea    0x421b41(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0x4194c5(%rip),%rsi        
 	lea    0x418934(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	mov    0x38(%rsp),%esi
 	mov    %rbx,%rdi
 	call   55b6a0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x2170>
 	lea    0x20(%rsp),%rbp
@@ -968967,15 +968967,15 @@
 	mov    %rbx,%rdx
 	mov    %r14,%rdi
 	mov    %rbp,%rsi
 	mov    %rax,0x20(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r14,%r8
 	lea    0x421bb4(%rip),%rcx        # 9a11e8 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ba8>
-	mov    $0x7e3,%edx
+	mov    $0x7e6,%edx
 	lea    0x419478(%rip),%rsi        
 	lea    0x42195c(%rip),%rdi        # 9a0fa3 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2963>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	lea    -0x40(%rsi),%rdi
 	call   155fe0 <c10::IValue::reportToTensorTypeError() const@plt>
 	mov    %rax,%rbp
 	jmp    57f693 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double), &fbgemm_gpu::jagged_to_padded_dense>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x483>
@@ -969486,15 +969486,15 @@
 	lea    0x4210e9(%rip),%rax        # 9a0f86 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2946>
 	mov    %r12,%rsi
 	mov    %r13,%rdi
 	mov    %rax,0x18(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r13,%r8
 	lea    0x421331(%rip),%rcx        # 9a11e8 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ba8>
-	mov    $0x7e3,%edx
+	mov    $0x7e6,%edx
 	lea    0x418bf5(%rip),%rsi        
 	lea    0x4210d9(%rip),%rdi        # 9a0fa3 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2963>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	lea    -0x40(%rsi),%rdi
 	call   155fe0 <c10::IValue::reportToTensorTypeError() const@plt>
 	mov    %rax,%rbp
 	jmp    57fee9 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, std::vector<at::Tensor, std::allocator<at::Tensor> > > (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&), &fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output>, std::tuple<at::Tensor, std::vector<at::Tensor, std::allocator<at::Tensor> > >, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x2f9>
@@ -970246,15 +970246,15 @@
 	lea    0x4203e1(%rip),%rax        # 9a0f86 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2946>
 	mov    %r12,%rsi
 	mov    %r13,%rdi
 	mov    %rax,0x18(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r13,%r8
 	lea    0x420629(%rip),%rcx        # 9a11e8 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ba8>
-	mov    $0x7e3,%edx
+	mov    $0x7e6,%edx
 	lea    0x417eed(%rip),%rsi        
 	lea    0x4203d1(%rip),%rdi        # 9a0fa3 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2963>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	lea    -0x30(%rsi),%rdi
 	call   155fe0 <c10::IValue::reportToTensorTypeError() const@plt>
 	mov    %rax,%rbp
 	jmp    580bf1 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, std::vector<at::Tensor, std::allocator<at::Tensor> > > (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&), &fbgemm_gpu::jagged_dense_elementwise_mul>, std::tuple<at::Tensor, std::vector<at::Tensor, std::allocator<at::Tensor> > >, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x2d1>
@@ -971410,15 +971410,15 @@
 	lea    0x41efb9(%rip),%rax        # 9a0f86 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2946>
 	mov    %rbp,%rsi
 	mov    %r12,%rdi
 	mov    %rax,0x10(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r12,%r8
 	lea    0x41f201(%rip),%rcx        # 9a11e8 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ba8>
-	mov    $0x7e3,%edx
+	mov    $0x7e6,%edx
 	lea    0x416ac5(%rip),%rsi        
 	lea    0x41efa9(%rip),%rdi        # 9a0fa3 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2963>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	cmp    $0x5,%esi
 	jne    582043 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, std::vector<at::Tensor, std::allocator<at::Tensor> > > (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::optional<c10::SymInt> const&), &fbgemm_gpu::dense_to_jagged>, std::tuple<at::Tensor, std::vector<at::Tensor, std::allocator<at::Tensor> > >, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::optional<c10::SymInt> const&> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x3d3>
 	movabs $0xc000000000000000,%rdx
 	mov    0x50(%rsp),%rax
@@ -978292,15 +978292,15 @@
 	lea    0x418189(%rip),%rax        # 9a0f86 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2946>
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
 	mov    %rax,0x18(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbp,%r8
 	lea    0x4183d1(%rip),%rcx        # 9a11e8 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ba8>
-	mov    $0x7e3,%edx
+	mov    $0x7e6,%edx
 	lea    0x40fc95(%rip),%rsi        
 	lea    0x418179(%rip),%rdi        # 9a0fa3 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2963>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	lea    0x4117dc(%rip),%rdi        
 	call   156c60 <std::__throw_length_error(char const*)@plt>
 	mov    %rax,%rbx
 	jmp    588e4c <std::vector<at::Tensor, std::allocator<at::Tensor> > c10::IValue::to<std::vector<at::Tensor, std::allocator<at::Tensor> > >() &&@@Base+0x2ac>
@@ -979753,15 +979753,15 @@
 	mov    %rax,%rdi
 	mov    %rax,-0xb0(%rbp)
 	mov    %rax,%rbx
 	mov    %rcx,-0xc0(%rbp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbx,%r8
 	lea    0x40ec5f(%rip),%rcx        
-	mov    $0x79f,%edx
+	mov    $0x7a2,%edx
 	lea    0x40e47b(%rip),%rsi        
 	lea    0x40d8ea(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopl   0x0(%rax)
 	lea    -0x88(%rbp),%r14
 	mov    %r14,%rdi
 	call   583e70 <fbgemm_gpu::jagged_softmax_backward_meta(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x20>
@@ -979772,15 +979772,15 @@
 	mov    %r12,%rsi
 	mov    %rbx,%rdi
 	mov    %rbx,-0xb0(%rbp)
 	mov    %rax,-0x90(%rbp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbx,%r8
 	lea    0x416839(%rip),%rcx        # 9a0ed0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2890>
-	mov    $0x803,%edx
+	mov    $0x806,%edx
 	lea    0x40e415(%rip),%rsi        
 	lea    0x41681c(%rip),%rdi        # 9a0ec6 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2886>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	vzeroupper
 	jmp    58a556 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7a6>
 	lea    -0x88(%rbp),%rbx
 	mov    %rbx,%rdi
@@ -1507058,15 +1507058,15 @@
 	mov    %r12,%rsi
 	mov    %rbx,%rdi
 	mov    %rbx,-0xa8(%rbp)
 	mov    %rax,-0x90(%rbp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbx,%r8
 	lea    0x1cd459(%rip),%rcx        # 9a0ed0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2890>
-	mov    $0x803,%edx
+	mov    $0x806,%edx
 	lea    0x1c5035(%rip),%rsi        
 	lea    0x1cd43c(%rip),%rdi        # 9a0ec6 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2886>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nop
 	lea    -0x80(%rbp),%r12
 	mov    -0x18(%rbx),%esi
 	mov    %r12,%rdi
@@ -1507078,15 +1507078,15 @@
 	mov    %r14,%rsi
 	mov    %rbx,%rdi
 	mov    %rbx,-0xa8(%rbp)
 	mov    %rax,-0x88(%rbp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbx,%r8
 	lea    0x1c57b9(%rip),%rcx        
-	mov    $0x79f,%edx
+	mov    $0x7a2,%edx
 	lea    0x1c4fd5(%rip),%rsi        
 	lea    0x1c4444(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	vzeroupper
 	jmp    7d3816 <fbgemm_gpu::jagged_2d_to_dense_forward_cpu(at::Tensor, at::Tensor, long)@@Base+0x56346>
 	lea    -0x88(%rbp),%r14
 	mov    %r14,%rdi
@@ -1531128,15 +1531128,15 @@
 	lea    0x1acb7c(%rip),%rax        
 	mov    %r15,%rsi
 	mov    %rbp,%rdi
 	mov    %rax,0x48(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbp,%r8
 	lea    0x1b5d76(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0x1ad6fa(%rip),%rsi        
 	lea    0x1acb69(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x0(%rbp),%rax
 	mov    0x10(%rax),%rax
 	cmp    $0x1,%rax
@@ -1531194,15 +1531194,15 @@
 	mov    %r15,%rdx
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,0x40(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r13,%r8
 	lea    0x1b5c4d(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0x1ad5d1(%rip),%rsi        
 	lea    0x1aca40(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	mov    0x10(%r14),%rax
 	lea    0x10(%r14),%rbx
 	cmp    $0x1,%rax
 	je     7eb513 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::vector<at::Tensor, std::allocator<at::Tensor> > (at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long), &fbgemm_gpu::stacked_jagged_1d_to_dense_cpu>, std::vector<at::Tensor, std::allocator<at::Tensor> >, c10::guts::typelist::typelist<at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x783>
@@ -1531750,15 +1531750,15 @@
 	lea    0x1ac09c(%rip),%rax        
 	mov    %r15,%rsi
 	mov    %rbp,%rdi
 	mov    %rax,0x48(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbp,%r8
 	lea    0x1b5296(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0x1acc1a(%rip),%rsi        
 	lea    0x1ac089(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x0(%rbp),%rax
 	mov    0x10(%rax),%rax
 	cmp    $0x1,%rax
@@ -1531816,15 +1531816,15 @@
 	mov    %r15,%rdx
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,0x40(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r13,%r8
 	lea    0x1b516d(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0x1acaf1(%rip),%rsi        
 	lea    0x1abf60(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	mov    0x10(%r14),%rax
 	lea    0x10(%r14),%rbx
 	cmp    $0x1,%rax
 	je     7ebff3 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::vector<at::Tensor, std::allocator<at::Tensor> > (at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long), &fbgemm_gpu::stacked_jagged_2d_to_dense_cpu>, std::vector<at::Tensor, std::allocator<at::Tensor> >, c10::guts::typelist::typelist<at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x783>
@@ -1542006,15 +1542006,15 @@
 	lea    0x30(%rsp),%rdx
 	mov    %rbp,%rsi
 	mov    %r15,%rdi
 	mov    %rax,0x38(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r15,%r8
 	lea    0x1a9c13(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0x1a1597(%rip),%rsi        
 	lea    0x1a0a06(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	lea    0x15(%rsp),%rdx
 	xor    %esi,%esi
 	mov    $0x4,%edi
 	call   15ab00 <std::string::_Rep::_S_create(unsigned long, unsigned long, std::allocator<char> const&)@plt>
@@ -1660436,15 +1660436,15 @@
 	mov    %rax,%rdi
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rbx
 	mov    %rcx,0x50(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbx,%r8
 	lea    0x125713(%rip),%rcx        # 9a11e8 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ba8>
-	mov    $0x7e3,%edx
+	mov    $0x7e6,%edx
 	lea    0x11cfd7(%rip),%rsi        
 	lea    0x1254bb(%rip),%rdi        # 9a0fa3 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2963>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	mov    0x20(%r12),%rsi
 	mov    %rdx,%r13
 	shl    $0x4,%r13
 	mov    %rsi,%r14
@@ -1660704,15 +1660704,15 @@
 	lea    0x12506c(%rip),%rax        # 9a0f86 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2946>
 	mov    %r12,%rsi
 	mov    %rax,0x68(%rsp)
 	mov    %rbx,%rdi
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbx,%r8
 	lea    0x1252b4(%rip),%rcx        # 9a11e8 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ba8>
-	mov    $0x7e3,%edx
+	mov    $0x7e6,%edx
 	lea    0x11cb78(%rip),%rsi        
 	lea    0x12505c(%rip),%rdi        # 9a0fa3 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2963>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	xor    %r12d,%r12d
 	jmp    87b932 <fbgemm_gpu::permute_sequence_embeddings_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x2a82>
 	lock addl $0x1,0x8(%rax)
 	jmp    87b793 <fbgemm_gpu::permute_sequence_embeddings_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x28e3>
@@ -1660730,15 +1660730,15 @@
 	lea    0x124fe6(%rip),%rax        # 9a0f86 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2946>
 	mov    %r12,%rsi
 	mov    %rax,0x68(%rsp)
 	mov    %rbx,%rdi
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbx,%r8
 	lea    0x124ff6(%rip),%rcx        # 9a0fb0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2970>
-	mov    $0x7e7,%edx
+	mov    $0x7ea,%edx
 	lea    0x11caf2(%rip),%rsi        
 	lea    0x124fd6(%rip),%rdi        # 9a0fa3 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2963>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	xor    %r9d,%r9d
 	jmp    87bb25 <fbgemm_gpu::permute_sequence_embeddings_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x2c75>
 	mov    0x70(%rsp),%rax
 	mov    0x10(%rax),%rax
@@ -1698794,15 +1698794,15 @@
 	lea    0xf3c0f(%rip),%rax        
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
 	mov    %rax,0x10(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbp,%r8
 	lea    0xfce09(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0xf478d(%rip),%rsi        
 	lea    0xf3bfc(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	lea    0xf62d4(%rip),%rdi        
 	call   156c60 <std::__throw_length_error(char const*)@plt>
 	sub    $0x2,%eax
 	cmp    $0x18,%eax
@@ -1699184,15 +1699184,15 @@
 	lea    0xf357f(%rip),%rax        
 	mov    %rbp,%rsi
 	mov    %r13,%rdi
 	mov    %rax,0x10(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r13,%r8
 	lea    0xfc779(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0xf40fd(%rip),%rsi        
 	lea    0xf356c(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	lea    0xf5c44(%rip),%rdi        
 	call   156c60 <std::__throw_length_error(char const*)@plt>
 	sub    $0x2,%eax
 	cmp    $0x18,%eax
@@ -1710524,15 +1710524,15 @@
 	mov    %r12,%rdx
 	mov    %rbp,%rdi
 	mov    %r14,%rsi
 	mov    %rax,0x10(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbp,%r8
 	lea    0xe8126(%rip),%rcx        
-	mov    $0x79f,%edx
+	mov    $0x7a2,%edx
 	lea    0xe7942(%rip),%rsi        
 	lea    0xe6db1(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopw   0x0(%rax,%rax,1)
 	xor    %r9d,%r9d
 	jmp    8b10bc <c10::IValue::IValue<long, decltype(nullptr)>(std::vector<long, std::allocator<long> > const&)@@Base+0x1ac>
 	lea    0xe947b(%rip),%rdi        
@@ -1710650,15 +1710650,15 @@
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
 	lea    0xe6bda(%rip),%rax        
 	mov    %rax,0x18(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbp,%r8
 	lea    0x10023a(%rip),%rcx        # 9b1588 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&), &fbgemm_gpu::pruned_array_lookup_from_row_idx_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&> >@@Base+0x268>
-	mov    $0x7a3,%edx
+	mov    $0x7a6,%edx
 	lea    0xe775e(%rip),%rsi        
 	lea    0x1002e0(%rip),%rdi        # 9b1641 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&), &fbgemm_gpu::pruned_array_lookup_from_row_idx_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&> >@@Base+0x321>
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	mov    0x1b17ab(%rip),%rbx        
 	mov    %rax,%r12
 	jmp    8b139a <c10::IValue::toIntVector() const@@Base+0x16a>
 	mov    %rax,%rbp
@@ -1713572,15 +1713572,15 @@
 	lea    0xe343f(%rip),%rax        
 	mov    %r14,%rsi
 	mov    %rbp,%rdi
 	mov    %rax,0x8(%rsp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %rbp,%r8
 	lea    0xec639(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0xe3fbd(%rip),%rsi        
 	lea    0xe342c(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	mov    0x1ae00a(%rip),%r12        
 	mov    %rax,%rbx
 	jmp    8b4b38 <std::vector<long, std::allocator<long> > c10::IValue::to<std::vector<long, std::allocator<long> > >() &&@@Base+0x1c8>
 	mov    %rax,%rbp
@@ -1713827,15 +1713827,15 @@
 	lea    -0x98(%rbp),%rax
 	mov    %r15,%rdi
 	mov    %rax,%rsi
 	mov    %rax,-0xb8(%rbp)
 	call   15be80 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r15,%r8
 	lea    0xec1ce(%rip),%rcx        # 9a1128 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2ae8>
-	mov    $0x79b,%edx
+	mov    $0x79e,%edx
 	lea    0xe3b52(%rip),%rsi        
 	lea    0xe2fc1(%rip),%rdi        
 	call   1575e0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	mov    %r13,%rdx
 	mov    %r15,%rsi
 	mov    %r12,%rdi
 	call   15b520 <void std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_realloc_insert<c10::IValue>(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, c10::IValue&&)@plt>
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -10018,27 +10018,27 @@
   0x009991f0 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x00999200 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x00999210 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x00999220 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
   0x00999230 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00999240 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00999250 2f415465 6e2f636f 72652f69 76616c75 /ATen/core/ivalu
-  0x00999260 655f696e 6c2e6822 3a323330 382c2070 e_inl.h":2308, p
+  0x00999260 655f696e 6c2e6822 3a323331 312c2070 e_inl.h":2311, p
   0x00999270 6c656173 65207265 706f7274 20612062 lease report a b
   0x00999280 75672074 6f205079 546f7263 682e2000 ug to PyTorch. .
   0x00999290 6973496e 744c6973 74282920 494e5445 isIntList() INTE
   0x009992a0 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x009992b0 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x009992c0 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x009992d0 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
   0x009992e0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x009992f0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00999300 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x00999310 6f72652f 6976616c 75655f69 6e6c2e68 ore/ivalue_inl.h
-  0x00999320 223a3139 35312c20 706c6561 73652072 ":1951, please r
+  0x00999320 223a3139 35342c20 706c6561 73652072 ":1954, please r
   0x00999330 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x00999340 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x00999350 76656374 6f723a3a 5f4d5f72 616e6765 vector::_M_range
   0x00999360 5f636865 636b3a20 5f5f6e20 28776869 _check: __n (whi
   0x00999370 63682069 7320257a 7529203e 3d207468 ch is %zu) >= th
   0x00999380 69732d3e 73697a65 28292028 77686963 is->size() (whic
   0x00999390 68206973 20257a75 29000000 00000000 h is %zu).......
@@ -10188,15 +10188,15 @@
   0x00999c90 7420222f 67697468 75622f68 6f6d652f t "/github/home/
   0x00999ca0 6d696e69 636f6e64 612f656e 76732f62 miniconda/envs/b
   0x00999cb0 75696c64 5f62696e 6172792f 6c69622f uild_binary/lib/
   0x00999cc0 70797468 6f6e332e 392f7369 74652d70 python3.9/site-p
   0x00999cd0 61636b61 6765732f 746f7263 682f696e ackages/torch/in
   0x00999ce0 636c7564 652f4154 656e2f63 6f72652f clude/ATen/core/
   0x00999cf0 6976616c 75655f69 6e6c2e68 223a3230 ivalue_inl.h":20
-  0x00999d00 36372c20 706c6561 73652072 65706f72 67, please repor
+  0x00999d00 37302c20 706c6561 73652072 65706f72 70, please repor
   0x00999d10 74206120 62756720 746f2050 79546f72 t a bug to PyTor
   0x00999d20 63682e20 00000000 45787065 63746564 ch. ....Expected
   0x00999d30 20612030 2d64696d 2054656e 736f722c  a 0-dim Tensor,
   0x00999d40 20627574 20676f74 2054656e 736f7220  but got Tensor 
   0x00999d50 77697468 2064696d 656e7369 6f6e733a with dimensions:
   0x00999d60 20000000 00000000 74656e73 6f722e64  .......tensor.d
   0x00999d70 696d2829 203d3d20 3020494e 5445524e im() == 0 INTERN
@@ -11871,15 +11871,15 @@
   0x009a05c0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x009a05d0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x009a05e0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x009a05f0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
   0x009a0600 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
   0x009a0610 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x009a0620 7564652f 4154656e 2f636f72 652f6976 ude/ATen/core/iv
-  0x009a0630 616c7565 5f696e6c 2e68223a 31393633 alue_inl.h":1963
+  0x009a0630 616c7565 5f696e6c 2e68223a 31393636 alue_inl.h":1966
   0x009a0640 2c20706c 65617365 20726570 6f727420 , please report 
   0x009a0650 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x009a0660 2e200000 00000000 2f676974 6875622f . ....../github/
   0x009a0670 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009a0680 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
   0x009a0690 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
   0x009a06a0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
@@ -12018,29 +12018,29 @@
   0x009a0ef0 61742022 2f676974 6875622f 686f6d65 at "/github/home
   0x009a0f00 2f6d696e 69636f6e 64612f65 6e76732f /miniconda/envs/
   0x009a0f10 6275696c 645f6269 6e617279 2f6c6962 build_binary/lib
   0x009a0f20 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
   0x009a0f30 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x009a0f40 6e636c75 64652f41 54656e2f 636f7265 nclude/ATen/core
   0x009a0f50 2f697661 6c75655f 696e6c2e 68223a32 /ivalue_inl.h":2
-  0x009a0f60 3035312c 20706c65 61736520 7265706f 051, please repo
+  0x009a0f60 3035342c 20706c65 61736520 7265706f 054, please repo
   0x009a0f70 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x009a0f80 7263682e 20004578 70656374 65642054 rch. .Expected T
   0x009a0f90 656e736f 724c6973 74206275 7420676f ensorList but go
   0x009a0fa0 74200074 6f54656e 736f724c 69737400 t .toTensorList.
   0x009a0fb0 69735465 6e736f72 4c697374 28292049 isTensorList() I
   0x009a0fc0 4e544552 4e414c20 41535345 52542046 NTERNAL ASSERT F
   0x009a0fd0 41494c45 44206174 20222f67 69746875 AILED at "/githu
   0x009a0fe0 622f686f 6d652f6d 696e6963 6f6e6461 b/home/miniconda
   0x009a0ff0 2f656e76 732f6275 696c645f 62696e61 /envs/build_bina
   0x009a1000 72792f6c 69622f70 7974686f 6e332e39 ry/lib/python3.9
   0x009a1010 2f736974 652d7061 636b6167 65732f74 /site-packages/t
   0x009a1020 6f726368 2f696e63 6c756465 2f415465 orch/include/ATe
   0x009a1030 6e2f636f 72652f69 76616c75 655f696e n/core/ivalue_in
-  0x009a1040 6c2e6822 3a323032 332c2070 6c656173 l.h":2023, pleas
+  0x009a1040 6c2e6822 3a323032 362c2070 6c656173 l.h":2026, pleas
   0x009a1050 65207265 706f7274 20612062 75672074 e report a bug t
   0x009a1060 6f205079 546f7263 682e2000 00000000 o PyTorch. .....
   0x009a1070 6973446f 75626c65 28292049 4e544552 isDouble() INTER
   0x009a1080 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x009a1090 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x009a10a0 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x009a10b0 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
@@ -12055,28 +12055,28 @@
   0x009a1140 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x009a1150 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x009a1160 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x009a1170 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
   0x009a1180 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x009a1190 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x009a11a0 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
-  0x009a11b0 75655f69 6e6c2e68 223a3139 34372c20 ue_inl.h":1947, 
+  0x009a11b0 75655f69 6e6c2e68 223a3139 35302c20 ue_inl.h":1950, 
   0x009a11c0 706c6561 73652072 65706f72 74206120 please report a 
   0x009a11d0 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x009a11e0 00000000 00000000 69735465 6e736f72 ........isTensor
   0x009a11f0 4c697374 28292049 4e544552 4e414c20 List() INTERNAL 
   0x009a1200 41535345 52542046 41494c45 44206174 ASSERT FAILED at
   0x009a1210 20222f67 69746875 622f686f 6d652f6d  "/github/home/m
   0x009a1220 696e6963 6f6e6461 2f656e76 732f6275 iniconda/envs/bu
   0x009a1230 696c645f 62696e61 72792f6c 69622f70 ild_binary/lib/p
   0x009a1240 7974686f 6e332e39 2f736974 652d7061 ython3.9/site-pa
   0x009a1250 636b6167 65732f74 6f726368 2f696e63 ckages/torch/inc
   0x009a1260 6c756465 2f415465 6e2f636f 72652f69 lude/ATen/core/i
-  0x009a1270 76616c75 655f696e 6c2e6822 3a323031 value_inl.h":201
-  0x009a1280 392c2070 6c656173 65207265 706f7274 9, please report
+  0x009a1270 76616c75 655f696e 6c2e6822 3a323032 value_inl.h":202
+  0x009a1280 322c2070 6c656173 65207265 706f7274 2, please report
   0x009a1290 20612062 75672074 6f205079 546f7263  a bug to PyTorc
   0x009a12a0 682e2000 746f446f 75626c65 00000000 h. .toDouble....
   0x009a12b0 69735379 6d496e74 2829207c 7c206973 isSymInt() || is
   0x009a12c0 496e7428 2920494e 5445524e 414c2041 Int() INTERNAL A
   0x009a12d0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x009a12e0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x009a12f0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
@@ -16221,15 +16221,15 @@
   0x009b15a0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x009b15b0 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x009b15c0 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x009b15d0 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
   0x009b15e0 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x009b15f0 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x009b1600 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
-  0x009b1610 75655f69 6e6c2e68 223a3139 35352c20 ue_inl.h":1955, 
+  0x009b1610 75655f69 6e6c2e68 223a3139 35382c20 ue_inl.h":1958, 
   0x009b1620 706c6561 73652072 65706f72 74206120 please report a 
   0x009b1630 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x009b1640 00746f49 6e745665 63746f72 00000000 .toIntVector....
   0x009b1650 62617463 685f696e 6465785f 73656c65 batch_index_sele
   0x009b1660 63745f64 696d3028 20202020 54656e73 ct_dim0(    Tens
   0x009b1670 6f722069 6e707574 732c2020 20205465 or inputs,    Te
   0x009b1680 6e736f72 20696e64 69636573 2c202020 nsor indices,
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.8.7
+Version: 2023.8.8
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 fbgemm_gpu/__init__.py,sha256=hyPNE6QvlwUNM4PlyfKee7j7agkOF2SNoT3EQXJ-pe0,567
 fbgemm_gpu/_fbgemm_gpu_docs.py,sha256=ks59ZF1sbng7P2uhG_taag5310ml9N_y4jU0EDsUhXs,14920
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=rc49BZwtZuu8qsO5MENAlHeswgPUn35aM8Cgr3XtBE0,2747
 fbgemm_gpu/enums.py,sha256=Tg1pBJrcfSIWmWec2WCZkRuMwmCnepKrcACi3ZijZmk,818
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=Acg6pAh9MEI2xBIKgwnFnLjUUrds4Z7SE0kvYCGIZiI,10915464
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=wDw1zBpGexM2mENXI47Xy3otpoN7Kho0BC6MXyiIz1U,10915464
 fbgemm_gpu/metrics.py,sha256=e5VnTatZjFqcgOfipH7Eqk5lsAkuxY2qsbil3Csy_yk,5648
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=n80gTkNwSA9k0dvJeZhVjzXC08c74o0G-u4MnKs7rek,2339
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=5i6X51URDXoUQnxa1EvQdQ0WMhh_4dq4vsLozDiNmQQ,2737
 fbgemm_gpu/quantize_comm.py,sha256=qONCevOTVA89K7vFJe-Bcc903lHsKDg6s661pTHCF2k,7682
 fbgemm_gpu/quantize_utils.py,sha256=pnZCkIeYxPnvwkIVsRdfPeGBLVXSpEdSsFLH2Ygk7D0,4005
 fbgemm_gpu/split_embedding_configs.py,sha256=Y3fJLHh4ffO6v_iKGc2MbBQTu8yFIMExEG_VYNW7rzI,5745
 fbgemm_gpu/split_embedding_inference_converter.py,sha256=z1NugAsdcLO4nVFa_DJlOZHahmEdrBELi15ywFdaP3U,6661
@@ -31,11 +31,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=ToqlGd9bLtY0OtUZr7JnaujeLgIcI2mAoCcPeaMVn1s,4320
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=PVePhoU52wiFE_1gdZezHBiqsjiwJjzn2JBLEW3X2uk,6067
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=lUEZjp4C3HxSizRXKr47gAV1hgBtGqENVSFqNo5NtA0,2768
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=2U09t7mznAY-6HosMRX5kqplVO-HETHt4gKI26jjQXs,4602
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=wv_Sdrifrrcw2hsgRwNCGsma6roIU5hXiEzpct4bmrc,3658
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=I6xnQ0vv6PZCxMsR87fWvb1Qtkp7ehx1b-9-La1vW2U,635
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=soARoBsdOnNNZdCIkVmryPHtKyhbcFLqHOTveG-hk6s,6136
-fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/METADATA,sha256=sIScrxDCkbDRY3U8Q7eEoA_oFK3t5F2Si7VUaK8THxI,2933
-fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/WHEEL,sha256=uNTrmykJsfnOiRowEmEAgdbSsr7BScgAFZq1d9YxSqA,105
-fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.8.7.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/METADATA,sha256=8YfPzWbRubKBpgAzAFO7rVCuMh_mC1EZZ4IG0HUto38,2933
+fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/WHEEL,sha256=uNTrmykJsfnOiRowEmEAgdbSsr7BScgAFZq1d9YxSqA,105
+fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.8.8.dist-info/RECORD,,
```

