load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "journal.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/go.etcd.io/etcd/client/pkg/v3/systemd",
    importpath = "go.etcd.io/etcd/client/pkg/v3/systemd",
    visibility = ["//visibility:public"],
)
