licenses(["notice"])  # 3-Clause BSD

exports_files(["LICENSE"])

cc_library(
    name = "ngraph_headers",
    hdrs = glob(["src/ngraph/**/*.hpp"]),
    visibility = ["//visibility:public"],
)

cc_library(
    name = "ngraph_core",
    srcs = glob([
        "src/ngraph/*.cpp",
        "src/ngraph/autodiff/*.cpp",
        "src/ngraph/builder/*.cpp",
        "src/ngraph/descriptor/*.cpp",
        "src/ngraph/descriptor/layout/*.cpp",
        "src/ngraph/op/*.cpp",
        "src/ngraph/op/util/*.cpp",
        "src/ngraph/pattern/*.cpp",
        "src/ngraph/pattern/*.hpp",
        "src/ngraph/pass/*.cpp",
        "src/ngraph/pass/*.hpp",
        "src/ngraph/runtime/*.cpp",
        "src/ngraph/type/*.cpp",
    ]),
    deps = [
        ":ngraph_headers",
        "@nlohmann_json_lib",
    ],
    copts = [
        "-I external/ngraph/src",
        "-I external/nlohmann_json_lib/include/",
        '-D SHARED_LIB_EXT=\\".so\\"',
        '-D NGRAPH_VERSION=\\"0.8.1\\"',
    ],
    visibility = ["//visibility:public"],
    alwayslink = 1,
)
