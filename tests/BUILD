py_library(
  name = "serial_mock_lib",
  srcs = ["serial_mock.py"],
  deps = [],
)

py_test(
  name = "device_test",
  srcs = ["test_device.py"],
  main = "test_device.py",
  deps = [
      "//pygatt:device_lib",
      "//pygatt/backends:backend_lib",
  ]
)
