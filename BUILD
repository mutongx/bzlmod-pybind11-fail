load("@pybind11_bazel//:build_defs.bzl", "pybind_extension")

pybind_extension(
    name = "example",
    srcs = ["add.cc"],
)

py_binary(
    name = "main",
    srcs = ["main.py"],
    deps = [":example.so"],
)
