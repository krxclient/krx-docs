---
icon: gear
description: >-
    Configure your KRX Client settings to optimize gameplay in Teeworlds. Learn how
    to set up hotkeys, adjust prediction margins, enable teleport prediction, and
    fine-tune bot behaviors for improved performance.
---

# Settings

The **Settings** tab in the KRX Client allows you to configure hotkeys and fine-tune specific features to enhance your gameplay experience.

---

## **Screenshot**
![Settings Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/settings-menu.png)

---

## **Hotkeys**
- **Aimbot**: Toggles the aimbot.  
- **Aimbot Auto Hook**: Automatically hooks targets when Aimbot is enabled.  
- **Aimbot Auto Shoot**: Automatically shoots at targets when Aimbot is enabled.  
- **Balance Bot**: Toggles the balance bot to maintain balance on tees.  
- **Emote Spam**: Enables continuous emote spamming.  
- **Hook Spam**: Enables rapid hook spamming.  
- **Super DynCam**: Enables unlimited zoom for the dynamic camera.  
- **Pixel Walk**: Allows precise, pixel-by-pixel movement when using directional keys.  
- **Hook Nearest Collision**: Automatically hooks to the nearest collision.  
- **Quick Stop**: Instantly counteracts movement when not holding any directional keys to stop as fast as possible.  
- **Hook Ride (risky)**: Activates hook ride bot.  
- **Record Replay**: Starts recording player inputs.  
- **Load Replay**: Loads previously recorded inputs.  
- **Avoid Freeze**: Activates the bot to help avoid freeze tiles.  
- **Auto Edge**: Enables the bot to automatically land on edges near freeze, death, or teleport tiles. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Laser Unfreeze Bot**: Activates a bot to automatically unfreeze you using the laser. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Avoid Auto Drag**: Automatically hooks the closest tee without freezing when this feature is active. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
- **Avoid Track Points**: Toggles advanced point tracking for the Blatant Gores Bot. See [Blatant Gores Bot](blatant.md) for more details. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  

---

## **Settings**
- **Teleport Prediction**: Enables teleport prediction for TAS or Gores Bot, otherwise teleports are replaced with freeze. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
- **Advanced Settings**: Unlocks advanced prediction settings for fine-tuning all KRX bots for maximum advantage: ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
   - **Death Tile Prediction**: Predicts death tiles for bots, including TAS and Gores Bot. Otherwise, death tiles are ignored.  
   - **Move Restrictions Prediction**: Predicts air stoppers. Disabling this can significantly boost bot performance.  
   - **Player Loop**: Predicts tee-to-tee collisions. Disabling this only removes collision handling and can significantly boost bot performance.  
   - **Prediction Margin**: Adjusts the prediction margin. Higher values make you less affected by lag spikes but might make others appear laggier.
- **Balance Bot Offset**: Configures how aggressively the balance bot reacts to maintain balance. Higher values reduce movement corrections.  
- **Hook Nearest FOV**: Sets the field of view for the **Hook Nearest Collision**"** feature.  

---

## **Configuration**

1. Open the **Settings** tab in the KRX Client.  
2. Assign custom hotkeys to features according to your preferences.  
3. Adjust settings to suit your gameplay needs. Below are some **recommended configurations**:  
   - **Teleport Prediction**: Recommended to keep disabled unless using TAS. Don't enable when using the Gores Bot. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
   - **Advanced Settings**: Recommended disabled unless you know what you are doing. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
      - **Death Tile Prediction**: Recommended disabled as it slows bots but it's useful for TAS.  
      - **Move Restrictions Prediction**: Recommended enabled for casual play. Disable for significant performance boosts in bots.  
      - **Player Loop**: Recommended enabled for casual play. Disable for significant performance boosts in bots.  
      - **Prediction Margin**: Choose a value based on your ping (e.g., for 50ms ping, set ~50). Setting higher values (>20) are recommended to avoid bot issues.
   - **Balance Bot Offset**: Recommended value: ~2.  
   - **Hook Nearest FOV**: Recommended to set a lower FOV (e.g., 30) to reduce lag on low-end CPUs.  
