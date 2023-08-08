# Comparing `tmp/cudagrad-0.0.35.tar.gz` & `tmp/cudagrad-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.35.tar", last modified: Sun Aug  6 15:12:42 2023, max compression
+gzip compressed data, was "cudagrad-0.0.36.tar", last modified: Tue Aug  8 00:58:00 2023, max compression
```

## Comparing `cudagrad-0.0.35.tar` & `cudagrad-0.0.36.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.031106 cudagrad-0.0.35/
--rw-r--r--   0 ryan       (501) staff       (20)     1112 2023-08-02 22:59:21.000000 cudagrad-0.0.35/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)       42 2023-08-06 01:04:30.000000 cudagrad-0.0.35/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3692 2023-08-06 15:12:42.030980 cudagrad-0.0.35/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3167 2023-08-05 23:00:08.000000 cudagrad-0.0.35/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.028390 cudagrad-0.0.35/cudagrad/
--rw-r--r--   0 ryan       (501) staff       (20)      120 2023-08-06 06:30:25.000000 cudagrad-0.0.35/cudagrad/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     5678 2023-08-06 06:30:27.000000 cudagrad-0.0.35/cudagrad/mlp.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.029345 cudagrad-0.0.35/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3692 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      337 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.35/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)      984 2023-08-06 06:32:56.000000 cudagrad-0.0.35/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-08-06 15:12:42.031147 cudagrad-0.0.35/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1648 2023-08-06 06:30:00.000000 cudagrad-0.0.35/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.030147 cudagrad-0.0.35/src/
--rw-r--r--   0 ryan       (501) staff       (20)     2888 2023-08-06 06:29:45.000000 cudagrad-0.0.35/src/bindings.cpp
--rw-r--r--   0 ryan       (501) staff       (20)      254 2023-07-29 18:53:13.000000 cudagrad-0.0.35/src/ops.cu
--rw-r--r--   0 ryan       (501) staff       (20)    20914 2023-08-05 23:40:01.000000 cudagrad-0.0.35/src/tensor.hpp
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.030630 cudagrad-0.0.35/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1083 2023-08-05 19:26:40.000000 cudagrad-0.0.35/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-08 00:58:00.915352 cudagrad-0.0.36/
+-rw-r--r--   0 ryan       (501) staff       (20)     1112 2023-08-02 22:59:21.000000 cudagrad-0.0.36/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)       42 2023-08-06 01:04:30.000000 cudagrad-0.0.36/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     5484 2023-08-08 00:58:00.915242 cudagrad-0.0.36/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     4959 2023-08-06 17:13:40.000000 cudagrad-0.0.36/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-08 00:58:00.912608 cudagrad-0.0.36/cudagrad/
+-rw-r--r--   0 ryan       (501) staff       (20)      120 2023-08-07 20:34:49.000000 cudagrad-0.0.36/cudagrad/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5678 2023-08-07 22:26:27.000000 cudagrad-0.0.36/cudagrad/mlp.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-08 00:58:00.913519 cudagrad-0.0.36/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     5484 2023-08-08 00:58:00.000000 cudagrad-0.0.36/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      355 2023-08-08 00:58:00.000000 cudagrad-0.0.36/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-08-08 00:58:00.000000 cudagrad-0.0.36/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.36/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-08-08 00:58:00.000000 cudagrad-0.0.36/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-08-08 00:58:00.000000 cudagrad-0.0.36/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      984 2023-08-07 20:34:44.000000 cudagrad-0.0.36/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-08-08 00:58:00.915390 cudagrad-0.0.36/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1648 2023-08-06 06:30:00.000000 cudagrad-0.0.36/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-08 00:58:00.914293 cudagrad-0.0.36/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     3198 2023-08-07 21:12:22.000000 cudagrad-0.0.36/src/bindings.cpp
+-rw-r--r--   0 ryan       (501) staff       (20)      254 2023-07-29 18:53:13.000000 cudagrad-0.0.36/src/ops.cu
+-rw-r--r--   0 ryan       (501) staff       (20)    21635 2023-08-07 22:28:29.000000 cudagrad-0.0.36/src/tensor.hpp
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-08 00:58:00.914946 cudagrad-0.0.36/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1083 2023-08-06 16:33:32.000000 cudagrad-0.0.36/tests/test.py
+-rw-r--r--   0 ryan       (501) staff       (20)      411 2023-08-06 16:33:49.000000 cudagrad-0.0.36/tests/test_mlp.py
```

### Comparing `cudagrad-0.0.35/LICENSE` & `cudagrad-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.35/PKG-INFO` & `cudagrad-0.0.36/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: cudagrad
-Version: 0.0.35
-Summary: A small autograd engine
-Home-page: https://github.com/yrom1/cudagrad
-Author: Ryan Moore
-Author-email: Ryan Moore <ryanm.inbox@gmail.com>
-Project-URL: Homepage, https://github.com/yrom1/cudagrad
-Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # cudagrad
 
 A small autograd engine
 
 Work In Progress! TODO: CUDA operation integration and release on PyPI
 
 ## Example
