---
icon: sparkles
description: >-
    Explore the Miscellaneous features of KRX Client, including automation tools,
    protections, trolling features, and mod detection. Enhance your Teeworlds gameplay
    with bots, auto-unfreeze, fake aim, and more.
---

# Misc

The **Misc** tab in KRX Client offers a range of tools and features designed to enhance gameplay, provide protections, and enable fun trolling mechanics.

---

## **Screenshot**
![Misc Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/misc-menu.png)
*(Note: Screenshot may slightly differ from the latest version).*

---

## **Features**

### **Bots**
*(Simple automation helpers)*
- **Moonwalk** (`krx_moonwalk`): Makes your character visually moonwalk when holding both left and right movement keys simultaneously by rapidly alternating the direction sent to the server.
- **Auto Fire** (`krx_autofire`): Automatically re-triggers the fire input while the fire key is held down, effectively acting like an auto-clicker for weapons like the pistol.
- **Auto Rehook** (`krx_autorehook`): Attempts to automatically release and re-hook a grabbed tee when the hook timer is about to expire, useful for maintaining drags.
- **Auto Jump Save** (`krx_autojumpsave`): Automatically performs a jump if it predicts doing so will prevent you from immediately falling into a freeze tile. Has different modes for sensitivity.
    - **Mode** (`krx_autojumpsave_mode`): Selects the mode (0: Simple, 1: Advanced-NoVel, 2: Advanced-VelCheck). Mode 2 only triggers if vertical velocity is dominant.
- **Quick Stop** (`krx_quickstop`): When no movement keys are pressed, the bot automatically inputs the opposite direction briefly to counteract current velocity, helping to stop faster.
    - **Ground Only** (`krx_quickstop_grounded`): If enabled, Quick Stop only activates when your character is grounded.
- **Avoid Freeze (Basic)** (`krx_avoidfreeze`): Enables the *basic* freeze avoidance bot, which only uses directional keys (left/right) to dodge freeze tiles. For more advanced avoidance, use the dedicated **Avoid** tab (Ultimate tier).
- **Dummy Fly** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) (`krx_dummyfly`): Makes your dummy automatically attempt to hook fly alongside you, mirroring hook and hammer actions.
- **Jet Ride** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) (`krx_jetride`): Automatically controls the jetpack (when active) to maintain flight, similar to hook ride but using gun recoil. Controllable with A/W/S/D.
- **Auto Aled** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square) (`krx_autoaled`): Automatically hammers a nearby frozen tee if doing so is predicted to unfreeze them safely on the other side of a freeze zone (an "aled").

### **Protections**
- **Random Timeout Seed** (`krx_randomtimeoutseed`): Generates a new timeout seed before connecting to a server. This can potentially hinder server-side fingerprinting attempts but prevents rejoining your previous position after a timeout.
- **Version Spoofer** (`krx_spoofversion`): Allows changing the client version reported to the server. May bypass some version restrictions but can cause issues if set incorrectly. Leave off if unsure.
  - **Version Nr** (`krx_spoofversion_nr`): The specific version number to report when spoofing is enabled.

### **Mod Detector**
- **Enable** (`krx_moddetector`): Activates the system to detect potential moderators or suspicious players.
- **Detect by Names** (`krx_moddetectornames`): Scans player names against internal lists of known moderators.
- **Detect Suspicious Players** (`krx_moddetector_warn`): Scans player names against internal lists of players considered potentially likely to report cheats ("Warn" list).
- **Leave on Mod Detection** (`krx_moddetector_leave`): Automatically disconnects from the server if a player detected as a moderator joins or is present.
- **Leave on Warn Detected** (`krx_moddetector_warnleave`): Automatically disconnects from the server if a player from the "Warn" list joins or is present.

### **Auto Unfreeze** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
*(Automatically shoots the laser rifle to break freeze)*
- **Enable** (`krx_unfreezebot`): Activates the Auto Unfreeze feature.
    - **Console Bind**: `bind KEY toggle krx_unfreezebot 1 0`
- **ESP** (`krx_unfreezebotesp`): Draws the predicted path of the laser used for unfreezing.
- **Advanced Settings** (`krx_unfreezebotadvancedsettings`): Enables more detailed configuration options.
    - **Bounces** (`krx_unfreezebotmostbounces`): Configures bounce preference (0: Least, 1: Most). Least bounces unfreezes quicker. Most bounces can be useful in TAS for faster reload times due to longer laser travel.
    - **Silent** (`krx_unfreezebotsilent`): Makes the aim adjustments for unfreezing invisible on your screen.
    - **Points** (`krx_unfreezebotpoints`): Number of points checked per segment when scanning for unfreeze directions. Higher values increase precision but cost more performance.
    - **Current Dir Ticks** (`krx_unfreezebotcurdirticks`): Lookahead duration (ticks) used to check if the *current* aim direction will unfreeze.
    - **Ticks** (`krx_unfreezebotticks`): Lookahead duration (ticks) used when scanning *all* directions to find the best unfreeze angle.
    - **FOV** (`krx_unfreezebotfov`): Field of view (degrees) within which the bot scans for potential unfreeze directions.

