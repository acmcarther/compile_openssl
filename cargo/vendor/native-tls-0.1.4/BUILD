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
    name = "google_connect",
    crate_root = "examples/google-connect.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":native_tls",
    "//cargo/vendor/openssl-0.9.21:openssl",
    
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
    name = "native_tls",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/openssl-0.9.21:openssl",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
)
# NOTE: Example may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_binary(
    name = "simple_server",
    crate_root = "examples/simple-server.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":native_tls",
    "//cargo/vendor/openssl-0.9.21:openssl",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu"
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
