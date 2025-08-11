# zmk-config (MySplit)

This repo follows the official Unified ZMK Config Template structure.
Pins are just placeholders to get the build green; we'll swap them to your real pins once we confirm it compiles.

## Build locally (optional)
```
west init -l config
west update
west zephyr-export
west build -s zmk/app -b nice_nano_v2 -- -DZMK_CONFIG=./config -DSHIELD=mysplit_left
west build -t clean
west build -s zmk/app -b nice_nano_v2 -- -DZMK_CONFIG=./config -DSHIELD=mysplit_right
```
