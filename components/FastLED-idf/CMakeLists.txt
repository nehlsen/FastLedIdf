set(FastLED_srcs 
    "bitswap.cpp"
    "colorpalettes.cpp"
    "colorutils.cpp"
    "FastLED.cpp"
    "hsv2rgb.cpp"
    "lib8tion.cpp"
    "noise.cpp"
    "power_mgt.cpp"
    "wiring.cpp"
    "esp32-hal.c"
    "esp32-hal-gpio.c"
    )

set(FastLED_include_dirs "include")

idf_component_register(SRCS "${FastLED_srcs}"
                       INCLUDE_DIRS "${FastLED_include_dirs}")
