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
    name = "all",
    crate_root = "tests/all.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":net2",
    "//cargo/vendor/cfg-if-0.1.2:cfg_if",
    "//cargo/vendor/libc-0.2.33:libc",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "default",
      "duration",
    ],
    visibility = ["//visibility:private"],
)
rust_library(
    name = "net2",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/cfg-if-0.1.2:cfg_if",
    "//cargo/vendor/libc-0.2.33:libc",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "default",
      "duration",
    ],
)
