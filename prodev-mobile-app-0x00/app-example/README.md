# First Mobile Application with Expo Router

## Objective

The goal of this task was to set up a first mobile application using the **Expo Router template**, run it on a physical device using Expo Go, and understand the basic file structure of a React Native application scaffolded with Expo.

---

## Project Setup

**Repository:** `prodev-mobile-setup`
**Directory:** `prodev-mobile-app-0x00`
**Example App Folder:** `app-example`

---

## Steps Followed

### 1. Navigate to Project Directory

Opened the terminal and navigated to the parent project directory:

```bash
cd prodev-mobile-setup
```

---

### 2. Scaffold Expo Router Application

Initialized a new Expo project using the latest Expo Router (Tabs) template:

```bash
npx create-expo-app@latest app-example
```

During setup, the **Expo Router (Tabs)** template was selected. This created the initial project structure and installed required dependencies.

---

### 3. Understanding the File Structure

Key folders and files generated:

* **app/**: Contains all application routes using file-based routing

  * **(tabs)/index.tsx**: Home screen of the application
  * **_layout.tsx**: Controls navigation layout
* **constants/Colors.tsx**: Centralized color definitions for consistent styling
* **package.json**: Project dependencies and scripts
* **node_modules/**: Installed packages (not edited manually)

Expo Router uses the folder and file structure inside `app/` to define navigation automatically.

---

### 4. Modify the Home Screen

Opened the home screen file:

```
app/(tabs)/index.tsx
```

Changed the default text from:

```
Welcome!
```

To:

```
First App Created
```

---

### 5. Run and Test the Application

Started the Expo development server:

```bash
npx expo start
```

* A QR code was generated in the terminal/browser
* The QR code was scanned using **Expo Go** on a physical device
* The application launched successfully and displayed **First App Created** on the screen

---

### 6. Reset the Project

Ran the reset command:

```bash
npm run reset-project
```

#### Observations from reset-project:

* Cleared the Metro bundler cache
* Restarted the development server
* Forced a clean rebuild of the app
* The application reloaded on the device
* **Source code changes were preserved** ("First App Created" remained unchanged)

This command is useful for fixing caching issues and unexpected runtime behavior.

---

## Final Outcome

* Expo Router app successfully scaffolded
* File-based routing structure understood
* Application ran correctly on a physical device
* Project reset behavior observed and documented

The development environment is now ready for further React Native and Expo-based projects.
