load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "auth_loaders.go",
        "client_config.go",
        "config.go",
        "doc.go",
        "loader.go",
        "merged_client_builder.go",
        "overrides.go",
        "validation.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/howeyc/gopass:go_default_library",
        "//vendor/github.com/imdario/mergo:go_default_library",
        "//vendor/github.com/spf13/pflag:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/api:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/api/unversioned:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/runtime:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/util/homedir:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/util/validation:go_default_library",
        "//vendor/k8s.io/client-go/1.5/rest:go_default_library",
        "//vendor/k8s.io/client-go/1.5/tools/auth:go_default_library",
        "//vendor/k8s.io/client-go/1.5/tools/clientcmd/api:go_default_library",
        "//vendor/k8s.io/client-go/1.5/tools/clientcmd/api/latest:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "client_config_test.go",
        "loader_test.go",
        "merged_client_builder_test.go",
        "validation_test.go",
    ],
    library = ":go_default_library",
    deps = [
        "//vendor/github.com/ghodss/yaml:go_default_library",
        "//vendor/github.com/imdario/mergo:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/runtime:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/client-go/1.5/rest:go_default_library",
        "//vendor/k8s.io/client-go/1.5/tools/clientcmd/api:go_default_library",
        "//vendor/k8s.io/client-go/1.5/tools/clientcmd/api/latest:go_default_library",
    ],
)
