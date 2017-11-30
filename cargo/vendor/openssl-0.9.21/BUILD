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

# Unsupported target "mk_certs" with type "example" omitted
rust_library(
    name = "openssl",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
        "//cargo/vendor/bitflags-0.9.1:bitflags",
        "//cargo/vendor/foreign-types-0.2.1:foreign_types",
        "//cargo/vendor/lazy_static-0.2.11:lazy_static",
        "//cargo/vendor/libc-0.2.33:libc",
        "//cargo/vendor/openssl-sys-0.9.21:openssl_sys",
        
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
        "--cfg=ossl102",
        "--cfg=version=102",
        "--cfg=ossl10x",
    ],
    crate_features = [
        
    ],
)
