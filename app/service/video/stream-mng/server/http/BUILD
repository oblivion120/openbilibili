package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "backup.go",
        "change-log.go",
        "change-src.go",
        "check-live.go",
        "clear-cache.go",
        "clear-retweet.go",
        "http.go",
        "notify.go",
        "official.go",
        "screen-shot.go",
        "stream.go",
        "stream-cut.go",
        "stream-info.go",
        "stream-mask.go",
        "stream-validate.go",
        "upstream-rtmp.go",
        "upstream-summary.go",
    ],
    importpath = "go-common/app/service/video/stream-mng/server/http",
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
    deps = [
        "//app/service/video/stream-mng/common:go_default_library",
        "//app/service/video/stream-mng/conf:go_default_library",
        "//app/service/video/stream-mng/middleware:go_default_library",
        "//app/service/video/stream-mng/model:go_default_library",
        "//app/service/video/stream-mng/service:go_default_library",
        "//library/ecode:go_default_library",
        "//library/log:go_default_library",
        "//library/net/http/blademaster:go_default_library",
        "//library/net/http/blademaster/middleware/auth:go_default_library",
        "//library/net/http/blademaster/middleware/verify:go_default_library",
        "//library/net/metadata:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
