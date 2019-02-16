#This is the build file
licenses(["notice"])  # Apache 2.0

cc_library(
    name = "ngraph_tf_headers",
    hdrs = glob(["src/*.h"]),
    visibility = ["//visibility:public"],
    deps = [
	"@ngraph//:ngraph_core"
    ]
)

cc_library(
    name = "ngraph_bridge",
    srcs = [
        #"ngraph_api.cc",
        # "src/ngraph_api.h",
        # "src/ngraph_assign_clusters.cc",
        # "src/ngraph_assign_clusters.h",
        # "src/ngraph_builder.cc",
        # "src/ngraph_builder.h",
        # "src/ngraph_capture_variables.cc",
        # "src/ngraph_capture_variables.h",
        # "src/ngraph_cluster_manager.cc",
        # "src/ngraph_cluster_manager.h",
        # "src/ngraph_conversions.h",
        # "src/ngraph_deassign_clusters.cc",
        # "src/ngraph_deassign_clusters.h",
        # "src/ngraph_encapsulate_clusters.cc",
        # "src/ngraph_encapsulate_clusters.h",
        # "src/ngraph_encapsulate_op.cc",
        # "src/ngraph_freshness_tracker.cc",
        # "src/ngraph_freshness_tracker.h",
        # "src/ngraph_mark_for_clustering.cc",
        # "src/ngraph_mark_for_clustering.h",
        # "src/ngraph_rewrite_for_tracking.cc",
        # "src/ngraph_rewrite_for_tracking.h",
        # "src/ngraph_rewrite_pass.cc",
        # "src/ngraph_tracked_variable.cc",
        # "src/ngraph_utils.cc",
        # "src/ngraph_utils.h",
        # "src/ngraph_version_utils.h",
        # "src/tf_deadness_analysis.cc",
        # "src/tf_deadness_analysis.h",
        # "src/tf_graphcycles.cc",
        # "src/tf_graphcycles.h",
        # "logging/ngraph_log.h",
        # "logging/ngraph_log.cc",
        # "logging/tf_graph_writer.h",
        # "logging/tf_graph_writer.cc",
        "src/version.cc",
    ],
    deps = [
        ":ngraph_tf_headers",
        "@org_tensorflow//tensorflow/core:protos_all_proto_text",
        "@tensorflow//tensorflow/core:framework_headers_lib",
        "@org_tensorflow//tensorflow/core:core_cpu_headers_lib",
        "@ngraph//:ngraph_core",
    ],
    copts = [
        "-I src",
        "-I logging",
        "-I external/ngraph/src",
    ],
    alwayslink = 1,
    visibility = ["//visibility:public"],
)



