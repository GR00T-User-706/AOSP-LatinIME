# AOSP Android Keyboard (LatinIME)

> [![basic-merchandising](https://i.imgur.com/KceuOBP.png)](https://github.com/leopq)

![license](https://img.shields.io/npm/l/express?color=%237429f7&style=for-the-badge) ![stars](https://img.shields.io/symfony/i/stars/15c5c748-f8d8-4b56-b536-a29a151aac6c?color=%237429f7&style=for-the-badge) ![vulnerabilities](https://img.shields.io/snyk/vulnerabilities/npm/npm?color=%237429f7&style=for-the-badge)

Develop Android LatinIME in Android Studio without a need to download and build whole Android Open Source Project.

> Currently building LatinIME requires downloading and building whole Android sources.
> This requires tens of gigabytes of disk space and takes couple hours to complete.
> The aim of this project is to allow development of LatingIME using Android Studio, Android SDK and NDK.

## 🚦 Current status

This is still a work in progress. Currently building the Java part of the app works fine
but you still need to build native libraries separately or extract them from existing APK.
Building host tools (used to generate dictionaries) still requires some more work.

## 🖖 How to build LatinIME APK

1.  Checkout this build configuration:

        git clone https://github.com/leonardoquevedox/AOSP-LatinIME.git .

1.  Checkout LatinIME sources to `LatinIME` subdirectory:

           git clone https://github.com/LineageOS/android_packages_inputmethods_LatinIME.git LatinIME

1.  Import project into `Android Studio`

### 🎉 Enjoy your new Android Keyboard!

## Project standards

See [PROJECT_STANDARDS.md](docs/PROJECT_STANDARDS.md) for project-specific documentation, contribution, and validation standards.
