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
    name = "smoke",
    crate_root = "tests/smoke.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tempdir",
    "//cargo/vendor/rand-0.3.18:rand",
    
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
    name = "tempdir",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/rand-0.3.18:rand",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
)
