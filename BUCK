load(":toolchain.bzl", "cpp_local_toolchain")
load(":rules.bzl", "cpp_binary")

cpp_local_toolchain(
    name = "clang",
    command = "clang++",
    visibility = ["PUBLIC"],
)

cpp_binary(
    name = "main",
    srcs = glob(["*.cpp"]),
    headers = glob(["*.hpp"]),
    toolchain = ":clang",
    deps = [],
)
