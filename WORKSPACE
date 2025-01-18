load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

# Load the Bazel Apple rules
http_archive(
    name = "build_bazel_rules_apple",
    url = "https://github.com/bazelbuild/rules_apple/releases/download/0.33.0/rules_apple.0.33.0.tar.gz",
    sha256 = "86025f64d723a66438787d089bea4a7bc387877229f927dcb72ee26a8db96917",
)

load("@build_bazel_rules_apple//apple:repositories.bzl", "apple_rules_dependencies", "apple_rules_toolchains")

apple_rules_dependencies()

apple_rules_toolchains()

# Swift rules
http_archive(
    name = "build_bazel_rules_swift",
    url = "https://github.com/bazelbuild/rules_swift/releases/download/0.34.0/rules_swift.0.34.0.tar.gz",
    sha256 = "9919ed1d8dae509645bfd380537ae6501528d8de971caebed6d5185b9970dc4d",
)

load("@build_bazel_rules_swift//swift:swift.bzl", "swift_rules_dependencies")

swift_rules_dependencies()