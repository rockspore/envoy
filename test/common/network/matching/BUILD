load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_test",
    "envoy_package",
)

licenses(["notice"])  # Apache 2

envoy_package()

envoy_cc_test(
    name = "inputs_test",
    srcs = ["inputs_test.cc"],
    deps = [
        "//source/common/http/matching:data_impl_lib",
        "//source/common/network:address_lib",
        "//source/common/network/matching:data_impl_lib",
        "//source/common/network/matching:inputs_lib",
        "//source/common/router:string_accessor_lib",
        "//test/mocks/network:network_mocks",
    ],
)

envoy_cc_test(
    name = "inputs_integration_test",
    srcs = ["inputs_integration_test.cc"],
    deps = [
        "//source/common/network:address_lib",
        "//source/common/network/matching:data_impl_lib",
        "//source/common/network/matching:inputs_lib",
        "//source/common/router:string_accessor_lib",
        "//test/common/matcher:test_utility_lib",
        "//test/mocks/matcher:matcher_mocks",
        "//test/mocks/network:network_mocks",
        "//test/mocks/server:factory_context_mocks",
    ],
)
