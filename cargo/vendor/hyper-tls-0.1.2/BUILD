"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""
package(default_visibility = ["//cargo:__subpackages__"])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_library",
    "rust_binary",
    "rust_test",
    "rust_bench_test",
)


# NOTE: Example may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_binary(
    name = "client",
    crate_root = "examples/client.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":hyper_tls",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/hyper-0.11.7:hyper",
    "//cargo/vendor/native-tls-0.1.4:native_tls",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    "//cargo/vendor/tokio-tls-0.1.3:tokio_tls",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu"
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
rust_library(
    name = "hyper_tls",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/hyper-0.11.7:hyper",
    "//cargo/vendor/native-tls-0.1.4:native_tls",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    "//cargo/vendor/tokio-tls-0.1.3:tokio_tls",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
)
