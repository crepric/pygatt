py_library(
    name = "pygatt_lib",
    visibility = [
      "//visibility:public",
    ],
    deps = [
      "//pygatt/backends/gatttool:gatttool_lib",
    ]
)

py_library(
    name = "device_lib",
    srcs = ["device.py"],
    visibility = [
        "//pygatt/backends/gatttool:__pkg__",
        "//tests:__pkg__",
        ],
    deps = [
      ":exceptions_lib",
    ]
)

py_library(
    name = "exceptions_lib",
    srcs = ["exceptions.py"],
    visibility = [
        "//pygatt/backends/gatttool:__pkg__",
        "//tests:__subpackages__",
    ],
    deps = []
)

py_library(
    name = "util_lib",
    srcs = ["util.py"],
    deps = []
)

