load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["internal.go"],
    importmap = "k8s.io/cloud-provider-gcp/vendor/google.golang.org/grpc/internal",
    importpath = "google.golang.org/grpc/internal",
    visibility = ["//vendor/google.golang.org/grpc:__subpackages__"],
    deps = [
        "//vendor/google.golang.org/grpc/connectivity:go_default_library",
        "//vendor/google.golang.org/grpc/serviceconfig:go_default_library",
    ],
)
