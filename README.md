
# Chat App

## Project Description

A real-time chat application built with Flutter and Firebase.

## Prerequisites

Before running the project, ensure you have the following installed:

- Flutter SDK: [Install Flutter](https://docs.flutter.dev/get-started/install)
- Firebase CLI: [Install Firebase CLI](https://firebase.google.com/docs/cli)

## Project Structure

- `android/`: Contains the Android-specific configuration and build files.
- `ios/`: Contains the iOS-specific configuration and build files (if applicable).
- `lib/`: The main directory for the Flutter application code.
  - `main.dart`: The entry point of the application.
  - `screens/`: Contains the different screens of the app (e.g., auth, chat, splash).
  - `widgets/`: Contains reusable UI widgets used throughout the app (e.g., chat messages, message bubble, new message, user image picker).
  - `firebase_options.dart`: Contains the Firebase configuration.
- `web/`: Contains the web-specific files for deploying the app on the web.
- `functions/`: Contains the Firebase Cloud Functions used by the application.
- `test/`: Contains the tests for the application.
- `pubspec.yaml`: The Flutter project configuration file, listing dependencies and other project settings.
- `firebase.json`: Configuration file for Firebase projects, specifying project settings and resources.
- `README.md`: This file, providing an overview of the project and instructions.

## Setup Instructions

### 1. Set up Firebase

1.  **Create a Firebase Project:**
    - Go to the [Firebase Console](https://console.firebase.google.com/).
    - Click "Add project" and follow the instructions to create a new project.

2.  **Add an Android App to Your Firebase Project:**
    - In your Firebase project overview, click the Android icon to add an Android app.
    - The Android package name should match the `applicationId` in `android/app/build.gradle.kts` (e.g., `com.example.myapp`).
    - Download the `google-services.json` file and place it in the `android/app/` directory.

3.  **(Optional) Add an iOS App to Your Firebase Project:**
    - If you want to support iOS, click the iOS icon and follow similar steps to add an iOS app.
    - Download the `GoogleService-Info.plist` file (if provided, otherwise the setup may be different) and follow the specific instructions from Firebase for placing it in your Xcode project.

4.  **(Optional) Add a Web App to Your Firebase Project:**
    - If you want to deploy to the web, click the web icon and follow similar steps to add a web app.
    - The setup steps are normally presented during the app creation process, and generally involve copying provided JavaScript snippets into your `web/index.html` file.

5.  **Enable Authentication:**
    - In the Firebase Console, go to "Authentication" in the left sidebar.
    - Click "Get started" and enable the authentication methods you want to use (e.g., Email/Password, Google, etc.).

6.  **Create a Firestore Database:**
    - In the Firebase Console, go to "Firestore Database" in the left sidebar.
    - Click "Create database" and follow the prompts to create a new database. Choose "Start in test mode" for initial setup (remember to configure security rules for production).

7. **(Optional) Set up Firebase Storage:**
    - If your app uses Firebase Storage, go to "Storage" in the left sidebar.
    - Click "Get started" and follow the prompts. Choose appropriate security rules for your app.

### 2. Install Dependencies

Navigate to the project directory in your terminal and run:



A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
