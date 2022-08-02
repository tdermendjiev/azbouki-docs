---
layout: default
title: Video sessions
parent: iOS
nav_order: 2
---

# Video sessions

Azbouki SDK can be used to capture video sessions from the user device along with UI events and logs.

## Requirements

### Update Info.plist

The recorded video is stored in the user's photo and video library so in order to send it to the server you need to add `NSPhotoLibraryUsageDescription` to your app's `Info.plist` file.

### Video permission

Before the recording starts the user will be prompted for a permission. If it's not granted, the recording won't start.

## Start video session

The video recording is started by this method:

```
AzboukiClient.startVideoSession(message: String?, completion: @escaping (Error?) -> Void)
```

## End video session

To end the session use this method:

```
AzboukiClient.stopVideoSession()
```

## Check recording status

You can check the recording status by calling `AzboukiClient.isRecording()`.