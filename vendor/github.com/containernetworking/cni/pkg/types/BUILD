load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "args.go",
        "types.go",
    ],
    importpath = "github.com/containernetworking/cni/pkg/types",
    visibility = ["//visibility:public"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//vendor/github.com/containernetworking/cni/pkg/types/020:all-srcs",
        "//vendor/github.com/containernetworking/cni/pkg/types/current:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
