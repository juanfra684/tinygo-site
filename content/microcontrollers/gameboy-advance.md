---
title: "Game Boy Advance"
weight: 3
---

The [Game Boy Advance](https://en.wikipedia.org/wiki/Game_Boy_Advance) is a handheld videogame platform based on the [ARM7TDMI](http://infocenter.arm.com/help/topic/com.arm.doc.ddi0210c/DDI0210B.pdf) microcontroller.

## Interfaces

| Interface | Hardware Supported | TinyGo Support |
| --------- | ------------- | ----- |
| GPIO      | ? | ? |
| UART      | ? | ? |
| SPI      | ? | ? |
| I2C      | ? | ? |
| ADC      | ? | ? |
| PWM      | ? | ? |

## Machine Package Docs

[Documentation for the machine package for the Gameboy Advance](../machine/gameboy-advance)

## Installing dependencies

You can use a Game Boy Advance software emulator such as MGBA (https://mgba.io) to test your programs.

## Building code

Build your Game Boy Advance programs using `-target gameboy-advance` like this:

```shell
tinygo build -o main.elf -target gameboy-advance examples/gba-display
```

Then convert the ELF output file to the GBA file format by using the `arm-none-eabi-objcopy` command like this:

```shell
arm-none-eabi-objcopy -v -O binary main.elf main.gba
```

You can now use the GBA file with your emulator or flash it onto your physical hardware.

## Flashing

Information needed here...
