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

rust_binary(
    name = "security_framework_sys_build_script",
    srcs = glob(["*", "**/*.rs"]),
    crate_root = "build.rs",
    deps = [
      
    ]
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu"
    ],
    crate_features = [
      "OSX_10_8",
    ],
    visibility = ["//visibility:private"],
)

genrule(
    name = "security_framework_sys_build_script_executor",
    srcs = glob(["*", "**/*.rs"]),
    outs = ["security_framework_sys_out_dir_outputs.tar.gz"],
    tools = [":security_framework_sys_build_script"],
    cmd = "mkdir security_framework_sys_out_dir_outputs/;"
        + " (export CARGO_MANIFEST_DIR=\"$$PWDcargo/vendor/security-framework-sys-0.1.16\";"
        + " export TARGET='x86_64-unknown-linux-gnu';"
        + " export RUST_BACKTRACE=1;"
        + " export OUT_DIR=$$PWD/security_framework_sys_out_dir_outputs;"
        + " export BINARY_PATH=\"$$PWD/$(location :security_framework_sys_build_script\";"
        + " export OUT_TAR=$$PWD/$@;"
        + " cd $$(dirname $(location :Cargo.toml)) && $$BINARY_PATH && tar -czf $$OUT_TAR -C $$OUT_DIR .)"
)
rust_library(
    name = "security_framework_sys",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/core-foundation-sys-0.2.3:core_foundation_sys",
    "//cargo/vendor/libc-0.2.33:libc",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      "OSX_10_8",
    ],
)
