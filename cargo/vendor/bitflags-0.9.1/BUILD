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


rust_library(
    name = "bitflags",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "default",
      "example_generated",
    ],
)
# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "conflicting_trait_impls",
    crate_root = "tests/conflicting_trait_impls.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":bitflags",
    
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "default",
      "example_generated",
    ],
    visibility = ["//visibility:private"],
)
# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "external",
    crate_root = "tests/external.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":bitflags",
    
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "default",
      "example_generated",
    ],
    visibility = ["//visibility:private"],
)
# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "external_no_std",
    crate_root = "tests/external_no_std.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":bitflags",
    
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "default",
      "example_generated",
    ],
    visibility = ["//visibility:private"],
)
# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "i128_bitflags",
    crate_root = "tests/i128_bitflags.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":bitflags",
    
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "default",
      "example_generated",
    ],
    visibility = ["//visibility:private"],
)
