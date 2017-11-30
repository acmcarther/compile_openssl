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


# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "bad",
    crate_root = "tests/bad.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_tls",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/native-tls-0.1.4:native_tls",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
# NOTE: Example may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_binary(
    name = "download_rust_lang",
    crate_root = "examples/download-rust-lang.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_tls",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/native-tls-0.1.4:native_tls",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu"
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "google",
    crate_root = "tests/google.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_tls",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/native-tls-0.1.4:native_tls",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
# NOTE: Example may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_binary(
    name = "hyper_client",
    crate_root = "examples/hyper-client.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_tls",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/native-tls-0.1.4:native_tls",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu"
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
# NOTE: Example may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_binary(
    name = "hyper_server",
    crate_root = "examples/hyper-server.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_tls",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/native-tls-0.1.4:native_tls",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu"
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "smoke",
    crate_root = "tests/smoke.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_tls",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/native-tls-0.1.4:native_tls",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
rust_library(
    name = "tokio_tls",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/native-tls-0.1.4:native_tls",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
)
