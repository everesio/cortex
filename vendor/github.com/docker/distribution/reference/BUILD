load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "reference.go",
        "regexp.go",
    ],
    visibility = ["//visibility:public"],
    deps = ["//vendor/github.com/docker/distribution/digest:go_default_library"],
)

go_test(
    name = "go_default_test",
    srcs = [
        "reference_test.go",
        "regexp_test.go",
    ],
    library = ":go_default_library",
    deps = ["//vendor/github.com/docker/distribution/digest:go_default_library"],
)
