load("@io_bazel_rules_scala//scala_proto:scala_proto.bzl", "scala_proto_srcjar", "scala_library")

proto_library(
    name = "a",
    srcs = ["a.proto"],
    deps = ["@com_google_protobuf//:any_proto"]
)

proto_library(
    name = "b",
    srcs = ["b.proto"],
    deps = [":a"]
)

java_proto_library(
    name = "b_java_proto",
    deps = [":b"]
)
