load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "funcs.go",
        "logging.go",
        "types.go",
        "types_linux.go",
        "types_nonlinux.go",
        "util_linux.go",
        "util_nonlinux.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/google.golang.org/grpc/internal/channelz",
    importpath = "google.golang.org/grpc/internal/channelz",
    visibility = ["//vendor/google.golang.org/grpc:__subpackages__"],
    deps = [
        "//vendor/google.golang.org/grpc/connectivity:go_default_library",
        "//vendor/google.golang.org/grpc/credentials:go_default_library",
        "//vendor/google.golang.org/grpc/grpclog:go_default_library",
    ] + select({
        "@io_bazel_rules_go//go/platform:android": [
            "//vendor/golang.org/x/sys/unix:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:linux": [
            "//vendor/golang.org/x/sys/unix:go_default_library",
        ],
        "//conditions:default": [],
    }),
)
