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
    name = "compile_tests",
    crate_root = "tests/compile_tests.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":lazy_static",
    
    
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
    name = "lazy_static",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
)
# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "no_std",
    crate_root = "tests/no_std.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":lazy_static",
    
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "test",
    crate_root = "tests/test.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":lazy_static",
    
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
