MechCommander Redux for Mac (unofficial)
=========================================

**[MacOS Patch download](https://github.com/PepeForFun/MechCommander-MacOS/releases/download/Release/MechCommander-Redux-Mac.zip)**


A native Mac version of MechCommander Redux (https://github.com/RevenantBob/MechCommanderRedux),
the modern rebuild of MechCommander Gold (1999). It runs without Windows, CrossOver or emulation,
draws through Metal, and sharpens the picture for high-resolution screens.

This package contains NO game data. You need your own copy of MechCommander Gold.

Requirements
------------
- A Mac with Apple Silicon (M1 or newer)
- macOS 14 (Sonoma) or newer
- The MechCommander Gold game files (from the original CD or a disc image of it)

Setup
-----
1. Make a folder, for example "MechCommander Gold", and copy EVERYTHING from the
   MechCommander Gold CD into it (the folder must contain SYSTEM.CFG and the DATA folder).
2. Put "MechCommander Redux.app" next to that folder (or inside it).
3. First start: macOS blocks apps from unknown developers. Double-click the app, close the
   warning, then open System Settings > Privacy & Security, scroll down and click
   "Open Anyway" next to MechCommander Redux. You only need to do this once.

Playing
-------
- Saves and settings are kept in ~/Library/Application Support/MechCommander Redux
- HUD size: Preferences > UI RESOLUTION (a smaller number makes the HUD bigger; 720 by default)
- Zoom with the mouse wheel or the zoom keys; the picture is sharpened at every zoom level.
- Keys: the first time the game starts it writes keys.cfg into your MechCommander Gold folder
  (next to SYSTEM.CFG). Open it with TextEdit, change the key after '=' (e.g. Jump = Ctrl+K),
  save, and start the next mission (or restart the game). Delete the file to get the original
  keys back.
- If macOS asks whether the game may use your Downloads/Documents folder, click Allow
  (it only reads the game files there).

What changed compared to Redux
------------------------------
- Builds and runs natively on macOS (Apple Silicon)
- Graphics-card renderer on Metal
- Pixel-art sharpening (xBR filter) for the battlefield, the HUD and the menus
- Fixed: movies shown sheared and repeated on Metal; a crash when a mission starts;
  the loading bar half off the screen
- Key bindings can be changed in keys.cfg
- The source changes are in "source-patches" (apply to Redux commit 3c56e89 with "git am")

Legal
-----
Unofficial, non-commercial fan work. Not affiliated with or endorsed by Microsoft, FASA,
MicroProse or the MechCommander Redux author. MechCommander, BattleTech and MechWarrior are
trademarks of their respective owners. No game content is included.
