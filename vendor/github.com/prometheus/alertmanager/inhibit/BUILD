load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["inhibit.go"],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/prometheus/alertmanager/config:go_default_library",
        "//vendor/github.com/prometheus/alertmanager/provider:go_default_library",
        "//vendor/github.com/prometheus/alertmanager/types:go_default_library",
        "//vendor/github.com/prometheus/common/log:go_default_library",
        "//vendor/github.com/prometheus/common/model:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["inhibit_test.go"],
    library = ":go_default_library",
    deps = [
        "//vendor/github.com/kylelemons/godebug/pretty:go_default_library",
        "//vendor/github.com/prometheus/alertmanager/types:go_default_library",
        "//vendor/github.com/prometheus/common/model:go_default_library",
    ],
)