@@ -60,28 +44,80 @@
 print(f.size)  # [1]
 print(a.grad)  # [143.0, 187.0, 143.0, 187.0]
 print(b.grad)  # [66.0, 66.0, 88.0, 88.0]
 ```
 
 ## Design
 
-~~The plan is to be similar to PyTorch's internals, particularily the [Variable/Tensor Merge Proposal](https://github.com/pytorch/pytorch/issues/13638) design.~~ The design is a mix of PyTorch and micrograd, with micrograd like members and PyTorch like backward classes with an `apply()` interface.
+~~The plan is to be similar to PyTorch's internals, particularily the [Variable/Tensor Merge Proposal](https://github.com/pytorch/pytorch/issues/13638) design.~~ The design is a mix of PyTorch and micrograd, with micrograd like members and PyTorch like backward classes with an `void apply(std::shared_ptr<Tensor> grad_output, std::vector<std::shared_ptr<Tensor>> grad_inputs)` interface.
 
 For simplicity, many features PyTorch has cudagrad does not, like broadcasting and views. All operations are defined only on `std::shared_ptr<Tensor>`, for now at least.
 
+### Tensor
+
+The `/cudagrad/src` folder contains the `Tensor` class written in C++ and CUDA, and it's pybind11 bindings. If you install the `cudagrad` package locally (using `python -m pip install -e .`) you will see a tensor `.so` file in the `/cudagrad/cudagrad` Python package folder, this is a normal Python package called `tensor` that you can import:
+
+```py
+$ pwd
+/Users/ryan/cudagrad/cudagrad
+$ ls
+__init__.py			mlp.py
+__pycache__			tensor.cpython-310-darwin.so
+$ python -q
+>>> from tensor import tensor
+>>> tensor
+<built-in method tensor of PyCapsule object at 0x100f81c80>
+>>> tensor([1], [42.0])
+tensor([1], [42])
+```
+
+In C++, constructors directly return an instance of the class type. However, if we want to manage the lifetime of an object using `std::shared_ptr<T>`, we typically use a factory function. In this case, the `tensor` factory function is used for creating `std::shared_ptr<Tensor>` instances in C++, but in Python, the distinction is abstracted away by the pybind11 bindings, allowing both `tensor` and `Tensor` to do the same thing.
+
+```py
+>>> from tensor import tensor, Tensor
+>>> tensor
+<built-in method tensor of PyCapsule object at 0x1015ca1f0>
+>>> Tensor
+<class 'tensor.Tensor'>
+>>> tensor([1], [42])
+tensor([1], [42])
+>>> Tensor([1], [42])
+tensor([1], [42])
+```
+
+### Neural networks
+
+To improve the `Tensor` class and it's Python bindings `cudagrad` tries to eat it's own dog food and implement the
+
+#### Multi-Layer Perceptron
+
+An MLP implementation can be found at `/cudagrad/cudagrad/mlp.py`.
+
+TODO example
+
+#### Transformer
+
+TODO
+
 ## Goals
 
 The goal of this project is to learn more about PyTorch's internals, neural networks, and C++. And some CUDA too!
 
 To do this, I'll gradually add support to cudagrad for the mathematical operations required to create the expression graph of various neural networks. The long term goals are to implement a Multilayer perceptron by the summer of 2023, and a Transformer by end of the year.
 
 > "Maybe it's a bad idea to have really big ambitions initially. Because the bigger your ambitions, the longer they're going to take to realize, and the longer you're projecting into the future, the more likely you're going to be wrong."
 >
 > [paulg @ PyCon US 2012](https://youtu.be/R9ITLdmfdLI?t=1927)
 
+## Setup
+
+- TODO: CUDA driver setup
+- TODO: CUDA toolkit setup
+- TODO: Check all system requirements met (nvcc, git, cmake, make...)
+
 ## Running tests
 
 Taking inspiration from [micrograd's tests](https://github.com/karpathy/micrograd/blob/master/test/test_engine.py), we will use [PyTorch's C++ frontend](https://pytorch.org/cppdocs/frontend.html) for high level sanity checks using GoogleTest.
 
 To run the tests use:
 
 ```sh
```

### Comparing `cudagrad-0.0.35/cudagrad/mlp.py` & `cudagrad-0.0.36/cudagrad/mlp.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.35/pyproject.toml` & `cudagrad-0.0.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=40.8.0", "wheel", "pybind11>=2.10.1", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.35"
+version = "0.0.36"
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 # TEMP while we implement mlp
 dependencies = [ "micrograd",]
 [[project.authors]]
```

### Comparing `cudagrad-0.0.35/setup.py` & `cudagrad-0.0.36/setup.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.35/src/bindings.cpp` & `cudagrad-0.0.36/src/bindings.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -39,26 +39,32 @@
     m.def("tensor", [](std::vector<int> sizes, std::vector<float> values) {
         // cast the function pointer to resolve the ambiguity
         auto func = static_cast<std::shared_ptr<cg::Tensor> (*)(std::vector<int>, std::vector<float>)>(&cg::tensor);
         return func(sizes, values);
     }, R"pbdoc(Magic tensor)pbdoc",
     py::arg("sizes"), py::arg("values"));
 
