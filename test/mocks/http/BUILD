licenses(["notice"])  # Apache 2

load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_mock",
    "envoy_package",
)

envoy_package()

envoy_cc_mock(
    name = "http_mocks",
    srcs = ["mocks.cc"],
    hdrs = ["mocks.h"],
    deps = [
        "//include/envoy/access_log:access_log_interface",
        "//include/envoy/buffer:buffer_interface",
        "//include/envoy/event:dispatcher_interface",
        "//include/envoy/http:async_client_interface",
        "//include/envoy/http:codec_interface",
        "//include/envoy/http:conn_pool_interface",
        "//include/envoy/http:filter_interface",
        "//include/envoy/ssl:connection_interface",
        "//include/envoy/tracing:http_tracer_interface",
        "//test/mocks/event:event_mocks",
        "//test/mocks/request_info:request_info_mocks",
        "//test/mocks/router:router_mocks",
        "//test/mocks/tracing:tracing_mocks",
        "//test/mocks/upstream:host_mocks",
    ],
)
