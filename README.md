works:
`USE_BAZEL_VERSION=7.0.2 bazelisk coverage ... --test_output=all`

fails with class not found for kotlin_test, unless you comment in `rules_java` in `WORKSPACE.bazel`:
`USE_BAZEL_VERSION=7.1.0rc1 bazelisk coverage ... --test_output=all`
