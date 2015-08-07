# iSightSwitch for El Capitan 

Apple Script allows you to enable/disable iSight camera by removing read right from the drivers.

1) Diable Rootless Mode by booting into recovery mode, opening "Security Configuration" from the Utilities menu, and unchecking the box for "Enforce System Integrity Protection."

2) Boot into OS X and execute the following command in the terminal:

```
sudo chflags norestricted "/System/Library/QuickTime/QuickTimeUSBVDCDigitizer.component/Contents/MacOS/QuickTimeUSBVDCDigitizer" "/System/Library/PrivateFrameworks/CoreMediaIOServicesPrivate.framework/Versions/A/Resources/AVC.plugin/Contents/MacOS/AVC" "/System/Library/PrivateFrameworks/CoreMediaIOServicesPrivate.framework/Versions/A/Resources/AVC.plugin/Contents/MacOS/AVC" "/System/Library/Frameworks/CoreMediaIO.framework/Versions/A/Resources/VDC.plugin/Contents/MacOS/VDC" "/Library/CoreMediaIO/Plug-Ins/DAL/AppleCamera.plugin/Contents/MacOS/AppleCamera"
```

3) Enable Rootless Mode back if needed and you can now execute the script to disable or enable the iSight camera.
