# Description:
# AdaNet distributed logic.

licenses(["notice"])  # Apache 2.0

exports_files(["LICENSE"])

py_library(
    name = "distributed",
    srcs = ["__init__.py"],
    visibility = ["//adanet:__subpackages__"],
    deps = [
        ":devices",
        ":placement",
    ],
)

py_library(
    name = "devices",
    srcs = ["devices.py"],
    deps = [
    ],
)

py_test(
    name = "devices_test",
    srcs = ["devices_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":devices",
        "@absl_py//absl/testing:parameterized",
    ],
)

py_library(
    name = "placement",
    srcs = ["placement.py"],
)

py_test(
    name = "placement_test",
    srcs = ["placement_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":placement",
        "@absl_py//absl/testing:parameterized",
    ],
)
