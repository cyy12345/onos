load("//tools/build/bazel:generate_workspace.bzl", "ONOS_VERSION")

COMPILE_DEPS = CORE_DEPS + JACKSON + CLI + [
    "//incubator/api:onos-incubator-api",
]

osgi_jar_with_tests(
    test_deps = TEST_ADAPTERS,
    deps = COMPILE_DEPS,
)

onos_app(
    app_name = "org.onosproject.optical-model",
    category = "Optical",
    description = "ONOS optical information model.",
    required_apps = [],
    title = "Optical Network Model",
    url = "https://wiki.onosproject.org/x/C4m",
)
