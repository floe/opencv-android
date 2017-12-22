# opencv-android-studio

[![Release](https://jitpack.io/v/floe/opencv-android-studio.svg)](https://jitpack.io/#floe/opencv-android)
The OpenCV SDK for Android as a ready-to-go module for Android Studio 3.0.

## Installation
This repository has JitPack.io support, so you can integrate it directly into your Android Studio projects by following the instructions on https://jitpack.io/#floe/opencv-android-studio.

_Note_: this is only the Java component. You will also need to install the *OpenCV Manager* app, which provides the native libraries and is either available from the Play Store (outdated) or directly as an APK from https://github.com/floe/opencv-android-studio/manager.

## Background

Currently, the OpenCV SDK for Android still contains all code as Eclipse projects,
which has been deprecated for a long time in favor of Android Studio.

This repository simply contains the resulting module from a clean import of the legacy Eclipse project, plus the manager APKs.

(Of course, the clean solution would be to have the OpenCV build process output Android Studio modules right away. 
But I don't have time for that ;-)

_Note_: I'm currently using outdated build tools in the project (gradle:2.3.2 and android-maven-gradle-plugin:1.5). This is because jitpack.io doesn't yet seem to support the current gradle version 3.0.1. I'll hopefully be able to update this soon.
