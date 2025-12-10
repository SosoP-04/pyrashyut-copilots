# Pyrashyut Copilots - App Installation Guide (Mac)

This guide is designed to help you run the Copilots prototype on your Mac and test it on your iPhone.

## Prerequisites
Ensure you have **Node.js** and **Git** installed.

## Part 1: Fix Previous Permission Errors
Based on your previous logs, there were permission issues with your system folders. Open your **Terminal** app and run these two commands one by one. You may be asked for your Mac password (it won't show on screen while typing, just type it and hit Enter).

```bash
sudo rm -rf ~/.npm/_cacache
sudo chown -R $(whoami) ~/.npm
```

## Part 2: Running the App
## 1. Download the Code
Clone the repository or download the ZIP file I sent you.

## 2. Navigate into the Folder (Crucial Step)
Your previous error (ENOENT: no such file package.json) happened because the terminal wasn't looking inside the project folder.

1.Open Terminal.
2.Type cd (type cd followed by a space).
3.Drag and drop the pyrashyut-copilots folder from your Finder window directly into the Terminal window.
4.Press Enter.

Your terminal prompt should now look like jaredburke@Mac pyrashyut-copilots %.

## 3. Install Dependencies
Run this command to download the necessary tools for the app:

```bash
npm install
```

## 4. Start the Server
Run this command to start the development server. The -c flag clears old cache to prevent conflicts.

```bash
npx expo start -c
```

### Part 3: Viewing on iPhone
Download the Expo Go app from the App Store on your iPhone.
Ensure your iPhone and Mac are on the same Wi-Fi network.
Point your iPhone camera at the QR code shown in the Terminal.
Tap the link that pops up to open Expo Go.