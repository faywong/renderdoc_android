# renderdoc_android
关于在 Android 上使用 RenderDoc 的指南

# install dependency

```shell
export ANDROID_NDK=/home/faywong/Android/Sdk/ndk/26.1.10909125/
export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
export ANDROID_SDK=/home/faywong/Android/Sdk
sudo apt install libxcb-keysyms1 libxcb-keysyms1-dev libqt5svg5* libx11-xcb-dev
```
# how to use

![](https://imgur.com/LLL1jYh.png)

![](https://imgur.com/2eJmzzi.png)

# FAQ

## inject failed


```shell

11-18 20:27:33.524 24607 27066 I renderdoc: @6558adb500000ab2@ __rdoc_internal_android_logcat 265975145
11-18 20:27:33.572   797   797 D io_stats: !@   8,0 r 91710410 1441255500 w 18329332 148010988 d 8234146 128878760 f 0 0 iot 28782540 0 th 0 0 0 pt 0 inp 0 0 265975.192
11-18 20:27:33.572   797   797 D io_stats: !@ Write_top(KB): kworker/u16:1(21884) 84
11-18 20:27:33.625 24607 27066 I renderdoc: @6558adb500000ab3@ __rdoc_internal_android_logcat 265975246
11-18 20:27:33.727 24607 27066 I renderdoc: @6558adb500000ab4@ __rdoc_internal_android_logcat 265975348
11-18 20:27:33.828 24607 27066 I renderdoc: @6558adb500000ab5@ __rdoc_internal_android_logcat 265975449
11-18 20:27:33.930 24607 27066 I renderdoc: @6558adb500000ab6@ __rdoc_internal_android_logcat 265975550
11-18 20:27:34.032 24607 27066 I renderdoc: @6558adb600000ab7@ __rdoc_internal_android_logcat 265975652
11-18 20:27:34.133 24607 27066 I renderdoc: @6558adb600000ab8@ __rdoc_internal_android_logcat 265975753
11-18 20:27:34.194 19038 19038 E adbd    : failed to connect to socket 'localabstract:renderdoc_38920': could not connect to localabstract address 'localabstract:renderdoc_38920'
11-18 20:27:34.239 24607 27066 I renderdoc: @6558adb600000ab9@ __rdoc_internal_android_logcat 265975859
11-18 20:27:34.339 24607 27066 I renderdoc: @6558adb600000aba@ __rdoc_internal_android_logcat 265975960
11-18 20:27:34.441 24607 27066 I renderdoc: @6558adb600000abb@ __rdoc_internal_android_logcat 265976061
11-18 20:27:34.541 24607 27066 I renderdoc: @6558adb600000abc@ __rdoc_internal_android_logcat 265976162
11-18 20:27:34.644 24607 27066 I renderdoc: @6558adb600000abd@ __rdoc_internal_android_logcat 265976264
11-18 20:27:34.744 24607 27066 I renderdoc: @6558adb600000abe@ __rdoc_internal_android_logcat 265976365
11-18 20:27:34.847 24607 27066 I renderdoc: @6558adb600000abf@ __rdoc_internal_android_logcat 265976467
11-18 20:27:34.948 24607 27066 I renderdoc: @6558adb600000ac0@ __rdoc_internal_android_logcat 265976568
11-18 20:27:35.050 24607 27066 I renderdoc: @6558adb700000ac1@ __rdoc_internal_android_logcat 265976670
11-18 20:27:35.151 24607 27066 I renderdoc: @6558adb700000ac2@ __rdoc_internal_android_logcat 265976771
11-18 20:27:35.252 24607 27066 I renderdoc: @6558adb700000ac3@ __rdoc_internal_android_logcat 265976873
11-18 20:27:35.355 24607 27066 I renderdoc: @6558adb700000ac4@ __rdoc_internal_android_logcat 265976975
11-18 20:27:35.410 19038 19038 E adbd    : failed to connect to socket 'localabstract:renderdoc_38920': could not connect to localabstract address 'localabstract:renderdoc_38920'
11-18 20:27:35.457 24607 27066 I renderdoc: @6558adb700000ac5@ __rdoc_internal_android_logcat 265977077
11-18 20:27:35.557 24607 27066 I renderdoc: @6558adb700000ac6@ __rdoc_internal_android_logcat 265977178

```
