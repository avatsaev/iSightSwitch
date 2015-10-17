# iSightSwitch for El Capitan 

Apple Script allows you to enable/disable iSight camera by removing read right from the drivers.

1) Diable Rootless Mode by following this tutorial: http://osxdaily.com/2015/10/05/disable-rootless-system-integrity-protection-mac-os-x/

2) Boot into OS X and execute the following command in the terminal:

```
sudo chflags norestricted "/System/Library/QuickTime/QuickTimeUSBVDCDigitizer.component/Contents/MacOS/QuickTimeUSBVDCDigitizer" "/System/Library/PrivateFrameworks/CoreMediaIOServicesPrivate.framework/Versions/A/Resources/AVC.plugin/Contents/MacOS/AVC" "/System/Library/PrivateFrameworks/CoreMediaIOServicesPrivate.framework/Versions/A/Resources/AVC.plugin/Contents/MacOS/AVC" "/System/Library/Frameworks/CoreMediaIO.framework/Versions/A/Resources/VDC.plugin/Contents/MacOS/VDC" "/Library/CoreMediaIO/Plug-Ins/DAL/AppleCamera.plugin/Contents/MacOS/AppleCamera"
```

3) Enable Rootless Mode back if needed and you can now execute the script to disable or enable the iSight camera.
