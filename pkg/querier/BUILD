load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "iterator.go",
        "querier.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//pkg/chunk:go_default_library",
        "//pkg/ingester/client:go_default_library",
        "//pkg/util:go_default_library",
        "//vendor/github.com/prometheus/common/log:go_default_library",
        "//vendor/github.com/prometheus/common/model:go_default_library",
        "//vendor/github.com/prometheus/prometheus/promql:go_default_library",
        "//vendor/github.com/prometheus/prometheus/storage/local:go_default_library",
        "//vendor/github.com/prometheus/prometheus/storage/metric:go_default_library",
        "//vendor/golang.org/x/net/context:go_default_library",
    ],
)
