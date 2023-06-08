# React Native Camera

The comprehensive camera module for React Native.

Supports:

- photographs.
- videos
- face detection (Android & iOS only)
- barcode scanning
- text recognition (optional installation for iOS using CocoaPods)

### Example import

```jsx
import { RNCamera, FaceDetector } from 'react-native-camera';
```

#### How to use master branch?

We recommend using the releases from npm, however if you need some features that are not published on npm yet you can install react-native-camera from git.

**yarn**: `yarn add react-native-camera@git+https://git@github.com/jambobrian/react-native-camera.git`

##### Permissions

To use the camera,

1. On Android you must ask for camera permission:

```java
  <uses-permission android:name="android.permission.CAMERA" />
```

To enable `video recording` feature you have to add the following code to the `AndroidManifest.xml`:

```java
  <uses-permission android:name="android.permission.RECORD_AUDIO"/>
  <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
  <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
```

2. On iOS, you must update Info.plist with a usage description for camera

```xml
...
<key>NSCameraUsageDescription</key>
<string>Your own description of the purpose</string>
...
```
