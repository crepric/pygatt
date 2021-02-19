workspace(name = "pygatt")

# load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

# Dependencies for MyPy Python Static Type Checker

# mypy_integration_version = "0.1.0" # latest @ November 15th 2020
# 
# http_archive(
#     name = "mypy_integration",
#     sha256 = "511ca642294129b7abebf6afd48aa63e7d91de3ec5fa0689d60d1dc6a94a7d1a",
#     strip_prefix = "bazel-mypy-integration-{version}".format(version = mypy_integration_version),
#     url = "https://github.com/thundergolfer/bazel-mypy-integration/archive/{version}.tar.gz".format(
#         version = mypy_integration_version,
#     ),
# )
# 
# load(
#     "@mypy_integration//repositories:repositories.bzl",
#     mypy_integration_repositories = "repositories",
# )
# mypy_integration_repositories()
# 
# load("@mypy_integration//:config.bzl", "mypy_configuration")
# # Optionally pass a MyPy config file, otherwise pass no argument.
# mypy_configuration("//bazel_helpers:mypy.ini")
# 
# load("@mypy_integration//repositories:deps.bzl", mypy_integration_deps = "deps")
# 
# mypy_integration_deps(
#     mypy_requirements_file="//bazel_helpers:mypy_version.txt",
# )

# Python Deps
#http_archive(
#    name = "rules_python",
#    sha256 = "b5668cde8bb6e3515057ef465a35ad712214962f0b3a314e551204266c7be90c",
#    strip_prefix = "rules_python-0.0.2",
#    url = "https://github.com/bazelbuild/rules_python/releases/download/0.0.2/rules_python-0.0.2.tar.gz",
#)

rules_python_version = "5c948dcfd4ca79c2ed3a87636c46abba9f5836e9"

http_archive(
    name = "rules_python",
    sha256 = "76e817a5e540f4c8a8b5e1de1e7afee6dfa42d78112a3694244450287ac20ebb",
    strip_prefix = "rules_python-{version}".format(version = rules_python_version),
    url = "https://github.com/bazelbuild/rules_python/archive/{version}.tar.gz".format(version = rules_python_version),
)

load("@rules_python//python:repositories.bzl", "py_repositories")
py_repositories()

load("@rules_python//python:pip.bzl", "pip_repositories", "pip_import", "pip_install")


# # Dependency for GRPC, a cheap trick to import SIX which is needed
# by gflags. Simply importing SIX alone doesn't work, the compilation
# phase fails, and this is a quick wayt to fix it indirectly.
# http_archive(
#     name = "com_github_grpc_grpc",
#     sha256 = "2fcb7f1ab160d6fd3aaade64520be3e5446fc4c6fa7ba6581afdc4e26094bd81",
#     strip_prefix = "grpc-1.26.0",
#     urls = [
#         #  This version of GRPC does not compile on raspberry, the "--linkopt=-latomic"
#         #  otpion is not honored by bazel.
#         #       "https://github.com/grpc/grpc/archive/v1.30.0.tar.gz",
#         "https://github.com/grpc/grpc/archive/v1.26.0.tar.gz",
#     ],
# )
# 
# load("@com_github_grpc_grpc//bazel:grpc_deps.bzl", "grpc_deps")
# 
# grpc_deps()
# 
# #Not mentioned in official docs... mentioned here https://github.com/grpc/grpc/issues/20511
# load("@com_github_grpc_grpc//bazel:grpc_extra_deps.bzl", "grpc_extra_deps")
# 
# grpc_extra_deps()
# 
# 
# # Dependencies for Google flags and Google logging library.
# http_archive(
#     name = "com_github_gflags_gflags",
#     sha256 = "34af2f15cf7367513b352bdcd2493ab14ce43692d2dcd9dfc499492966c64dcf",
#     strip_prefix = "gflags-2.2.2",
#     urls = [
#         "https://github.com/gflags/gflags/archive/v2.2.2.tar.gz",
#     ],
# )
# 
# http_archive(
#     name = "com_github_glog_glog",
#     sha256 = "f28359aeba12f30d73d9e4711ef356dc842886968112162bc73002645139c39c",
#     strip_prefix = "glog-0.4.0",
#     urls = [
#         "https://github.com/google/glog/archive/v0.4.0.tar.gz",
#     ],
# )
# 
# bind(
#     name = "glog",
#     actual = "@com_github_glog_glog//:glog",
# )
# 
# bind(
#     name = "gflags",
#     actual = "@com_github_gflags_gflags//:gflags",
# )
# 
# http_archive(
#     name = "com_github_abseil_abseil_py",
#     sha256 = "603febc9b95a8f2979a7bdb77d2f5e4d9b30d4e0d59579f88eba67d4e4cc5462",
#     strip_prefix = "abseil-py-pypi-v0.9.0",
#     urls = [
#         "https://github.com/abseil/abseil-py/archive/pypi-v0.9.0.tar.gz",
#     ],
# )
# 
# 
