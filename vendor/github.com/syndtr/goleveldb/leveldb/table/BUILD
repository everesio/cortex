load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "reader.go",
        "table.go",
        "writer.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/golang/snappy:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/cache:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/comparer:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/errors:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/filter:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/iterator:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/opt:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/storage:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/util:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "block_test.go",
        "table_suite_test.go",
        "table_test.go",
    ],
    library = ":go_default_library",
    deps = [
        "//vendor/github.com/onsi/ginkgo:go_default_library",
        "//vendor/github.com/onsi/gomega:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/comparer:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/iterator:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/opt:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/storage:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/testutil:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/util:go_default_library",
    ],
)
