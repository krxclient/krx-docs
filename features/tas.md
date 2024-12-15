---
icon: stopwatch
---

# TAS (Tool-Assisted Speedrun) ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)

The **TAS** tab in the KRX Client Ultimate version is a feature designed for advanced tool-assisted gameplay, enabling precise and repeatable inputs.  
**Note: Always use the `/showall` command upon joining a server(otherwise weapons, pickups, etc. might not work)**.  
To automatically run this command there's 2 options:
1. `F1->cl_run_on_join showall 1`
2. `Main Menu -> DDNet -> Miscellaneous -> Run on join -> showall 1` 

---

## **Screenshot**
![TAS Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/tas-menu.png)

---
## **Main**
- **TPS (Ticks Per Second)**: Adjusts the tick rate for tool-assisted inputs (default TPS for Teeworlds: 50).  
- **Pause**: Pauses TAS world(works the same as Pause hotkey).
- **Playback replay**: Plays the recorded replay(works the same as Load hotkey).
---

## **Settings**
- **Enable sound**: Enables supported sound effects in TAS world.
- **Enable effects**: Enables supported effects in TAS world(for example grenade explosions).
- **Show real aim**: When playing back a run, the tee will aim at the recorded directions.
- **Predict players**: Adds all the players in the server to the TAS world.
- **Auto Replay**: Automatically loads and restarts replays.  
   - **On freeze**: Restarts the replay when freezing occurs.  
   - **Kill**: Kills the player when the replay ends.
- **Auto Save Replay**: Automatically saves replay to the `krxclient.xyz/replays/auto/` directory.
---

## **Hotkeys**
- **Record**: Assigns a key to start recording a replay.  
- **Load**: Assigns a key to load a replay.  
- **Clear**: Assigns a key to clear current replay and respawn in TAS world.  
- **Pause**: Assigns a key to pause TAS.  
- **Rewind**: Assigns a key to rewind during TAS.  
- **Forward**: Assigns a key to forward during TAS.

---

## **Replay**
- **Folder button**: Opens replay folder(`krxclient.xyz/replays/`).
- **Replay selection**: Selector for the current replay from the saved replays.
- **Reload button**: Reloads the saved replays for selection.
- **Enter button**: Loads the inputs from the replay and automatically loads the TAS world for this replay(similar to old `Continue`).
- **Validate replay**: Validates the inputs of the replay(if the positions of the simulated inputs match the saved positions).
- **Save replay**: Opens a popup with the dialog for saving the replay.

---

## **Tools**
- **Ticks**: Sets the number of ticks to forward & rewind(default: 1 tick).
- **Auto Rewind**: Automatically rewinds to the last safe tick before freezing.  
- **Auto Forward**: Automatically forwards to the first tick before unfreezing.  
- **Auto pause**: Pauses TAS after auto-rewinding or auto-forwarding.  
- **Step**: Rewinds or forwards by exactly one tick, enabling precise movement selection for each tick.

---

## **Fake Aim**
- **Mode**: Selects the type of fake aim (Smooth, Robot Aim, etc.).
- **Add fake aim**: Adds the fake aim to the current input.  

---

## **Visuals**
- **Draw start/end pos**: Enables rendering the start/end pos of the replay.
- **Draw replay path**: Enables rendering the path of the currently loading replay.
   - **Segmented**: Draws only a segment of the whole path(when disabled renders the whole path of the replay).  
   - **Mode**: Selects the type of path rendering(Dotted, Full line).
   - **Color**: Color to be used for replay path
- **Draw prediction path**: Renders prediction lines in TAS world.
   - **Mode**: Selects the type of path rendering(Dotted, Full line).
   - **Local color**: Color to be used for rendering local/dummy characters.
   - **Frozen color**: Color used for prediction path when characters are frozen.
   - **Other color**: Color used for prediction paths of non-local characters.

---

## **FAQ**
1. **Q: Why don’t I see weapons/shields/hearts/etc. in TAS?**  
   **A:** You didn’t run the command `/showall`.  

2. **Q: Why can’t I continue my run after a map change?**  
   **A:** Unfortunately, continuing is not supported across map changes. Stop recording, save your replay, join the map on a different server, and continue from there.  

3. **Q: Why did my TAS fail mid-run?**  
   **A:** TAS failures usually occur due to lag. Use the appropriate `cl_prediction_margin` setting and restart the replay from the correct starting position. Contact support if the issue persists.  

4. **Q: Why can’t I move in TAS?**  
   **A:** Most likely, TAS is paused or `krx_tasrespawn` is set to 1. Unpause TAS or run `krx_tasrespawn 0` in the console to fix this.  
