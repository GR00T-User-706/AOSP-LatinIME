# AOSP LatinIME Build Project Standards

This repository provides a development/build configuration for Android's LatinIME keyboard sources. The README identifies it as a work in progress and states that Java application builds work while native libraries and host dictionary-generation tools require separate handling.

## Upstream boundaries

Keep upstream LatinIME source and this repository's build configuration clearly distinguished. Document upstream source provenance, the expected checkout location/revision, and any local modifications. Do not imply that this repository contains the complete Android Open Source Project or all upstream source code.

## Build status

Document Java, native-library, and host-tool build stages separately. State exact Android Studio, Android SDK, NDK, Gradle, JDK, and source prerequisites only when verified. Clearly label required externally built or extracted native libraries and their ABI coverage.

A successful Java build alone must not be described as a complete, installable keyboard build if required native libraries or dictionary tools are missing.

## Android input-method behavior and privacy

As a keyboard/IME, the application handles highly sensitive user input. Document permissions, input-processing boundaries, network behavior, telemetry, logging, and data retention based on the actual code. Do not make blanket privacy guarantees without implementation evidence.

## Validation

Separate Gradle configuration, Java compilation, native library build, APK assembly, APK inspection, device installation, and real input-method operation. Record Android versions and device/ABI details for physical-device tests.
