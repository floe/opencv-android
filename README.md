# opencv-android-studio

[![Release](https://jitpack.io/v/floe/opencv-android.svg)](https://jitpack.io/#floe/opencv-android/3.3.1)
The OpenCV Java SDK for Android as a ready-to-go module for Android Studio 3.0.

## Installation
This repository has JitPack.io support, so you can integrate it directly into your Android Studio projects by following the instructions on https://jitpack.io/#floe/opencv-android/3.3.1.

*__Note__:* this is only the Java component. You will also need to install the *OpenCV Manager* app, which provides the native libraries and is either available from the Play Store (outdated) or directly as an APK from https://github.com/floe/opencv-android/tree/master/manager. A minimal sample using just the Java interface is available at https://github.com/floe/opencv-tutorial-1-camerapreview.

*__Note__:* if you want to build native code using OpenCV in your app, then you also need to download and unzip the corresponding "OpenCV Android SDK 3.3.1" from https://github.com/opencv/opencv/releases/download/3.3.1/opencv-3.3.1-android-sdk.zip and edit `app/build.gradle` to set the CMake config path to `/path/to/opencv-android-sdk-3.3.1/sdk/native/jni/`. An example project using this approach is available at https://github.com/floe/opencv-tutorial-2-mixedprocessing.

## Background

Currently, the OpenCV SDK for Android still contains all code as Eclipse projects,
which has been deprecated for a long time in favor of Android Studio.

This repository simply contains the resulting module from a clean import of the legacy Eclipse project, plus the manager APKs.

(Of course, the clean solution would be to have the OpenCV build process output Android Studio modules right away. 
But I don't have time for that. If you feel you want to tackle this, see discussion at https://github.com/opencv/opencv/issues/5003 ;-)

_Note_: I'm currently using outdated build tools in the project (`gradle:2.3.2` and `android-maven-gradle-plugin:1.5`). This is because jitpack.io doesn't yet seem to support the current gradle version 3.0.1. I'll hopefully be able to update this soon.
