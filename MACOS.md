# Dhee Studio macOS Installation

The current macOS app is not notarized yet. Because of that, macOS may block the app or show a warning such as "`Dhee` is damaged and can't be opened." If you downloaded Dhee Studio from the official website, follow the steps below to install it and remove the quarantine flag.

[Download Dhee Studio](https://dhee.studio/)

## 1. Open the downloaded DMG

After downloading Dhee Studio, open Finder, go to your Downloads folder, and double-click the `Dhee-mac-arm64.dmg` file.

![Dhee Studio DMG in the macOS Downloads folder](mac-terminal/Step-1.png)

## 2. Move Dhee to Applications

Drag the **Dhee** app icon into the **Applications** folder.

![Dhee app copied from the DMG to Applications](mac-terminal/Step-2.png)

## 3. Try opening Dhee

In Finder, open the Applications folder. Hold **Control** while clicking **Dhee**, then choose **Open** from the context menu. If macOS shows a security dialog, click **Open**.

If Dhee opens successfully, you can skip the terminal steps below.

## 4. If macOS says Dhee is damaged, open Terminal

If macOS shows "`Dhee` is damaged and can't be opened," do not move it to Trash. Open the macOS Terminal app and enter this command:

```bash
sudo xattr -dr com.apple.quarantine "/Applications/Dhee.app"
```

![macOS damaged app warning for Dhee](mac-terminal/Warning.png)

![Terminal command to remove the Dhee quarantine flag](mac-terminal/Step-3.png)

## 5. Enter your Mac password

Press **Return**. Terminal may ask for your Mac password. Type your password and press **Return** again.

Terminal does not show password characters while you type. This is normal.

![Terminal password prompt for the quarantine command](mac-terminal/Step-4.png)

## 6. Launch Dhee Studio

After the command finishes, open Dhee from the Applications folder.

![Dhee Studio landing screen](mac-terminal/image.png)
