[![pub package](https://img.shields.io/pub/v/gif_view.svg)](https://pub.dev/packages/gif_view)

<!-- 
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages). 

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages). 
-->
# GifView

Load GIF images and can set framerate

## Features

With `GifView` you can load GIF images of easy way and can configure frameRate.

- Load from `Assets`;
- Load from `Network`;
- Load from `Memory`;
- Set frame rate;
- Listen when start (`onStart`), change frame (`onChange`) and finish (`onFinish`) animation.
- Set `progress` while loading GIF

## Getting started

Add `gif_view` as a [dependency in your pubspec.yaml file](https://flutter.dev/using-packages/).

## Usage

### GIF from Asset

```dart
  GifView.asset(
    'assets/gif1.gif',
    height: 200,
    width: 200,
    frameRate: 30, // default is 15 FPS
  )
```


### GIF from Network

```dart
  GifView.network(
    'https://www.showmetech.com.br/wp-content/uploads/2015/09/happy-minion-gif.gif',
    height: 200,
    width: 200,
  )
```


### GIF from Memory

```dart
  GifView.memory(
    _bytes,
    height: 200,
    width: 200,
  )
```

## Atributes

| Name | Description  | Default  |
| ------- | --- | --- |
| frameRate | - | - | 
| isAnimated | - | `true` |
| invertedAnimation | - | `false` |
| loop | - | `true` |
| height | - | - | 
| width | - | - | 
| progress | - |
| fit | - | - | 
| color | - | - | 
| colorBlendMode | - | - | 
| alignment | - | `Alignment.center` |
| repeat | - |  `ImageRepeat.noRepeat` |
| centerSlice | - | - | 
| matchTextDirection | - | `false` |
| invertColors | - | `false` |
| filterQuality | - | `FilterQuality.low` |
| isAntiAlias | - | `false` |
| onFinish | - | - | 
| onStart | - | - | 
| onFrame | - | - | 
| onError | - | - | 
| scale | - | `1.0` |
| headers | - | - | 
