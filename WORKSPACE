http_archive(
    name = "io_bazel_rules_closure",
    sha256 = "a38539c5b5c358548e75b44141b4ab637bba7c4dc02b46b1f62a96d6433f56ae",
    strip_prefix = "rules_closure-dbb96841cc0a5fb2664c37822803b06dab20c7d1",
    urls = [
        "https://mirror.bazel.build/github.com/bazelbuild/rules_closure/archive/dbb96841cc0a5fb2664c37822803b06dab20c7d1.tar.gz",
        "https://github.com/bazelbuild/rules_closure/archive/dbb96841cc0a5fb2664c37822803b06dab20c7d1.tar.gz",  # 2018-04-13
    ],
)

load("@io_bazel_rules_closure//closure:defs.bzl", "closure_repositories")

closure_repositories()

http_archive(
    name = "tensorflow",
    sha256 = "",
    strip_prefix = "tensorflow-1.12.0",
    urls = [
        "https://github.com/tensorflow/tensorflow/archive/v1.12.0.tar.gz",
    ],
)

new_http_archive(
    name = "nlohmann_json_lib",
    build_file = "nlohmann_json.BUILD",
    sha256 = "9f3549824af3ca7e9707a2503959886362801fb4926b869789d6929098a79e47",
    strip_prefix = "json-3.1.1",
    urls = [
        "https://mirror.bazel.build/github.com/nlohmann/json/archive/v3.1.1.tar.gz",
        "https://github.com/nlohmann/json/archive/v3.1.1.tar.gz",
    ],
)

new_http_archive(
    name = "ngraph",
    build_file = "ngraph.BUILD",
    sha256 = "",
    urls = [
        "https://github.com/NervanaSystems/ngraph/archive/v0.8.1.tar.gz",
    ],
)



