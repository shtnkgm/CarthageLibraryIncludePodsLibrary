# CarthageLibraryIncludePodsLibrary

## What I want to do
 - sample code to create a library to distribute with "carthage"
 - this library depends on the "cocoapods" library

```
MyApplication 
↓
(depends on) 
↓
MyFramework(carthage compatible) 
↓
(depends on)
↓
SomeCocoaPodsLibrary（not carthage compatible）
```

## Current status

Run-time crash with error
```
dyld: Library not loaded: @rpath/SVProgressHUD.framework/SVProgressHUD
  Referenced from: /Users/snakagam/Library/Developer/CoreSimulator/Devices/59C69E2D-1FA4-490D-AF94-06ADE6DC4517/data/Containers/Bundle/Application/EC31680F-FD1C-49F0-B3D8-B49EA83F6188/MyApplication.app/Frameworks/MyFramework.framework/MyFramework
  Reason: image not found
```
