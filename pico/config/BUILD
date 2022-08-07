load("@bazel_skylib//rules:common_settings.bzl", "bool_flag", "string_flag")
load("//pico/config:defs.bzl", "BOARD_LIST")

package(default_visibility = ["@pico-sdk//:__pkg__"])

string_flag(
    name = "board",
    build_setting_default = "pico",
    values = BOARD_LIST,
)

label_flag(
    name = "double_impl",
    build_setting_default = "@pico-sdk//:pico_double_pico",
)

label_flag(
    name = "float_impl",
    build_setting_default = "@pico-sdk//:pico_float_pico",
)

bool_flag(
    name = "stdio_uart",
    build_setting_default = True,
)

bool_flag(
    name = "stdio_usb",
    build_setting_default = False,
)

bool_flag(
    name = "stdio_semihosting",
    build_setting_default = False,
)

bool_flag(
    name = "rtos_adapter_enable",
    build_setting_default = False,
)

label_flag(
    name = "rtos_adapter_header",
    build_setting_default = "@//:please-set-the-rtos_adapter_header-and-rtos_adapter_header_name-flags",
)

string_flag(
    name = "rtos_adapter_header_name",
    build_setting_default = "",
)