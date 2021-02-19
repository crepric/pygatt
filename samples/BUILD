load("@rules_python//python:defs.bzl", "py_binary")

py_binary(
  name = "basic_bluez_gatttool_sample",
  srcs = ["basic_bluez_gatttool_sample.py"],
  deps = [
      "//pygatt/backends:backend_lib",
      "//pygatt/backends/gatttool:gatttool_lib",
  ]
)

py_binary(
  name = "subscribe_indicate_thermometer_sample",
  srcs = ["subscribe_indicate_thermometer_sample.py"],
  deps = [
      "//pygatt/backends/gatttool:gatttool_lib",
  ]
)
