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
    name = "futures_cpupool",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/num_cpus-1.7.0:num_cpus",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "default",
      "futures",
      "with-deprecated",
    ],
)
# NOTE: Test may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_test(
    name = "smoke",
    crate_root = "tests/smoke.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":futures_cpupool",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/num_cpus-1.7.0:num_cpus",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "default",
      "futures",
      "with-deprecated",
    ],
    visibility = ["//visibility:private"],
)
