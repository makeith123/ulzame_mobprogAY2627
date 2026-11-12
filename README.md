# ulzame_mobprog

A new Flutter project.
# Lab Activity 0A: Discussion

**1. What challenges did you encounter while installing or configuring Flutter?**
The main challenge was the incomplete Android and Windows toolchain setup. I had Flutter and VS Code working, but the Android SDK command-line tools and the Visual Studio C++ workload were not yet installed.

**2. Did you encounter any errors when running flutter doctor?**
Yes. `flutter doctor` reported issues in two categories: (a) Android toolchain: the `cmdline-tools` component was missing and the Android license status was unknown; (b) Visual Studio: the "Desktop development with C++" workload was missing, which is needed for Windows desktop apps. Flutter, Chrome, connected devices, and network resources all passed.

**3. How did you resolve installation, dependency, SDK, or device-related issues?**
Since the Android and Windows desktop issues did not affect web development, I used Chrome as my target device. The project built and ran successfully on Chrome (Hello World! screen). I have not yet installed the Android command-line tools or accepted the licenses; to fix this later I will install them through Android Studio and run `flutter doctor --android-licenses`.

**4. What did you learn about configuring a Flutter development environment?**
I learned that `flutter doctor` is the main tool for checking the setup, that its warnings only matter for the platform I actually target, and that Android development requires Android Studio, the SDK command-line tools, and accepted licenses.

**5. What practices will you follow to make future Flutter development easier?**
I will run `flutter doctor` right after installing, set up Android Studio and the `ANDROID_HOME` variable early, keep Flutter updated, read the official setup guide before troubleshooting, and keep my project folders organized.