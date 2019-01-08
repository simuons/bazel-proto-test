load("@io_bazel_rules_scala//scala_proto:scala_proto.bzl", "scala_proto_srcjar", "scala_library")

proto_library(
    name = "message1_proto",
    srcs = ["message-1.proto"],
    deps = ["@com_google_protobuf//:wrappers_proto"])

proto_library(
    name = "message2_proto",
    srcs = ["message-2.proto"],
    deps = ["@com_google_protobuf//:wrappers_proto"])

java_proto_library(
    name = "message1_proto_java",
    deps = [":message1_proto"])

java_proto_library(
    name = "message2_proto_java",
    deps = [":message2_proto"])

java_library(
    name = "lib_java",
    deps = [":message1_proto_java", ":message2_proto_java", "@com_google_protobuf//:protobuf_java"])

scala_proto_srcjar(
    name = "message1_proto_scala",
    generator = "@io_bazel_rules_scala//src/scala/scripts:scalapb_generator",
    deps = [":message1_proto"])

scala_proto_srcjar(
    name = "message2_proto_scala",
    generator = "@io_bazel_rules_scala//src/scala/scripts:scalapb_generator",
    deps = [":message2_proto"])

scala_library(
    name = "lib_scala",
    srcs = [":message1_proto_scala", ":message2_proto_scala"],
    visibility = ["//visibility:public"],
    deps = [
        "@com_google_protobuf//:protobuf_java",
        "@scala_proto_rules_scalapb_lenses",
        "@scala_proto_rules_scalapb_runtime",
    ])
