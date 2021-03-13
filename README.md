#  RPUADE

RPUADE is the UADE based player plugin for RetroPlayer.
It is just a Xcode project for building the standard uadecore executable as an universal binary for both Apple silicon and Intel-based Macs.

The UADE source tree is located in the Source/uade folder and is a Git submodule and can be checked out with the following commands:

    git submodule init
    git submodule update

There are two custom build phases:

1. "Configure UADE" runs the UADE configure script and creates the UADE Makefile.
2. "Generate CPU Emulator Sources" generates the CPU emulator source files that will then built in the standard "Compile Sources" phase.