+    py::class_<cg::DataProxy>(m, "_DataProxy")
+        .def("__getitem__", &cg::DataProxy::get)
+        .def("__setitem__", &cg::DataProxy::set);
+
     // TODO(yrom1): When doing C++ bindings does repr
     //              override str when no str present?
     py::class_<cg::Tensor, std::shared_ptr<cg::Tensor>>(m, "Tensor")
         .def(py::init<std::vector<int>, std::vector<float>>())
         .def("get_shared", &cg::Tensor::get_shared)
         .def("backward", &cg::Tensor::backward)
         .def("zero_grad", &cg::Tensor::zero_grad)
         .def("sum", &cg::Tensor::sum)
         .def("relu", &cg::Tensor::relu)
-        .def_property_readonly("size", &cg::Tensor::get_size)
-        .def_property_readonly("data", &cg::Tensor::get_data)
-        .def_property_readonly("grad", &cg::Tensor::get_grad)
+        .def_property_readonly("data", &cg::Tensor::data_proxy)
+       .def("__getitem__", &cg::Tensor::get_data_at)
+        .def("__setitem__", &cg::Tensor::set_data_at)
+        .def_property_readonly("size", &cg::Tensor::get_size) // do something about this
+        .def_property_readonly("grad", &cg::Tensor::get_grad) // do something about this
         .def("graph", &cg::Tensor::graph)
         .def_static("ones", &cg::Tensor::ones)
         .def_static("zeros", &cg::Tensor::zeros)
         .def_static("explode", &cg::Tensor::explode)
         .def_static("rand", &cg::Tensor::rand)
         .def("__add__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a + b; })
         .def("__sub__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a - b; })
```

### Comparing `cudagrad-0.0.35/src/tensor.hpp` & `cudagrad-0.0.36/src/tensor.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 struct ReluBackward;
 struct MatMulBackward;
 
 struct AutoGradForward;
 struct MatMulForward;
 
 class Tensor;
+class DataProxy;
 
 std::shared_ptr<Tensor> tensor(std::initializer_list<int>,
                                std::initializer_list<float>);
 
 std::shared_ptr<Tensor> tensor(std::vector<int>, std::vector<float>);
 
 std::shared_ptr<Tensor> tensor(std::vector<int>, std::vector<float>,
@@ -116,19 +117,23 @@
         grad_fn_(std::move(other.grad_fn_)),
         op_(other.op_),
         offset_(other.offset_),
         strides_(std::move(other.strides_)) {}
 
   std::shared_ptr<Tensor> get_shared() { return this->shared_from_this(); }
 
+  DataProxy data_proxy();
+
   void backward();
   void zero_grad();
   std::shared_ptr<Tensor> sum();
   std::shared_ptr<Tensor> relu();
   std::shared_ptr<Tensor> matmul(std::shared_ptr<Tensor> other);
+  float get_data_at(int index) const;
+  void set_data_at(int index, float value);
 
   std::string repr() {
     std::ostringstream oss_s;
     for (const auto& s : size_) {
       oss_s << s << ", ";
     }
     std::string s_str = oss_s.str();
@@ -296,14 +301,35 @@
     for (int i = size_.size() - 1; i >= 0; i--) {
       strides_[i] = stride;
       stride *= size_[i];
     }
   }
 };
 
+// This helps pybind11 do __getitem__ __setitem__ on the .data member
+class DataProxy {
+public:
+    DataProxy(Tensor& tensor): parent_tensor(tensor) {}
+
+    float get(int index) const {
+        return parent_tensor.get_data_at(index);
+    }
+
+    void set(int index, float value) {
+        parent_tensor.set_data_at(index, value);
+    }
+
+private:
+    Tensor& parent_tensor;
+};
+
+DataProxy Tensor::data_proxy() {
+    return DataProxy(*this);
+}
+
 template <typename T>
 std::shared_ptr<Tensor> binaryElementwiseOperator(
     std::shared_ptr<Tensor> lhs, std::shared_ptr<Tensor> rhs,
     std::function<float(float, float)> func, char op,
     std::shared_ptr<T> backward) {
   std::vector<std::shared_ptr<Tensor>> children;
   children.push_back(lhs);
@@ -390,14 +416,22 @@
     std::vector<std::shared_ptr<Tensor>> children = {},
     std::shared_ptr<AutoGradBackward> grad_fn =
         std::make_shared<AutoGradBackward>(),
     char op = '?') {
   return std::make_shared<Tensor>(size, data, children, std::move(grad_fn), op);
 }
 
+float Tensor::get_data_at(int index) const {
+    return data_[index];
+}
+
+void Tensor::set_data_at(int index, float value) {
+    data_[index] = value;
+}
+
 struct AutoGradBackward {
   AutoGradBackward() = default;
   virtual ~AutoGradBackward() = default;
 
   virtual void apply(std::shared_ptr<Tensor> grad_output,
                      std::vector<std::shared_ptr<Tensor>> grad_inputs) = 0;
 };
```

### Comparing `cudagrad-0.0.35/tests/test.py` & `cudagrad-0.0.36/tests/test.py`

 * *Files identical despite different names*

