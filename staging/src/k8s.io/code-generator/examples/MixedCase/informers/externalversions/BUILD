load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "factory.go",
        "generic.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/k8s.io/code-generator/examples/MixedCase/informers/externalversions",
    importpath = "k8s.io/code-generator/examples/MixedCase/informers/externalversions",
    visibility = ["//visibility:public"],
    deps = [
        "//staging/src/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//staging/src/k8s.io/client-go/tools/cache:go_default_library",
        "//staging/src/k8s.io/code-generator/examples/MixedCase/apis/example/v1:go_default_library",
        "//staging/src/k8s.io/code-generator/examples/MixedCase/clientset/versioned:go_default_library",
        "//staging/src/k8s.io/code-generator/examples/MixedCase/informers/externalversions/example:go_default_library",
        "//staging/src/k8s.io/code-generator/examples/MixedCase/informers/externalversions/internalinterfaces:go_default_library",
    ],
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
        "//staging/src/k8s.io/code-generator/examples/MixedCase/informers/externalversions/example:all-srcs",
        "//staging/src/k8s.io/code-generator/examples/MixedCase/informers/externalversions/internalinterfaces:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
