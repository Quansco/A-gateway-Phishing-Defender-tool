# Notifications Module

This folder contains the React Native application for receiving phishing alerts in real-time via push notifications.

### Project Setup
1. **Ensure Development Environment is Ready**:
   - Install Node.js.
   - Install React Native CLI.
   - Install Android Studio (for Android testing) or Xcode (for iOS testing).

2. **Initialize the React Native Project**:
   - Run `npx react-native init PhishingDefenderApp`.
   - Navigate into the `PhishingDefenderApp` project.

3. **Install Firebase Packages**:
   ```bash
   npm install @react-native-firebase/app @react-native-firebase/messaging
   ```

   For iOS:
   ```bash
   cd ios && pod install && cd ..
   ```

4. **Add Firebase Configuration**:
   - Place your `google-services.json` (Android) or `GoogleService-Info.plist` (iOS) in the respective folders.

5. **Run the App Locally**:
   - For Android: `npx react-native run-android`
   - For iOS: `npx react-native run-ios`

### How It Works
- **FCM Token**: The app fetches a unique token to identify the device with Firebase.
- **Push Notifications**: Alerts from Firebase can be received in real-time, even when the app is closed.
- **Foreground Alerts**: A notification banner is displayed when the app is in use.

### Next Steps
Integrate this module with the phishing detection backend to trigger notifications.