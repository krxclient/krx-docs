---
icon: stopwatch
description: >-
    Master the TAS (Tool-Assisted Speedrun) feature in KRX Client for Teeworlds.
    Learn how to record, replay, and optimize inputs for precision movement in DDNet
    maps, with auto-save and path visualization.
---

# TAS (Tool-Assisted Speedrun) ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)

The **TAS** (Tool-Assisted Speedrun) tab in the KRX Client Ultimate version provides a comprehensive suite for recording, replaying, and manipulating precise sequences of inputs, primarily for creating optimized runs on DDNet maps.

**Important Prerequisite: `/showall`**
- For TAS playback and recording to correctly interact with map entities (weapons, pickups, shields, hearts, etc.), you **must** ensure all entities are rendered *before* starting a TAS session on a server. There are two ways to do this automatically:
    1.  **KRX Console:** Press `F1` and type `cl_run_on_join "showall 1"` (requires quotes).
    2.  **DDNet Settings:** Go to `Settings -> DDNet -> Miscellaneous` and add `showall 1` to the "Run on join" field.
- *Failure to do this will likely result in TAS replays desyncing or behaving incorrectly around map entities.*

---

## **Video Tutorial**
[![TAS Tutorial](https://markdown-videos-api.jorgenkh.no/url?url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DRUUiq1ml9TU)](https://www.youtube.com/watch?v=RUUiq1ml9TU)
*(Note: Tutorial provided by m4zty, may not reflect the absolute latest UI but covers core concepts).*

---

## **Screenshot**
![TAS Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/tas-menu.png)
*(Note: Screenshot may slightly differ from the latest version).*

---
## **Main Controls**
- **TPS (Ticks Per Second)** (`krx_tastps`): Adjusts the simulation speed of the TAS world. Default Teeworlds TPS is 50. Lower values slow down the simulation, allowing for more precise input timing during recording.
- **Pause** (Hotkey: `Pause`): Toggles pausing/unpausing the TAS world simulation. Essential for frame-by-frame input.
- **Playback Replay** (Hotkey: `Load`): Starts/stops playing back the currently selected replay file in the main game world.
- **Record Replay** (Hotkey: `Record`): Starts/stops recording your inputs into the current replay buffer.
- **Clear Replay** (Hotkey: `Clear`): Clears the current replay buffer and respawns your character at the start position within the TAS world.
- **Rewind** (Hotkey: `Rewind`): Moves backward through the recorded replay buffer tick by tick (or by `Ticks` steps).
- **Forward** (Hotkey: `Forward`): Moves forward through the recorded replay buffer tick by tick (or by `Ticks` steps). Useful for reviewing or reaching a specific point after rewinding.

---

## **Settings**
- **Enable Sound** (`krx_tasusesound`): Enables playback of supported sound effects (jumps, weapon fire, etc.) within the TAS world simulation.
- **Enable Effects** (`krx_tasshoweffects`): Enables rendering of supported visual effects (grenade explosions, muzzle flashes, etc.) within the TAS world simulation.
- **Show Real Aim** (`krx_tasshowaim`): During replay playback (`Load`), makes the character visually aim according to the directions recorded in the replay, rather than following the mouse.
- **Predict Players** (`krx_tasplayerprediction`): Includes other players currently on the server in the TAS world simulation. Useful for TASing interactions but increases complexity.
- **Auto Replay** (`krx_tasautoreplay`): Automatically restarts the loaded replay when it finishes.
   - **On Freeze** (`krx_tasautoreplayfreeze`): Automatically restarts the replay if your character enters a freeze state during playback.
   - **Kill** (`krx_tasautoreplaykill`): Automatically sends `/kill` at the end of a successful replay playback cycle (useful for restarting runs quickly).
- **Auto Save Replay** (`krx_autosavereplay`): Automatically saves the current replay buffer periodically to the `replays/auto/` directory while recording.
   - **Interval** (`krx_autosavereplayinterval`): Sets the auto-save frequency in seconds.

---

## **Hotkeys**
*(Configure these keybinds in the main Settings tab or via console)*
- **Record**: `toggle krx_recordreplay 1 0`
- **Load**: `toggle krx_loadreplay 1 0`
- **Clear**: `+toggle krx_tasrespawn 1 0` (Hold key to stay at spawn after clearing)
- **Pause**: `toggle krx_taspause 0 1`
- **Rewind**: `+toggle krx_tasrewind 1 0` (Hold key to continuously rewind)
- **Forward**: `+toggle krx_tasforward 1 0` (Hold key to continuously forward)

---

## **Replay Management**
- **Folder Button**: Opens the main replay folder (`%APPDATA%/krxclient.xyz/replays/`). Replays are typically saved in subfolders named after the map.
- **Replay Selection**: Dropdown menu to select a saved replay file (`*.tas`) from the currently viewed map's folder or the main replays folder.
- **Reload Button**: Refreshes the list of available replays in the selection dropdown.
- **Load Replay Data**: (Formerly "Enter" / "Continue") Loads the selected replay file's input data into the TAS buffer and initializes the TAS world to the replay's starting state. Does *not* start playback.
- **Validate Replay**: Simulates the loaded replay internally and compares the resulting positions tick-by-tick against the positions saved within the replay file (if available). Useful for checking if a replay desyncs due to game updates or inconsistencies.
- **Save Replay**: Opens a popup dialog allowing you to name and save the current replay buffer to a `.tas` file, typically within a folder named after the current map.
- **Replay Vault Auto Sync**: ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square) (`krx_tasreplayvaultautosync`) Automatically checks for and downloads updates to the community replay vault from GitHub when the client starts.
    - **Sync Now**: Manually triggers a sync with the replay vault.

---

## **Tools**
*(Features for fine-grained control during TAS creation)*
- **Ticks** (`krx_tastickcontrolticks`): Sets the number of ticks the `Forward` and `Rewind` hotkeys jump per press (default: 1).
- **Auto Rewind** (`krx_tasautorewind`): Automatically rewinds the replay to the last safe tick *before* entering a freeze state. Triggered automatically upon freezing while recording.
- **Auto Forward** (`krx_tasautoforward`): Automatically fast-forwards through a freeze state in the recording to the first tick *after* becoming unfrozen. Useful for quickly skipping freeze waits.
- **Auto Pause** (`krx_tickcontrolpause`): Automatically pauses the TAS simulation after an Auto Rewind or Auto Forward action completes.
- **Step** (`krx_tickcontrolstep`): Modifies the `Forward` and `Rewind` hotkeys to only advance/retreat exactly one tick per press, regardless of the `Ticks` setting. Allows precise frame-by-frame input.

---

## **Fake Aim**
*(Modify aiming data within the replay for aesthetic purposes)*
- **Mode** (`krx_tas_fake_aim_mode`): Selects the type of fake aim to apply (Robot Aim, Spinbot, Random, Smooth).
- **Add Fake Aim** (`krx_tas_fake_aim`): Applies the selected fake aim mode to the current replay buffer. It modifies the `m_TargetX`/`m_TargetY` values only on ticks where aiming input is not strictly necessary for the recorded movement (e.g., not during the exact tick of firing or hooking).
    - **Robot Aim**: Keeps the aim static between essential actions.
    - **Spinbot/Random**: Replaces non-essential aim inputs with spinning/random values.
    - **Smooth**: Interpolates aim direction smoothly between essential aim input ticks.

---

## **Visuals**
- **Draw Start/End Pos** (`krx_tasdrawstartendpos`): Renders visual markers (tees) at the starting and ending positions of the loaded replay.
- **Draw Replay Path** (`krx_tasdrawpath`): Renders the positional path recorded in the currently loaded replay file.
   - **Segmented** (`krx_tasdrawpathsegmented`): If enabled, only draws a small segment of the path ahead of the current playback position. If disabled, renders the entire path.
   - **Mode** (`krx_tasdrawpathmode`): Selects the rendering style (Dotted, Full Line).
   - **Color** (`krx_tasdrawpathcolor`): Sets the color of the replay path line/dots.
- **Draw Prediction Path** (`krx_tasdrawpredictionpath`): Renders predicted future paths for characters within the TAS world simulation while recording.
   - **Mode** (`krx_tasdrawpredictionpathmode`): Selects rendering style (Dotted, Full Line).
   - **Local Color** (`krx_tasdrawpredictionpathcolor`): Color for your tee and dummy's prediction path.
   - **Frozen Color** (`krx_tasdrawpredictionpathcolorfrozen`): Color used for the prediction path when a character is predicted to be frozen.
   - **Other Color** (`krx_tasdrawpredictionpathcolorothers`): Color used for the prediction paths of other players (if Predict Players is enabled).

---

## **FAQ**
1.  **Q: Why don’t I see weapons/shields/hearts/etc. in the TAS world?**
    **A:** You most likely forgot to enable `/showall` before starting the TAS. Use `cl_run_on_join "showall 1"` or the DDNet setting to automate this. Also ensure `Settings -> DDNet -> Antiping -> Predict weapons` is enabled.
2.  **Q: Why can’t I continue my TAS run after a map change?**
    **A:** TAS state is not preserved across map changes. You must stop recording, save your replay, manually change to the correct map (e.g., on a local server or different online server), load the replay data, and then continue recording from the end point.
3.  **Q: Why did my TAS replay desync or fail mid-run?**
    **A:** Desyncs usually happen due to network lag affecting the precise timing needed for TAS playback, or complex map features not perfectly predicted by the client (e.g., random teleporters, intricate stoppers). **Solution:** Increase `cl_prediction_margin` significantly (e.g., 200+) in the F1 console before playback. If it still fails, the map might have elements inherently unreliable for TAS, or server-side checks might be interfering.
4.  **Q: Why can’t I move when I start recording TAS?**
    **A:** Check if TAS is paused (toggle with the `Pause` hotkey). Also, ensure the `krx_tasrespawn` command (bound to `Clear` hotkey) is not being held down, as holding it prevents movement.
