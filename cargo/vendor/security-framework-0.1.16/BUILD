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
    ":security_framework",
    "//cargo/vendor/core-foundation-0.2.3:core_foundation",
    "//cargo/vendor/core-foundation-sys-0.2.3:core_foundation_sys",
    "//cargo/vendor/libc-0.2.33:libc",
    "//cargo/vendor/security-framework-sys-0.1.16:security_framework_sys",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu"
    ],
    
    crate_features = [
      "OSX_10_8",
      "security-framework-sys",
    ],
    visibility = ["//visibility:private"],
)
rust_library(
    name = "security_framework",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/core-foundation-0.2.3:core_foundation",
    "//cargo/vendor/core-foundation-sys-0.2.3:core_foundation_sys",
    "//cargo/vendor/libc-0.2.33:libc",
    "//cargo/vendor/security-framework-sys-0.1.16:security_framework_sys",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "OSX_10_8",
      "security-framework-sys",
    ],
)
