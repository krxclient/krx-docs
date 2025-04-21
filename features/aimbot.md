---
icon: bullseye-arrow
description: >-
    Learn how to configure the Aimbot feature in KRX Client for Teeworlds. This guide
    covers targeting methods, FOV adjustments, grenade prediction, and advanced settings
    for improved precision in DDNet.
---

# Aimbot

The **Aimbot** tab in KRX Client is designed to give you a competitive edge in Teeworlds by offering precise targeting and extensive customization options.
Starting from the **Premium** tier, the Aimbot provides functionality for all weapons, edge hook mechanics, and advanced settings, such as grenade move prediction, edge accuracy, and adjustable shooting delays.

---

## **Screenshot**
![Aimbot Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/aimbot-menu.png)

*(Note: Screenshot may slightly differ from the latest version).*

---

## **Features**

- **Enable**: Toggles the Aimbot on or off globally via the menu.
    - **Console Bind**: You can also toggle the aimbot using a key bind in the F1 console: `bind KEY toggle krx_aimbot 1 0` (replace `KEY` with your desired key, e.g., `lctrl`).
- **Draw FOV**: Displays two lines originating from your character, indicating the angular Field of View (FOV) centered around your mouse cursor. Targets outside this wedge are ignored by the aimbot for the active weapon/hook.
- **Auto Shoot**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Toggles automatic firing when the aimbot acquires a valid weapon target. This can also be controlled via a separate hotkey (see Settings tab).
- **Target Priority**: Determines the method for selecting targets:
  - **Closest to Crosshair**: Targets based on the distance from your crosshair. This option ensures more precise identification but may struggle with hammer aimbot in some scenarios.
  - **Closest to Player**: Targets the nearest player to you. Ideal for HvH scenarios or more aggressive playstyles.
- **Silent**: Makes Aimbot adjustments invisible on your screen (your aim remains where your mouse points locally) while still sending the adjusted aim to the server, making it functional but visually hidden from your perspective. This applies differently per weapon based on individual silent settings.
- **Ignore Friends**: Prevents the Aimbot from targeting friends (added via the Teeworlds client's friend system). This applies differently per weapon based on individual ignore settings.
- **Target Box**: Highlights targets with boxes (red for hook, orange for weapon). Useful for PvP modes but may be distracting in casual play.
- **Target Glow**: Adds a "glow" effect by changing the target's tee colors. Note: This does not work effectively with tees that have a solid black color body/feet. Color settings are available if enabled.
    - **Weapon Glow Color**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Sets the glow color applied to the weapon target.
    - **Hook Glow Color**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Sets the glow color applied to the hook target.
- **Advanced Settings**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Unlocks additional per-weapon controls and advanced behavior settings.
- **Grenade Move Prediction**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Anticipates target movements based on potential inputs to improve grenade accuracy. **Note:** This is CPU-intensive and may impact performance, especially on lower-end PCs.
- **Edge Accuracy**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Adjusts edge hook precision:
  - **Lower Values**: Increases the chance of missing but makes movements look more legitimate.
  - **Higher Values**: Improves accuracy for difficult edge hooks, even in challenging scenarios.
- **Min/Max Shoot Delay**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Simulates holding the fire button for a randomized duration within the specified range after the aimbot decides to shoot. Delay is measured in ticks (1 tick ≈ 20ms at 50 TPS). For HvH play, setting both to the minimum (1) maximizes shooting speed.

---

## **Weapon Specific Settings**
*(These settings might be visible only when "Enable" is checked for the respective weapon)*

For **Hook**, **Hammer**, **Pistol**, **Shotgun**, **Grenade**, and **Laser**:
- **Enable**: Toggles aimbot functionality specifically for this weapon/hook.
- **FOV**: Adjusts the angular Field of View (degrees) within which the aimbot will consider targets for this specific weapon/hook.
- **Target Priority**: Overrides the global target priority setting for this specific weapon/hook (Closest to Crosshair / Closest to Player).
- **Silent**: Overrides the global silent setting for this specific weapon/hook.
- **Ignore Friends**: Overrides the global ignore friends setting for this specific weapon/hook.

---

## **Configuration**

1. Open the **Aimbot** tab in the client.
2. Customize the settings. Here are the **recommended settings for semi-legit daily play**:
   - **Enable**: On (preferably bind to a key like `lctrl` using `bind lctrl toggle krx_aimbot 1 0`).
   - **Draw FOV**: Off for less visual clutter, On if you need to visualize the range.
   - **Auto Shoot**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Enable based on preference or bind the hotkey `+toggle krx_aimbot_autoshoot_key 1 0` (see Settings tab).
   - **Target Priority (Global)**: Use **Closest to Crosshair** for most scenarios. Switch to **Closest to Player** if encountering hammer aimbot issues.
   - **Silent (Global/Per-Weapon)**: Off for legit play. On if playing casually or prioritizing convenience.
   - **Ignore Friends (Global/Per-Weapon)**: Enable for block or PvP modes to avoid targeting teammates.
   - **Target Box**: Off for less distraction in casual play; On can be useful in PvP to identify targets easily.
   - **Target Glow**: A subtler alternative to the Target Box—use based on preference. Set colors if enabled.
   - **Advanced Settings**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Keep off unless you need fine-grained control or premium features.
   - **Grenade Move Prediction**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Disable unless you have a powerful CPU and require maximum grenade precision.
   - **Edge Accuracy**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Set higher for consistent hooks, lower to appear more legitimate.
   - **Min/Max Shoot Delay**: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) Keep default (Min 1, Max 8) unless specific adjustments are needed (e.g., set both to 1 for rapid fire in HvH).
   - **Weapon Specific Settings**: Enable only the weapons/hook you intend to use the aimbot for. Adjust FOV per weapon (e.g., smaller FOV for rifle/laser, larger for shotgun/hammer) to balance effectiveness and legitimacy. Set per-weapon Silent/Ignore Friends/Target Priority as needed.
