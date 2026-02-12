# android_setup

##  Objective
The goal of this lab is to verify that your development environment is correctly configured. You will demonstrate that Android Studio is installed, the SDK is working, and you can successfully deploy an app to a device or emulator.

---

##  Instructions

### 1. Install Android Studio
Download and install the latest stable version of **Android Studio**
### 2. Create a New Project
* Open Android Studio and select **New Project**.
* Select the **Empty Activity** template. 
    * *Note: Do NOT select "Empty Views Activity"—we are using Jetpack Compose.*
* **Name:** `MyFirstApp`
* **Package name:** `com.example.myfirstapp`
* **Language:** Kotlin
* **Build configuration language:** Kotlin DSL (`build.gradle.kts`)

### 3. Modify the Code
You need to personalize the app so we know it’s running your specific build.
1.  Navigate to: `app/src/main/java/com/example/myfirstapp/MainActivity.kt`.
2.  Locate the `Greeting` function (usually at the bottom of the file).
3.  Change the text parameter from `"Android"` to **your full name**:

```kotlin
// Change this:
Greeting("Android")

// To this:
Greeting("Your Name Here")
```
### 4. Run the Application
- Start your Android Emulator (via Device Manager) or connect a Physical Device (with USB Debugging enabled).

- Click the green Run icon (Play button) in the top toolbar.

- Verify the app launches and displays: "Hello Your Name Here!"

### Submission Requirements
To successfully complete this lab, you must push two things to this repository:

1. The Source Code: Commit and push your entire MyFirstApp project folder.

2. The Proof (Screenshot): * Take a screenshot of your entire desktop.
   - The screenshot must show Android Studio open in the background AND the Emulator/Physical Device (via Screen Mirror you can use [screen copy](https://github.com/Genymobile/scrcpy/releases/tag/v3.3.4)) in the foreground showing your name.
   - Save this image as setup_proof.png.
   - Upload/Push setup_proof.png to the root of this repository.

**Note**: Ensure you have a .gitignore file in your project so you don't upload the build/ folders!
