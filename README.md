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
   - The screenshot must show Android Studio open in the background AND the Emulator/Physical Device (via Screen Mirror [screen copy](https://release-assets.githubusercontent.com/github-production-release-asset/111583593/340b0451-4569-4e8f-a78f-15b2d59d0cb7?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-01-31T08%3A36%3A18Z&rscd=attachment%3B+filename%3Dscrcpy-win64-v3.3.4.zip&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-01-31T07%3A35%3A26Z&ske=2026-01-31T08%3A36%3A18Z&sks=b&skv=2018-11-09&sig=yIwlW2TpwQfU8HLxSD88X%2BPT7FJ%2FHWSUUSbsl9QZIGE%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc2OTg0NTU4NiwibmJmIjoxNzY5ODQ1Mjg2LCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.oDyc7xeGwy0iaodkGZXwKHK7TTGSXEn97SCMFnK5PqA&response-content-disposition=attachment%3B%20filename%3Dscrcpy-win64-v3.3.4.zip&response-content-type=application%2Foctet-stream)) in the foreground showing your name.
   - Save this image as setup_proof.png.
   - Upload/Push setup_proof.png to the root of this repository.

**Note**: Ensure you have a .gitignore file in your project so you don't upload the build/ folders!
