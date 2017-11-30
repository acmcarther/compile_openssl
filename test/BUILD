package(default_visibility = ["//cargo:__subpackages__"])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_binary",
)

rust_binary(
    name = "test",
    srcs = ["main.rs"],
    deps = [
        "//cargo/vendor:futures",
        "//cargo/vendor:hyper",
        "//cargo/vendor:hyper_tls",
        "//cargo/vendor:tokio_core",
    ],
)
