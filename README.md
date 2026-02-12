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
      <img width="894" height="608" alt="one" src="https://github.com/user-attachments/assets/dadad496-f6b6-4f24-9cdd-d6fd4bd48f4b" />

* **Name:** `MyFirstApp`
* **Package name:** `com.example.myfirstapp`
* **Language:** Kotlin
* **Build configuration language:** Kotlin DSL (`build.gradle.kts`)
<img width="940" height="611" alt="two" src="https://github.com/user-attachments/assets/f397fc95-4663-4e1d-9391-1a95f2be022b" />

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


###  Submission Requirements

#### **Phase 1: Accept the Assignment**

1. Accept the invitation link provided by your teacher.
2. Once accepted, GitHub will create a **unique repository link** for you (e.g., `https://github.com/Debre-birhan-university/lab-0-setup-yourname`). **Copy this URL.**

#### **Phase 2: Connect Android Studio to GitHub**

1. **Enable Git:** Inside Android Studio, go to the top menu: **VCS > Enable Version Control Integration** (or **Git > Create Git Repository**). Select your project folder and click **OK**.
2. **Add Remote:** * Go to **Git > Manage Remotes...**
* Click the **+** (plus) icon.
* Paste the **unique repository URL** you copied in Phase 1. Name it `origin`.


3. **Commit:** * Go to the **Commit** tab on the left (or press `Ctrl+K`).
* Check all files, write a message (e.g., "Initial Setup"), and click **Commit**.


4. **Push:** * Go to **Git > Push...** (or press `Ctrl+Shift+K`).
* If prompted, log in to your GitHub account to authorize Android Studio.



#### **Phase 3: Final Deliverables**

To successfully complete this lab, you must ensure your repository contains:

1. **The Source Code:** Your entire `MyFirstApp` project folder (pushed via Git).
2. **The Proof (Screenshot):** * Take a screenshot of your **entire desktop**.
* The screenshot **must** show Android Studio open in the background AND the Emulator or Physical Device in the foreground.
* **Tip:** If using a physical device, use [scrcpy](https://github.com/Genymobile/scrcpy/releases/tag/v3.3.4) to mirror your screen to your computer.
* The app on the screen **must** show your name.
* Save this image as `setup_proof.png`.
* **Upload/Push** this image to the root of your repository.



> [!IMPORTANT]
> **Check your .gitignore:** Ensure your project has a `.gitignore` file so you do not upload the `build/` folders. If you see hundreds of files in your "Commit" tab, your `.gitignore` is missing!
