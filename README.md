# prodev-mobile-setup# Mobile Development Setup with Expo Go

## Objective

Mobile development demands more computational resources compared to web development. To ensure a smooth development experience, this setup uses the **Expo Framework for React Native**, which simplifies mobile app development and testing by allowing applications to run directly on a physical device.

## Prerequisites

Before starting, the following tools were required:

* **Node.js (LTS)** installed
* **VS Code** as the development environment
* A compatible operating system (Windows, macOS, or Linux)
* A physical **Android or iOS device** with internet access
* **Expo Go** installed on the mobile device

These tools are essential for efficiently completing mobile development projects.

---

## Why Expo Go?

Unlike web development, mobile development typically relies on emulators, which can be resource-intensive and require frequent updates to match new device models.

**Expo Go** provides a cost-effective and efficient alternative by:

* Allowing apps to run directly on a physical device
* Supporting both Android and iOS
* Eliminating the need for heavy emulators

---

## Setup Process

### Step 1: Verify Node.js Installation

On the computer terminal, the following commands were run:

```bash
node -v
npm -v
```

Both commands returned version numbers, confirming that Node.js and npm were installed correctly.

---

### Step 2: Install Expo Go on Mobile Device

1. Visited the Expo Go website: [https://expo.dev/go](https://expo.dev/go)
2. Selected the latest SDK version
3. Installed Expo Go:

   * Android: Google Play Store
   * iOS: Apple App Store
4. Opened the Expo Go app
5. Created an Expo account and logged in successfully

---

### Step 3: Create and Run a Test Expo Project

1. Installed Expo CLI globally (legacy CLI):

```bash
npm install -g expo-cli
```

2. Created a test project:

```bash
expo init MyTestApp
cd MyTestApp
```

3. Installed project dependencies:

```bash
npm install
```

4. Started the development server using the recommended local CLI:

```bash
npx expo start
```

5. A QR code was displayed in the browser.
6. Opened **Expo Go** on the mobile device and scanned the QR code.
7. The test application launched successfully on the phone.

---

## Challenges Faced and Solutions

### 1. Expo Login Issues

* Initial login attempts inside the Expo Go app failed.
* **Solution:** Created the account directly from the Expo website and then logged in via the app.

### 2. Deprecated Expo CLI Warnings

* Warnings appeared indicating that the global `expo-cli` is deprecated and does not fully support newer Node versions.
* **Solution:** Used the recommended local Expo CLI via:

```bash
npx expo start
```

This resolved compatibility and dependency issues.

### 3. Missing React Native Dependencies Error

* An error appeared indicating missing `@react-native-community/cli-server-api`.
* **Solution:** Ensured commands were run in the correct project directory and reinstalled dependencies using `npm install`.

---

## Final Status

* [x] Node.js installed and verified
* [x] Expo Go installed on physical device
* [x] Expo account created and logged in
* [x] Expo project successfully running on mobile device

The mobile development environment is now fully set up and ready for upcoming React Native projects.

---

**Repository:** `prodev-mobile-setup`
**Directory:** `mobile-development-setup`
**File:** `README.md`