### **Fake Aim**
- **Enable** (`krx_fake_aim`): Turns on fake aim behavior to confuse or mislead other players about your actual aiming direction.
- **Send Always** (`krx_fake_aim_send_always`): If enabled, the fake aim direction is sent every tick to the server, making it appear smoother to others. If disabled, it might only send updates when other inputs change.
- **Visible** (`krx_fake_aim_visible`): Shows the fake aim direction on your own screen.
- **Mode** (`krx_fake_aim_mode`): Determines how the fake aim behaves:
  - **Mouse Pos**: Aims towards your actual mouse position. Useful with Avoid bots to make their aiming corrections less obvious.
  - **Robot Aim**: Only updates the aim position sent to the server when you hook or fire. Between actions, it keeps showing the last aim direction used.
  - **Spinbot**: Rotates your aim rapidly. Speed configurable via `krx_fake_aim_speed`.
  - **Random**: Moves your aim in random directions constantly.
  - **Fake Angles**: Aims in the opposite direction of your mouse cursor.
  - **Aimbot Troll Aim**: Always aims at the closest player (uses aimbot logic).

### **Other**
- **Change Name on Finish** (`krx_change_name_on_finish`): Automatically changes your name just before crossing a finish line.
  - **Random Name** (`krx_change_name_on_finish_random`): Use a randomly generated name.
  - **Name** (`krx_change_name_on_finish_name`): Specify a custom name to use (if Random is off).
- **Auto Team** (`krx_auto_team`): Automatically joins the specified **Preferred Team** and locks it upon connecting to a server.
  - **Preferred Team** (`krx_auto_team_preferred`): The team number (1-63) to join.
- **Anti AFK** (`krx_anti_afk`): Periodically makes small mouse movements to prevent being marked as AFK by the server based on the configured **Seconds**.
  - **Seconds** (`krx_anti_afk_seconds`): The inactivity duration (server-side) after which the anti-AFK movement triggers.
- **Kill on Freeze** (`krx_killonfreeze`): Kills your player automatically (`/kill`) the moment you enter a freeze state.
- **Fast Input** (`cl_fast_input`): Applies your input one tick earlier to the *local prediction*. This makes your actions *feel* more responsive locally but does not change server-side processing or give a true latency advantage.
  - **Fast Input Others** (`cl_fast_input_others`): Extends the fast input prediction effect to other players locally. Can make dragging feel smoother but increases the visual latency discrepancy between your view and the server state for others.
- **Ignore Replay Warnings**: Suppresses console warnings related to TAS replays (e.g., inconsistencies).
- **Hide Chat Bubble** (`krx_hidebubble`): Hides the "..." chat bubble indicator that normally appears above your tee when you are typing.
- **Send Occasional Ads** (`krx_sendads`): ![Free](https://img.shields.io/badge/Free-%234CAF50?style=flat-square) Sends occasional advertisements for KRX Client via private messages to other players on the server (Free version only).

### **Troll**
- **Emote Spam** (`krx_emotespam`): Spams random emotes as fast as the server allows.
    - **Console Bind**: `bind KEY toggle krx_emotespam 1 0`
- **Killsay/Deathsays** (`krx_killsay`): Sends pre-defined messages in chat upon getting kills or dying.
    - **Note**: Messages can be customized by editing the `data/krx/killsays.json` file.
- **Fancy Chat Font** (`krx_fancychatfont`): Changes your chat messages to use a Unicode fancy font style.
- **Mass Mention Spam** (`krx_massmentionspam`): Sends chat messages containing random spam text and mentions multiple players on the server repeatedly.
- **Chat Repeater** (`krx_chatrepeater`): Automatically repeats another player's chat message, but with alternating uppercase and lowercase letters (e.g., "Hello there" becomes "HeLlO tHeRe"). Only repeats messages longer than the specified **Min Length**.
  - **Min Length** (`krx_chatrepeater_length`): Minimum length of a message for the repeater to trigger.

### **ID Stealer**
- **Enable** (`krx_idstealer`): Activates the ID Stealer feature, copying information from another player.
- **Closest Player** (`krx_idstealer_closest`): If enabled, targets the closest player. If disabled, targets a random player.
- **Steal Name** (`krx_idstealer_name`): Copies the target's name.
- **Steal Clan** (`krx_idstealer_clan`): Copies the target's clan tag.
- **Steal Skin** (`krx_idstealer_skin`): Copies the target's skin settings (name, custom colors, body/feet colors).
- **Steal Flag** (`krx_idstealer_flag`): Copies the target's country flag.
- **Steal Eye Emote** (`krx_idstealer_emote`): Copies the target's default eye emote.
- **Stealer Speed** (`krx_idstealer_speed`): Adjusts the interval (in seconds) between updates of the stolen information.

### **Ghost Move**
*(Exploit to hide certain actions from other players)*
- **Enable** (`krx_ghostmove`): Activates the Ghost Move features selected below.
- **Direction** (`krx_ghostmovedirection`): Hides the directional arrows others see based on your movement input.
- **Jump** (`krx_ghostmovejump`): Hides the jump arrow others normally see when you jump.
- **Hook** (`krx_ghostmovehook`): Spams an invisible hook (no visual hook chain/head for others) towards your aim direction. Hook reach is still limited by server settings/tuning.
- **Hook Closest** (`krx_ghostmovehookclosest`): Spams an invisible hook towards the closest player. Hook reach is limited.

---

## **Configuration**

For most use cases, consider enabling the following features based on your needs:
- **Auto Fire**: Convenient for weapons like the pistol.
- **Avoid Freeze (Basic)**: A simple safety net on Gores maps if not using the Ultimate Avoid bots.
- **Quick Stop**: Useful for precise stopping, especially on block maps.
- **Auto Jump Save**: Situational helper to prevent accidental falls into freeze.
- **Mod Detector**: Enable if playing on servers where you are concerned about moderator detection. Configure leave settings based on risk tolerance.
- **Fast Input**: Try enabling this; many find it improves the feeling of responsiveness, though it's a local visual effect.
- **Auto Team**: Quality-of-life feature for automatically joining and locking a preferred team.

Adjust these and other features based on the game mode, server rules, and personal preference.
