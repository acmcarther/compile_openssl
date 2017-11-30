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
    name = "simple_client_proto",
    crate_root = "tests/simple_client_proto.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_proto",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    "//cargo/vendor/net2-0.2.31:net2",
    "//cargo/vendor/rand-0.3.18:rand",
    "//cargo/vendor/slab-0.3.0:slab",
    "//cargo/vendor/smallvec-0.2.1:smallvec",
    "//cargo/vendor/take-0.1.0:take",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    
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
    name = "simple_framed",
    crate_root = "tests/simple_framed.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_proto",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    "//cargo/vendor/net2-0.2.31:net2",
    "//cargo/vendor/rand-0.3.18:rand",
    "//cargo/vendor/slab-0.3.0:slab",
    "//cargo/vendor/smallvec-0.2.1:smallvec",
    "//cargo/vendor/take-0.1.0:take",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    
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
    name = "test_multiplex_client",
    crate_root = "tests/test_multiplex_client.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_proto",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    "//cargo/vendor/net2-0.2.31:net2",
    "//cargo/vendor/rand-0.3.18:rand",
    "//cargo/vendor/slab-0.3.0:slab",
    "//cargo/vendor/smallvec-0.2.1:smallvec",
    "//cargo/vendor/take-0.1.0:take",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    
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
    name = "test_multiplex_deadlock",
    crate_root = "tests/test_multiplex_deadlock.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_proto",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    "//cargo/vendor/net2-0.2.31:net2",
    "//cargo/vendor/rand-0.3.18:rand",
    "//cargo/vendor/slab-0.3.0:slab",
    "//cargo/vendor/smallvec-0.2.1:smallvec",
    "//cargo/vendor/take-0.1.0:take",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    
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
    name = "test_multiplex_server",
    crate_root = "tests/test_multiplex_server.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_proto",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    "//cargo/vendor/net2-0.2.31:net2",
    "//cargo/vendor/rand-0.3.18:rand",
    "//cargo/vendor/slab-0.3.0:slab",
    "//cargo/vendor/smallvec-0.2.1:smallvec",
    "//cargo/vendor/take-0.1.0:take",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    
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
    name = "test_pipeline_client",
    crate_root = "tests/test_pipeline_client.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_proto",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    "//cargo/vendor/net2-0.2.31:net2",
    "//cargo/vendor/rand-0.3.18:rand",
    "//cargo/vendor/slab-0.3.0:slab",
    "//cargo/vendor/smallvec-0.2.1:smallvec",
    "//cargo/vendor/take-0.1.0:take",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    
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
    name = "test_pipeline_server",
    crate_root = "tests/test_pipeline_server.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    ":tokio_proto",
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    "//cargo/vendor/net2-0.2.31:net2",
    "//cargo/vendor/rand-0.3.18:rand",
    "//cargo/vendor/slab-0.3.0:slab",
    "//cargo/vendor/smallvec-0.2.1:smallvec",
    "//cargo/vendor/take-0.1.0:take",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    
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
    name = "tokio_proto",
    crate_root = "src/lib.rs",
    srcs = glob(["**/*.rs"]),
    deps = [
    "//cargo/vendor/futures-0.1.17:futures",
    "//cargo/vendor/log-0.3.8:log",
    "//cargo/vendor/net2-0.2.31:net2",
    "//cargo/vendor/rand-0.3.18:rand",
    "//cargo/vendor/slab-0.3.0:slab",
    "//cargo/vendor/smallvec-0.2.1:smallvec",
    "//cargo/vendor/take-0.1.0:take",
    "//cargo/vendor/tokio-core-0.1.10:tokio_core",
    "//cargo/vendor/tokio-io-0.1.4:tokio_io",
    "//cargo/vendor/tokio-service-0.1.0:tokio_service",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    
    crate_features = [
      
    ],
)
