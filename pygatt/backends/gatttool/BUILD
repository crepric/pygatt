py_library(
    name = "device_lib",
    srcs = ["device.py"],
    visibility = [
      "//samples:__pkg__",
      "//tests:__subpackages__"
    ],
    deps = [
      "//pygatt:exceptions_lib",
      "//pygatt:device_lib"
    ]

)

py_library(
    name = "gatttool_lib",
    srcs = ["gatttool.py"],
    visibility = [
      "//samples:__pkg__",
      "//tests:__subpackages__",
      "//pygatt:__pkg__",
    ],
    deps = [
      ":device_lib",
      "//pygatt:exceptions_lib",
      "//pygatt/backends:backend_lib",
    ]
)
