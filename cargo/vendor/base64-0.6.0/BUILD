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
    name = "base64",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/byteorder-1.1.0:byteorder",
    "//cargo/vendor/safemem-0.2.0:safemem",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
)
# NOTE: Benchmark may not function correctly: Development dependencies will be absent
# TODO(acmcarther/cargo-raze/issues/7): Extend this with dev dependencies
rust_bench_test(
    name = "benchmarks",
    crate_root = "benches/benchmarks.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":base64",
    "//cargo/vendor/byteorder-1.1.0:byteorder",
    "//cargo/vendor/safemem-0.2.0:safemem",
    
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
    name = "make_tables",
    crate_root = "examples/make_tables.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":base64",
    "//cargo/vendor/byteorder-1.1.0:byteorder",
    "//cargo/vendor/safemem-0.2.0:safemem",
    
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
    name = "tests",
    crate_root = "tests/tests.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":base64",
    "//cargo/vendor/byteorder-1.1.0:byteorder",
    "//cargo/vendor/safemem-0.2.0:safemem",
    
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
    visibility = ["//visibility:private"],
)
