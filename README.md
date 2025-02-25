
---

# BYD – Enable ADB & Install Apps  

This repository provides a step-by-step guide on how to enable ADB (Android Debug Bridge) and Wireless ADB on BYD cars running firmware versions released after 2407.  

In the latest firmware updates, BYD has disabled standard developer tools, preventing users from installing APK files. This guide will help you bypass these restrictions and sideload apps onto your vehicle's system.  

## Enabling ADB  

1. Ensure your phone is connected to the car via **Bluetooth**.  
2. Dial the following number on the car's infotainment system:  

   ```
   *#91532547#*
   ```

3. A verification menu will appear displaying your **IMEI number**.  
4. Visit the following website to generate the required password:  

   👉 [BYD ADB Unlock Tool](https://ahmada3mar.github.io/BYD/)  

5. Enter your **IMEI number** on the website.  

   ⚠ **Make sure your car’s time is synchronized with the website’s time.**  

Once ADB is enabled, you can proceed with installing an **unlocked package installer** to allow APK sideloading.  

---

## Installing the Package Installer  

1. **Download the Package Installer APK**:  

   👉 [Download PackageInstaller.apk](https://github.com/ahmada3mar/BYD/raw/refs/heads/main/PackageInstaller.apk)  

2. Connect your phone or PC to the car via ADB.  
3. Install the Package Installer using the following command:  

   ```
   adb install PackageInstaller.apk
   ```

Once installed, you will be able to install APK files via **USB** or **SD Card** without restrictions.  

---
