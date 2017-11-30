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
    name = "tokio_core",
    srcs = glob(["**/*.rs"]),
    crate_features = [
    ],
    crate_root = "src/lib.rs",
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    deps = [
        "//cargo/vendor/bytes-0.4.5:bytes",
        "//cargo/vendor/futures-0.1.17:futures",
        "//cargo/vendor/iovec-0.1.1:iovec",
        "//cargo/vendor/log-0.3.8:log",
        "//cargo/vendor/mio-0.6.11:mio",
        "//cargo/vendor/scoped-tls-0.1.0:scoped_tls",
        "//cargo/vendor/slab-0.4.0:slab",
        "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    ],
)
