1:

```
INFO: Build option --define has changed, discarding analysis cache.
ERROR: /Users/emilio/Code/test/rust-bazel-image/rust/BUILD.bazel:3:12: While resolving toolchains for target //rust:bin: No matching toolchains found for types @bazel_tools//tools/cpp:toolchain_type. Maybe --incompatible_use_cc_configure_from_rules_cc has been flipped and there is no default C++ toolchain added in the WORKSPACE file? See https://github.com/bazelbuild/bazel/issues/10134 for details and migration instructions.
ERROR: Analysis of target '//rust:bin' failed; build aborted:
INFO: Elapsed time: 0.205s
INFO: 0 processes.
FAILED: Build did NOT complete successfully (0 packages loaded, 267 targets configured)
```

2:

```
ERROR: Analysis of target '//rust:bin' failed; build aborted: error loading package '@io_bazel_rules_docker//': at /private/var/tmp/_bazel_emilio/df46fc64877e15fd2a061db2455d93bd/external/bazel_gazelle/def.bzl:34:5: at /private/var/tmp/_bazel_emilio/df46fc64877e15fd2a061db2455d93bd/external/bazel_gazelle/internal/gazelle_binary.bzl:22:5: Label '@io_bazel_rules_go//go/private:rules/aspect.bzl' is invalid because '@io_bazel_rules_go//go/private/rules' is a subpackage; perhaps you meant to put the colon here: '@io_bazel_rules_go//go/private/rules:aspect.bzl'?
INFO: Elapsed time: 0.216s
INFO: 0 processes.
FAILED: Build did NOT complete successfully (2 packages loaded, 271 targets configured)
    currently loading: @io_bazel_rules_docker//
```
