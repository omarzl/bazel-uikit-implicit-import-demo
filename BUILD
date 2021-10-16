load("@build_bazel_rules_swift//swift:swift.bzl", "swift_library")

swift_library(
    name = "MyLib",
    srcs = glob(["Sources/*.swift"]),
    copts = [
      "-import-underlying-module",
      "-Xcc",
      "-fmodule-map-file=Sources/MyLib.modulemap",
    ],
    data = ['Sources/MyLib.modulemap', 'Sources/MyLib-umbrella.h'],
    module_name = "MyLib",
    visibility = ["//visibility:public"],
)
