load("@build_bazel_rules_swift//swift:swift.bzl", "swift_library")

swift_library(
    name = "MyLib",
    srcs = glob(["Sources/*.swift"]),
    copts = [
        "-Xcc",
        "-fmodule-map-file=Sources/Dummy.modulemap",
    ],
    data = ['Sources/Dummy.modulemap', 'Sources/Dummy-umbrella.h'],
    module_name = "MyLib",
    visibility = ["//visibility:public"],
)
