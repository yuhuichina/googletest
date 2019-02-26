# Google Test including Google Mock
cc_library(
    name = "gtest",
    incs = [
        './googletest/',
        './googletest/include/',
        './googlemock/'
        './googlemock/include/'
    ],
    export_incs = [
        './googletest/include/',
        './googlemock/include/'
    ],
    srcs = [
        'googletest/src/gtest-filepath.cc',
        'googletest/src/gtest-printers.cc',
        'googletest/src/gtest.cc',
        'googletest/src/gtest-test-part.cc',
        'googletest/src/gtest-death-test.cc',
        'googletest/src/gtest-port.cc',
        'googletest/src/gtest-typed-test.cc',
        'googlemock/src/gmock-internal-utils.cc',
        'googlemock/src/gmock-spec-builders.cc',
        'googlemock/src/gmock-cardinalities.cc',
        'googlemock/src/gmock.cc',
        'googlemock/src/gmock-matchers.cc',
        # 'googletest/src/gtest-all.cc',
        # 'googletest/src/gtest_main.cc',
        # 'googlemock/src/gmock-all.cc',
        # 'googlemock/src/gmock_main.cc'
    ],
    # srcs = glob(
    #     include = [
    #         "googletest/src/*.cc",
    #         "googletest/src/*.h",
    #         "googlemock/src/*.cc",
    #     ],
    #     exclude = [
    #         "googletest/src/gtest-all.cc",
    #         "googletest/src/gtest_main.cc",
    #         "googlemock/src/gmock-all.cc",
    #         "googlemock/src/gmock_main.cc",
    #     ],
    # ),
    # hdrs = glob([
    #     "googletest/include/gtest/*.h",
    #     "googlemock/include/gmock/*.h",
    # ]),
    # copts = select(
    #     {
    #         ":windows": [],
    #         ":windows_msvc": [],
    #         "//conditions:default": ["-pthread"],
    #     },
    # ),
    # defines = select(
    #     {
    #         ":has_absl": [
    #             "GTEST_HAS_ABSL=1",
    #         ],
    #         "//conditions:default": [],
    #     },
    # ),
    # includes = [
    #     "googlemock",
    #     "googlemock/include",
    #     "googletest",
    #     "googletest/include",
    # ],
    # linkopts = select({
    #     ":windows": [],
    #     ":windows_msvc": [],
    #     "//conditions:default": [
    #         "-pthread",
    #     ],
    # }),
    # deps = select(
    #     {
    #         ":has_absl": [
    #             "@com_google_absl//absl/debugging:failure_signal_handler",
    #             "@com_google_absl//absl/debugging:stacktrace",
    #             "@com_google_absl//absl/debugging:symbolize",
    #             "@com_google_absl//absl/strings",
    #             "@com_google_absl//absl/types:optional",
    #             "@com_google_absl//absl/types:variant",
    #         ],
    #         "//conditions:default": [],
    #     },
    # ),
)

cc_library(
    name = "gtest_main",
    srcs = [
        "googlemock/src/gmock_main.cc",
    ],
    deps = [":gtest"],
)

# The following rules build samples of how to use gTest.
# cc_library(
#     name = "gtest_sample_lib",
#     srcs = [
#         "googletest/samples/sample1.cc",
#         "googletest/samples/sample2.cc",
#         "googletest/samples/sample4.cc",
#     ],
#     # hdrs = [
#     #     "googletest/samples/prime_tables.h",
#     #     "googletest/samples/sample1.h",
#     #     "googletest/samples/sample2.h",
#     #     "googletest/samples/sample3-inl.h",
#     #     "googletest/samples/sample4.h",
#     # ],
# )
# 
# cc_test(
#     name = "gtest_samples",
#     # size = "small",
#     #All Samples except:
#     #sample9 ( main )
#     #sample10 (main and takes a command line option and needs to be separate)
#     srcs = [
#         "googletest/samples/sample1_unittest.cc",
#         "googletest/samples/sample2_unittest.cc",
#         "googletest/samples/sample3_unittest.cc",
#         "googletest/samples/sample4_unittest.cc",
#         "googletest/samples/sample5_unittest.cc",
#         "googletest/samples/sample6_unittest.cc",
#         "googletest/samples/sample7_unittest.cc",
#         "googletest/samples/sample8_unittest.cc",
#     ],
#     deps = [
#         ":gtest_sample_lib",
#         ":gtest_main",
#     ],
# )
# 
# cc_test(
#     name = "sample9_unittest",
#     # size = "small",
#     srcs = ["googletest/samples/sample9_unittest.cc"],
#     deps = [":gtest"],
# )
# 
# cc_test(
#     name = "sample10_unittest",
#     # size = "small",
#     srcs = ["googletest/samples/sample10_unittest.cc"],
#     deps = [
#         ":gtest",
#     ],
# )
