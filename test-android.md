# Testing Accessibility in Android

To test on an Android emulator you will utilize Google Talkback APK. You would need to download this apk and drag it onto the emulator. 
Most up to date information about this feature can be found on the [React Native docs](https://facebook.github.io/react-native/docs/accessibility#testing-talkback-support-android) 

It can be rather challenging to interact with the emulator once Talkback is enabled so consider utilizing the adb commands referenced. It was found to be helpful to create an alias for your terminal that will do this for you.

```
alias talkback-on = adb shell settings put secure enabled_accessibility_services com.google.android.marvin.talkback/com.google.android.marvin.talkback.TalkBackService
alias talkback-off = adb shell settings put secure enabled_accessibility_services com.android.talkback/com.google.android.marvin.talkback.TalkBackService
```

Once you have enabled talkback you will turn up the volume and interact with your screens. You will need to double-tap in order to perform an action like a button press.

For additional Accessibility information/auditing on Android you can utilize a tool such as [Accessibility Scanner](https://play.google.com/store/apps/details?id=com.google.android.apps.accessibility.auditor) For this you will also need the apk or download it from the PlayStore on the emulator or physical device and enable it under the settings menu.