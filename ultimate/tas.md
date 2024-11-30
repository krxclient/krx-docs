---
icon: stopwatch
---

# TAS

The **TAS** tab in the KRX Client Ultimate version is a beta feature designed for advanced tool-assisted gameplay, enabling precise and repeatable inputs.\
For the smoothest TAS experience, we recommend using the `/showall` command upon joining a server.\
&#xNAN;_&#x4E;ote: This feature is currently under rework, and its functionality may change in the future._

***

![Меню "TAS"](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/tas-menu.png)

***

## **TAS**

* **Enable**: Activates TAS and teleports you to the TAS world.
* **TPS (Ticks Per Second)**: Adjusts the tick rate for tool-assisted inputs (default TPS for Teeworlds: 50).
* **Dummy Replay**: Enables dummy support in TAS mode.
* **Player Prediction**: Adds other players to the TAS world.
* **Ignore Start Warnings**: Suppresses warning messages at the beginning of TAS.
* **Stop Mouse When Paused**: Disables mouse input when TAS is paused, allowing for legitimate runs.
* **Use Rewind Input**: Sets mouse input to match rewinded input for more realistic replays.
* **Show Real Aim**: Displays the actual aiming direction during TAS replay.

***

## **Tools**

* **Auto Rewind**: Automatically rewinds to the last safe tick before freezing.
* **Auto Forward**: Automatically forwards to the first tick before unfreezing.
* **Rewind Ticks**: Sets the number of ticks to rewind (default: 1 tick).
* **Forward Ticks**: Sets the number of ticks to forward (default: 1 tick).
* **Pause**: Pauses TAS after auto-rewinding or auto-forwarding.
* **Step**: Rewinds or forwards by exactly one tick, enabling precise movement selection for each tick.

***

## **Fake Aim**

* **Enable**: Activates fake aim mode for deceptive targeting.
* **Mode**: Selects the type of fake aim (e.g., Robot Aim).

***

## **Auto Replay**

* **Enable**: Automatically loads and restarts replays.
* **Reset on Freeze**: Restarts the replay when freezing occurs.
* **Kill on Reset**: Kills the player when the replay ends.

***

## **God Mode**

* **Super**: Toggles the RCON command `super` in the TAS world.
* **Weapon**: Allows you to give yourself a weapon (except Ninja due to known issues).
* **Give Weapon**: Grants the selected weapon.

***

## **Hotkeys**

* **Enable TAS**: Assigns a key to activate TAS.
* **Record Replay**: Assigns a key to start recording a replay.
* **Load Replay**: Assigns a key to load a replay.
* **Respawn TAS**: Assigns a key to respawn in TAS mode.
* **Pause TAS**: Assigns a key to pause TAS.
* **Rewind TAS**: Assigns a key to rewind during TAS.
* **Forward TAS**: Assigns a key to forward during TAS.

***

## **Additional Options**

* **Replays Folder**: Opens the folder where TAS replays are stored.
* **Load/Save**: Loads or saves replays.
* **Continue**: Resumes playback from the last tick of a selected replay.
* **Custom Name Field**: Saves replays with a custom name (e.g., `my_tas`).

***

## **FAQ**

1. **Q: Why don’t I see weapons in TAS?**\
   **A:** You didn’t run the command `/showall`.
2. **Q: Why can’t I continue my run after a map change?**\
   **A:** Unfortunately, continuing is not supported across map changes. Stop recording, join the map on a different server, and continue from there.
3. **Q: What are these warnings like `Verify TAS Integrity failed...`?**\
   **A:** These warnings ensure smooth TAS runs. You can usually ignore them, but they help with debugging issues—please share them with us if you encounter problems.
4. **Q: Why did my TAS fail mid-run?**\
   **A:** TAS failures usually occur due to lag. Use the appropriate `cl_prediction_margin` setting and restart the replay from the correct starting position. Contact support if the issue persists.
5. **Q: Why can’t I move in TAS?**\
   **A:** Most likely, TAS is paused or `krx_tasrespawn` is set to 1. Unpause TAS or run `krx_tasrespawn 0` in the console to fix this.
6. **Q: Why don’t I see anything when entering TAS?**\
   **A:** You need to respawn. Use the Respawn hotkey to resolve this.
7. **Q: Why can’t I rewind or forward?**\
   **A:** You need to start recording in TAS to use rewind or forward. If step rewind/forward is enabled, the changes may be too subtle to notice—disable it if needed.
