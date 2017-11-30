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
    name = "async_read",
    crate_root = "tests/async_read.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_io",
    "//cargo/vendor/bytes-0.4.5:bytes",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    
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
    name = "codecs",
    crate_root = "tests/codecs.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_io",
    "//cargo/vendor/bytes-0.4.5:bytes",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    
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
    name = "framed",
    crate_root = "tests/framed.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_io",
    "//cargo/vendor/bytes-0.4.5:bytes",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    
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
    name = "framed_read",
    crate_root = "tests/framed_read.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_io",
    "//cargo/vendor/bytes-0.4.5:bytes",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    
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
    name = "framed_write",
    crate_root = "tests/framed_write.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_io",
    "//cargo/vendor/bytes-0.4.5:bytes",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    
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
    name = "length_delimited",
    crate_root = "tests/length_delimited.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_io",
    "//cargo/vendor/bytes-0.4.5:bytes",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    
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
    name = "tokio_io",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/bytes-0.4.5:bytes",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
)
