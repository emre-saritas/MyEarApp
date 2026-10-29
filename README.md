# MyEarApp

The Android client for MyEar: records surrounding sound, sends it to the MyEar back-end for classification, and shows the result.

## Features

- Records audio from the microphone
- Live audio visualizer
- Sends audio to the MyEar Flask API over HTTP and displays the detected sound class

## Tech stack

- Java, Android SDK (min 16, target 30)
- Gradle 6.7.1, Android Gradle Plugin 4.2.1
- OkHttp, AudioVisualizer, AndroidX

## Getting started

Open the project in Android Studio and run the `app` configuration, or build from the command line:

```bash
./gradlew assembleDebug
```

The app needs microphone and internet permissions. The back-end URL is set in `WebManager.java`.

## Project structure

```
app/src/main/java/com/ee_ys2/myear/
├── MainActivity.java     # recording screen
├── VisualizerView.java   # audio visualizer
└── WebManager.java       # HTTP client for the back-end
```

## License

[MIT](LICENSE)
