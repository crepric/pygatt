py_test(
  name = "device_test",
  srcs = ["test_device.py"],
  main = "test_device.py",
  deps = [
      "//pygatt:exceptions_lib",
      "//pygatt/backends:backend_lib",
      "//pygatt/backends/gatttool:device_lib",
  ]
)

py_test(
  name = "backend_test",
  srcs = ["test_backend.py"],
  main = "test_backend.py",
  deps = [
      "//pygatt/backends/gatttool:gatttool_lib",
  ]
)
