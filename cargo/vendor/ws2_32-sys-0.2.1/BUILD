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
    name = "ws2_32_sys_build_script",
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
    name = "ws2_32_sys_build_script_executor",
    srcs = glob(["*", "**/*.rs"]),
    outs = ["ws2_32_sys_out_dir_outputs.tar.gz"],
    tools = [":ws2_32_sys_build_script"],
    cmd = "mkdir ws2_32_sys_out_dir_outputs/;"
        + " (export CARGO_MANIFEST_DIR=\"$$PWDcargo/vendor/ws2_32-sys-0.2.1\";"
        + " export TARGET='x86_64-unknown-linux-gnu';"
        + " export RUST_BACKTRACE=1;"
        + " export OUT_DIR=$$PWD/ws2_32_sys_out_dir_outputs;"
        + " export BINARY_PATH=\"$$PWD/$(location :ws2_32_sys_build_script\";"
        + " export OUT_TAR=$$PWD/$@;"
        + " cd $$(dirname $(location :Cargo.toml)) && $$BINARY_PATH && tar -czf $$OUT_TAR -C $$OUT_DIR .)"
)
alias(
  name = "ws2_32_sys",
  actual = ":ws2_32",
)

rust_library(
    name = "ws2_32",
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
