package(default_visibility = ["//visibility:public"])

load("//tools:defaults.bzl", "pkg_npm", "ts_library")

ts_library(
    name = "schematics-core",
    srcs = glob(
        [
            "**/*.ts",
        ],
        exclude = [
            "**/testing/**/*.ts",
            "**/*spec.ts",
        ],
    ),
    module_name = "@ngrx/effects/schematics-core",
    deps = [
        "@npm//@angular-devkit/core",
        "@npm//@angular-devkit/schematics",
        "@npm//tslib",
        "@npm//typescript",
    ],
)

pkg_npm(
    name = "npm_package",
    srcs = [],
    deps = [
        ":schematics-core",
    ],
)
