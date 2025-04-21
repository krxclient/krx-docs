---
icon: gear
description: >-
    Configure your KRX Client settings to optimize gameplay in Teeworlds. Learn how
    to set up hotkeys, adjust prediction margins, enable teleport prediction, and
    fine-tune bot behaviors for improved performance.
---

# Settings

The **Settings** tab in the KRX Client allows you to configure hotkeys for various features and fine-tune specific client and bot behaviors to enhance your gameplay experience.

---

## **Screenshot**
![Settings Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/settings-menu.png)

*(Note: Screenshot may slightly differ from the latest version).*

---

## **Hotkeys**
*(Assign keys to quickly toggle features. Use the format `bind KEY COMMAND` in the F1 console for more complex binds like toggles, e.g., `bind x toggle krx_avoidfreeze 1 0`)*

- **Aimbot** (`+toggle krx_aimbot 1 0`): Toggles the main aimbot system.
- **Aimbot Auto Hook** (`+toggle krx_aimbot_autohook_key 1 0`): Press-and-hold key to enable automatic hooking when Aimbot is active and finds a valid hook target.
- **Aimbot Auto Shoot** (`+toggle krx_aimbot_autoshoot_key 1 0`): Press-and-hold key to enable automatic firing when Aimbot is active and finds a valid weapon target.
- **Balance Bot** (`+toggle krx_balancebot 1 0`): Toggles the balance bot, which helps maintain horizontal position relative to a targeted tee.
- **Emote Spam** (`+toggle krx_emotespam 1 0`): Toggles continuous random emote spamming.
- **Hook Spam** (`+toggle krx_hookspam 1 0`): Toggles rapid hook/unhook spamming.
- **Super DynCam** (`toggle krx_superdyncam 1 0`): Enables unlimited zoom when using the dynamic camera (`cl_dyncam 1`).
- **Pixel Walk** (`toggle krx_pixelwalk 1 0`): When holding a movement key, only inputs movement every other tick, allowing for precise pixel-by-pixel adjustments.
- **Hook Nearest Collision** (`+toggle krx_hooknearestcollisionautohook 1 0`): Press-and-hold key to automatically aim at and hook the nearest solid tile within the configured FOV.
- **Quick Stop** (`toggle krx_quickstop 1 0`): Toggles the Quick Stop bot, which helps stop faster by briefly countering movement.
- **Hook Ride (risky)** (`toggle krx_hookride 1 0`): Toggles the Hook Ride bot (can be unstable or detectable).
- **Record Replay** (`toggle krx_recordreplay 1 0`): Starts/stops recording player inputs for TAS.
- **Load Replay** (`toggle krx_loadreplay 1 0`): Starts/stops playing back the loaded TAS replay.
- **Avoid Freeze** (`toggle krx_avoidfreeze 1 0`): Toggles the currently selected Gores Bot (Avoid feature).
- **Auto Edge** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) (`+toggle krx_autoedge 1 0`): Press-and-hold key to enable the bot that attempts to automatically land on edges near dangerous tiles (freeze, death, tele).
- **Laser Unfreeze Bot** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) (`toggle krx_unfreezebot 1 0`): Toggles the bot that automatically uses the laser rifle to unfreeze you.
- **Avoid Auto Drag** ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square) (`+toggle krx_avoid_tile_auto_drag 1 0`): Press-and-hold key to enable the Blatant bot's Auto Drag feature.
- **Avoid Track Points** ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square) (`toggle krx_avoid_tile_track_points 1 0`): Toggles the Blatant bot's Track Point feature. See [Blatant Gores Bot](goresbot/blatant.md) for details.

---

## **Settings**
- **Prediction Margin** (`cl_prediction_margin`): Adjusts the client-side prediction time margin (in milliseconds).
    - **Recommendation**: Set this value slightly higher than your average ping to the server (e.g., `cl_prediction_margin 70` for 50ms ping).
    - **Impact**: Higher values help compensate for lag spikes, making your local prediction smoother but potentially increasing the visual delay of other players. Crucial for the reliability of prediction-heavy features like Avoid bots and TAS.
- **Teleport Prediction** ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square) (`krx_predictionteleports`): Enables prediction of teleport tile destinations. Primarily useful for TAS. If disabled, teleporters are treated like freeze tiles by bots. **Recommendation**: Keep disabled unless specifically needed for TAS, as it can interfere with Gores Bots.
- **Advanced Prediction Settings** ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square) (`krx_predictionadvancedsettings`): Unlocks fine-grained control over prediction behavior.
    - **Death Tile Prediction** (`krx_predictiondeathtile`): Predicts death tiles for bots (TAS, Avoid). Disabling ignores death tiles, potentially speeding up calculations but making bots unsafe near death tiles. **Recommendation**: Disable for performance unless needed for TAS accuracy.
    - **Move Restrictions Prediction** (`krx_predictionmoverestriction`): Predicts tiles that restrict movement (stoppers). Disabling can significantly boost bot calculation performance but makes them unaware of stoppers. **Recommendation**: Enable for general play; disable for maximum bot speed if stoppers aren't relevant.
    - **Player Loop (Collision)** (`krx_predictionplayers`): Predicts character-to-character collisions. Disabling removes this check, potentially boosting bot calculation performance but making them ignore player interactions. **Recommendation**: Enable for general play; disable for maximum bot speed if player collision isn't relevant.
    - **Heart Tile Prediction** (`krx_predictionheart`): Predicts behavior of heart tiles (pickup tiles). **Recommendation**: Disable unless playing on specific maps where heart tiles cause freezing issues.
- **Balance Bot Offset** (`krx_balancebot_offset`): Configures how aggressively the Balance Bot reacts. Higher values mean the bot allows for a larger horizontal distance difference before correcting, resulting in less frequent adjustments.
- **Hook Nearest FOV** (`krx_hooknearestcollisionfov`): Sets the field of view (degrees) for the "Hook Nearest Collision" feature. Lower values reduce the scan area, potentially improving performance on lower-end systems.

---

## **Configuration**

1. Open the **Settings** tab in the KRX Client.
2. **Assign Hotkeys**: Click the buttons next to each feature and press the desired key to bind it. Use the console (`F1`) for more complex binds (e.g., toggles with `bind KEY toggle COMMAND 1 0`).
3. **Adjust Settings**:
   - **Prediction Margin**: **Crucial setting.** Set based on your ping as recommended above. Increase if bots behave erratically due to lag.
   - **Teleport Prediction**: Usually **Disabled**, enable only for specific TAS needs.
   - **Advanced Prediction Settings**: Keep **Disabled** unless you understand the performance/safety trade-offs. If enabled:
      - **Death Tile**: Usually **Disabled** (performance > safety) unless doing TAS.
      - **Move Restrictions / Player Loop**: Usually **Enabled**. Disable only if you need maximum bot calculation speed and are certain stoppers/player collisions are irrelevant or handled manually.
   - **Balance Bot Offset**: Start around **2** and adjust based on desired responsiveness.
   - **Hook Nearest FOV**: Lower values (e.g., **30-90**) can reduce potential lag if the feature feels heavy.
