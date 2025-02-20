# YOLOv8 Android App with NCNN

This Android application demonstrates real-time object detection using YOLOv8 model with NCNN framework. The app features a modern UI design and efficient performance.

## Features

- Real-time object detection using camera feed
- Support for both YOLOv8n and YOLOv8s models
- Modern Material Design UI elements
- Efficient NCNN backend for optimal performance
- Support for multiple CPU architectures (arm64-v8a, armeabi-v7a, x86, x86_64)

## Requirements

- Android Studio 
- Android SDK 
- Android NDK
- OpenCV for Android
- NCNN framework

## Setup Instructions

1. Clone the repository
2. Open the project in Android Studio
3. Sync project with Gradle files
4. Build and run the application

## Project Structure

```
app/
├── src/
│   ├── main/
│   │   ├── assets/         # YOLOv8 model files
│   │   ├── java/          # Java source code
│   │   ├── jni/           # C++ source code
│   │   └── res/           # Android resources
└── build.gradle           # Project build configuration
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- NCNN framework by Tencent
- YOLOv8 by Ultralytics
- OpenCV Mobile

## some notes
* Android ndk camera is used for best efficiency
* Crash may happen on very old devices for lacking HAL3 camera interface
* All models are manually modified to accept dynamic input shape
* Most small models run slower on GPU than on CPU, this is common
* FPS may be lower in dark environment because of longer camera exposure time

## screenshot
![](screenshot.png)

## Reference：  
https://github.com/nihui/ncnn-android-nanodet  
https://github.com/Tencent/ncnn  
https://github.com/ultralytics/assets/releases/tag/v0.0.0
