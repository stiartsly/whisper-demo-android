Native-Dist Structure
=====================

Here put your dependency native ffpemg distructions

## Build ffmpeg souce

You can get ffmpeg source code from the following github repository:

```
$ git clone https://github.com/stiartsly/ffmpeg.git
```

and make compilation for android arm distributions with commands

```shell
$ cd ffmepg
$ ./dist_build/android_arm.sh
```
or for armv7l ditributions

```shell
$ cd ffmpeg
$ ./dist_build/android_armv7.sh
```

## Import native ffmpeg

After finishing building native ffmepg, copy ditributions to 'native-dist' directory.

The struct of "native-dist" directory should be listed as blow:

```
|-- native-dist
   |-- include
      |-- libavcodec
      |-- libavfilter
      |-- libavformat
      |-- libavutil
      |-- libpostproc
      |-- libswresample	
      |-- libswscale
   |-- libs
      |-- armeabi
      		|-- libavcodec.a	
      		|-- libavfilter.a
      		|-- libavformat.a
      		|-- libavutil.a
      		|-- libpostproc.a
      		|-- libswresample.a
      		|-- libswscale.a
      |-- armeabi-v7a
      		|-- libavcodec.a	
      		|-- libavfilter.a
      		|-- libavformat.a
      		|-- libavutil.a
      		|-- libpostproc.a
      		|-- libswresample.a
      		|-- libswscale.a
```

Notice: Currently only support to run on Android phone, not simulator.