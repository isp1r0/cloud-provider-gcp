load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["httpbody.pb.go"],
    importmap = "k8s.io/cloud-provider-gcp/vendor/google.golang.org/genproto/googleapis/api/httpbody",
    importpath = "google.golang.org/genproto/googleapis/api/httpbody",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/golang/protobuf/proto:go_default_library",
        "//vendor/google.golang.org/protobuf/reflect/protoreflect:go_default_library",
        "//vendor/google.golang.org/protobuf/runtime/protoimpl:go_default_library",
        "//vendor/google.golang.org/protobuf/types/known/anypb:go_default_library",
    ],
)
