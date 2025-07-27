#testpage: https://klein-8kk.pages.dev

# Klein Bottle Rift — macOS No Keyboard Usage Guide

## What it is

This project traps the mouse cursor in a Klein bottle topology inside fullscreen mode with pointer lock, disables keyboard shortcuts (like refresh, dev tools), and shows a “rift” warning if you exit. Normally it needs keyboard input (like Escape or shortcuts) to interact.

---

## How to use on macOS **with no keyboard**

Since your keyboard is unavailable or disabled, you’ll rely on:

- **Mouse / Trackpad clicks and movement only**
- Optional **on-screen keyboard or alternative input devices**
- Fullscreen & pointer lock control via mouse/touch events

---

## Step-by-step usage instructions:

1. **Open the webpage** in a modern browser (Safari, Chrome, Firefox) on macOS.

2. **Enter fullscreen and pointer lock with mouse click**  
   - The page requires a **user click** to start fullscreen and lock the pointer.  
   - Simply **click anywhere on the page**.  
   - The pointer will then be trapped in Klein bottle mode.  
   - The custom glowing cursor appears and moves with your mouse/trackpad.

3. **Control cursor with mouse or trackpad movement**  
   - Move your mouse or finger on the trackpad.  
   - The cursor position will wrap with Klein bottle logic.

4. **If you accidentally “rift” out** (pointer lock lost)  
   - The page shows a red flashing background and a message.  
   - Simply **click the message or anywhere on the page** to re-enter pointer lock/fullscreen.  
   - No keyboard needed to recover.

5. **Disable keyboard shortcuts**  
   - The script blocks keyboard refresh/dev tools commands.  
   - Without a keyboard, these are naturally inaccessible.

---

## Optional: On-Screen Keyboard or Accessibility

- macOS has a built-in **On-Screen Keyboard**:  
  - Go to **System Settings > Accessibility > Keyboard > On-Screen Keyboard**  
  - This can simulate key presses if needed (e.g., Escape).

- You can also connect alternative input devices (e.g., **USB mouse**, **gamepad with mouse emulation**).

---

## Notes

- **No keyboard is strictly required** to use the Klein bottle cursor or recover pointer lock — **mouse clicks suffice**.
- Fullscreen & pointer lock APIs require a **user gesture**, so clicks/taps are necessary.
- If you want to **trigger Escape or other keys without keyboard**, consider adding UI buttons or gestures in the webpage.

---

## Troubleshooting

| Issue                        | Fix/Workaround                                     |
|-----------------------------|---------------------------------------------------|
| Cannot enter fullscreen      | Make sure to click on the page; browsers block auto fullscreen without gesture. |
| Pointer lock lost unexpectedly | Click the page again to re-enter pointer lock.  |
| Mouse movement not working   | Ensure no external mouse driver conflicts; trackpad should work by default. |
| Want to exit fullscreen      | Use mouse menu bar or `Cmd+Control+F` shortcut (may require keyboard). |

---

## Running in Kiosk Mode on macOS with Google Chrome

To run the Klein Bottle Rift webpage in a **locked fullscreen kiosk mode** using Google Chrome on macOS, follow these steps:

### Step 1: Locate Your HTML File

Make sure your `index.html` (or whatever you named it) is saved locally, e.g.: index.html
### Step 2: Open Terminal

Launch the macOS Terminal app (`/Applications/Utilities/Terminal.app`).

### Step 3: Run Chrome in Kiosk Mode

Execute this command in Terminal (replace the path with your actual file path):

```open -a "Google Chrome" --args --kiosk "file:///~/Documents/index.html"```
This will:
	•	Launch Chrome fullscreen without address bar, tabs, or controls.
	•	Load your Klein Bottle Rift webpage.
	•	Trap the mouse pointer and disable keyboard commands as scripted.

Step 4: Exiting Kiosk Mode

To exit kiosk mode, press:
	•	Cmd + Q to quit Google Chrome completely.

⸻

Tips for Using Chrome Kiosk Mode
	•	You can create a shell script or macOS Automator app with the above command to launch more easily.
	•	For public kiosks, configure macOS System Preferences to prevent app switching or quitting if needed.
	•	Chrome kiosk mode disables most browser UI, but OS-level shortcuts still work (like Cmd+Q).
	•	Combine with macOS settings or third-party tools to lock down the environment further.
---
