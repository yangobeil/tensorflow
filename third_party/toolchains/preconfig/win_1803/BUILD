licenses(["restricted"])

package(default_visibility = ["//visibility:public"])

java_runtime(
    name = "windows_jdk8",
    srcs = [],
    java_home = "C:/openjdk",
)

platform(
    name = "rbe_windows_1803",
    constraint_values = [
        "@bazel_tools//platforms:x86_64",
        "@bazel_tools//platforms:windows",
    ],
    remote_execution_properties = """
        properties:{
          name:"container-image"
          value:"docker://gcr.io/tensorflow-testing/tf-win-rbe@sha256:f109576c7c0c8a1783ff22b666e8923b52dbbe7933f69a1c7a7275202c304a12"
        }
        properties:{
          name: "OSFamily" value: "Windows"
        }
        """,
)

platform(
    name = "rbe_windows_1803_gpu",
    constraint_values = [
        "@bazel_tools//platforms:x86_64",
        "@bazel_tools//platforms:windows",
    ],
    remote_execution_properties = """
        properties:{
          name:"container-image"
          value:""
        }
        properties:{
          name:"sandbox"
          value:"none"
        }
        properties:{
          name: "OSFamily" value: "Windows"
        }
        """,
)
