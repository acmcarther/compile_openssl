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
    name = "secur32_sys_build_script",
    srcs = glob(["*", "**/*.rs"]),
    crate_root = "build.rs",
    deps = [
      "//cargo/vendor/winapi-build-0.1.1:winapi_build",
    ]
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu"
    ],
    
    visibility = ["//visibility:private"],
)

genrule(
    name = "secur32_sys_build_script_executor",
    srcs = glob(["*", "**/*.rs"]),
    outs = ["secur32_sys_out_dir_outputs.tar.gz"],
    tools = [":secur32_sys_build_script"],
    cmd = "mkdir secur32_sys_out_dir_outputs/;"
        + " (export CARGO_MANIFEST_DIR=\"$$PWDcargo/vendor/secur32-sys-0.2.0\";"
        + " export TARGET='x86_64-unknown-linux-gnu';"
        + " export RUST_BACKTRACE=1;"
        + " export OUT_DIR=$$PWD/secur32_sys_out_dir_outputs;"
        + " export BINARY_PATH=\"$$PWD/$(location :secur32_sys_build_script\";"
        + " export OUT_TAR=$$PWD/$@;"
        + " cd $$(dirname $(location :Cargo.toml)) && $$BINARY_PATH && tar -czf $$OUT_TAR -C $$OUT_DIR .)"
)
alias(
  name = "secur32_sys",
  actual = ":secur32",
)

rust_library(
    name = "secur32",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/winapi-0.2.8:winapi",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
)
