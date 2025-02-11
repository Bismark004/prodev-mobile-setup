# Table of Contents
- Steps for Scaffolding
- Observations from the reset-project Command
- File Structure
- How to Run the Project

## Steps for Scaffolding
### Navigate to Your Project Directory
Open your terminal and move to your parent project directory:
```sh
cd prodev-mobile-setup
```
### Set Up Your Project
Initialize a new Expo project using the latest Expo Router template:
```sh
npx create-expo-app@latest .
```
### Modify the Home Screen
Open the file `app/(tabs)/index.tsx` and change the default text `Welcome!` to `**First App Created**`.

### Run and Test Your Application
Start the Expo development server:
```sh
npx expo start
```
For iOS Devices: Scan the QR code in the terminal using your phone’s Camera app.

For Android Devices: Scan the QR code using the Expo Go app.

### Reset the Application
Run the reset command:
```sh
npm run reset-project
```

## Observations from the reset-project Command
When you run the `reset-project` command, the following actions occur:
- **Clearing Cache**: Temporary files and cache are cleared.
- **Reinstalling Dependencies**: All dependencies are reinstalled.
- **Resetting Metro Bundler**: The Metro Bundler is reset to resolve bundling issues.
- **Clearing Build Artifacts**: Build artifacts are removed for a fresh build.

This command is useful for resolving issues related to cached data or corrupted dependencies.

## File Structure
The project structure is as follows:
```
prodev-mobile-setup/
├── app/
│   ├── (tabs)/
│   │   ├── index.tsx
│   │   └── _layout.tsx
│   ├── _layout.tsx
│   └── index.tsx
├── assets/
│   ├── icon.png
│   └── splash.png
├── node_modules/
├── .gitignore
├── app.json
├── babel.config.js
├── package.json
├── README.md
└── tsconfig.json
```

## How to Run the Project
### Install Dependencies
Install the project dependencies:
```sh
npm install
```

### Start the Development Server
Run the Expo development server:
```sh
npx expo start
```

### Run on a Device
- **iOS**: Scan the QR code in the terminal using your phone’s Camera app.
- **Android**: Scan the QR code using the Expo Go app.

### Reset the Project (Optional)
If you encounter issues, reset the project:
```sh
npm run reset-project
```

