# Description:
#   Contains the legacy TF RNN APIs (internal TensorFlow version).

package(
    default_visibility = [
        "//keras:__subpackages__",
        "//third_party/tensorflow:__subpackages__",
    ],
    licenses = ["notice"],  # Apache 2.0
)

filegroup(
    name = "all_py_srcs",
    srcs = glob(["*.py"]),
    visibility = ["//keras/google/private_tf_api_test:__pkg__"],
)

py_library(
    name = "rnn_cell_impl",
    srcs = ["rnn_cell_impl.py"],
    deps = [
        ":rnn_cell_wrapper_impl",
        "//:expect_tensorflow_installed",
        "//keras:activations",
        "//keras:initializers",
        "//keras/engine:input_spec",
        "//keras/legacy_tf_layers:layers_base",
        "//keras/saving",
        "//keras/utils:tf_utils",
    ],
)

py_library(
    name = "rnn_cell_wrapper_impl",
    srcs = ["rnn_cell_wrapper_impl.py"],
    deps = [
        "//:expect_tensorflow_installed",
        "//keras/utils:generic_utils",
    ],
)
