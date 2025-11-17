---
icon: robot
description: >-
    Discover the Fent Bot in KRX Client, an advanced pathfinding and tunneling bot
    for Teeworlds. Learn how to optimize movement using its genetic algorithm, tweak inputs,
    and visualize generated paths.
---

# Fent Bot ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
The **Fent Bot** in KRX Client is an advanced, experimental tool for automating map completion. It is primarily designed for KoG (King of Gores)-style maps and requires significant computational resources.

- **Console Bind**: You can toggle the Avoid bot (when Fentbot is selected) using: `bind KEY toggle krx_avoidfreeze 1 0` (replace `KEY` with your desired key). Note that enabling this mainly *starts* the Fentbot's calculation process.
- **Prediction Note**: Remember to set `cl_prediction_margin` based on your ping (e.g., `cl_prediction_margin 70` for 50ms ping) for optimal performance during calculation and potential playback (if used with TAS).
- **CPU Intensive**: Fentbot performs complex, asynchronous calculations in the background. It can consume significant CPU resources, potentially impacting game performance, especially on lower-end systems or with high configuration settings.

---

## **Screenshot**
![Fent Bot Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/fentbot-menu.png)

*(Note: Screenshot may slightly differ from the latest version).*

---

## **Avoid**
*(Settings controlling the Fentbot calculation process)*
- **Player Prediction**: Enables prediction of other players' movements during the pathfinding calculation. This allows the bot to potentially find paths that avoid other players but significantly increases calculation complexity and time.
- **Unfreeze** (Light Tile Support): Allows Fentbot to consider paths through freeze tiles if an unfreeze tile is nearby, potentially finding solutions on maps with "light freeze".
  - **Radius**: Defines the search radius around a freeze tile within which an unfreeze tile must exist for the light tile logic to apply.
- **Advanced Settings**: Unlocks detailed customization options for the bot's calculation parameters. If disabled, uses pre-defined "Quality" settings.
  - **Fent Ticks**: The maximum duration (in ticks) the bot will simulate ahead during its path calculation process. Higher values allow finding solutions for longer map segments but increase computation time.
  - **Tweaker Inputs**: Higher values explore more potential input sequences, but increase CPU load.
  - **Tweaker Ticks**: Controls the number of consecutive inputs evaluated for each cycle. Longer sequences can solve more complex maneuvers but increase calculation time.
  - **Tweaker Dosage**: Controls the number of the tests. Bigger "dosage" allows for better optimization of input sequences but significantly increases computation time.
- **Quality Setting**: *(Only available if Advanced Settings is OFF)*. Selects predefined sets of Tweaker/Fent parameters (Low, Mid, Max) offering a trade-off between calculation speed and solution quality.
- **Inject Fent**: This button toggles the main Avoid bot (`krx_avoidfreeze`). When Fentbot is the selected agent, enabling this starts the asynchronous pathfinding calculation process in the background. Disabling it should stop the calculation.

## **Visuals**
- **Render Path**: Displays the calculated path (sequence of positions) visually in the game world once found.
- **Render Pathfinding**: Highlights the areas defined as "tunnels" (valid movement areas) visually. Useful for visualizing areas where fentbot can navigate.
- **Spectate Scan**: Allows spectating the bot's simulated progress during the calculation phase. The camera will attempt to follow the bot's current best-known position in the simulation. Requires being in spectator mode.

## **Tile Editor**
*(Tools for defining the bot's pathfinding area)*
- **Recalculate**: Manually triggers a recalculation of the pathfinding grid.
- **Auto Finish**: Attempts to automatically detect and mark finish tiles for the bot's navigation goal.
- **Enable Editor**: Enables a mode where you can manually add or remove tiles from the navigable area. This directly influences the pathfinding calculation.
- **Tile Type**: Choose between "Tunnel" (navigable area) and "Finish" tiles when editing.
- **Auto Tunnels**: Automatically generates a restricted movement tunnel based on the path taken in a loaded TAS replay file (`*.tas`). The bot will then only search for solutions within this defined tunnel.
  - **Auto Tunnel Width**: Adjusts the width (in tiles) of the auto-generated tunnel around the replay path.
- **Clear All Tiles**: Removes all manually created and auto-generated tunnels, resetting the pathfinding area to the entire map (minus standard obstacles).

---

## **Configuration**
- For most users, starting with the default settings or a predefined **Quality Setting** (Low/Mid/Max) is recommended.
- **Advanced Settings**: Only enable if you understand the impact of the Tweaker parameters on performance and solution quality. Higher values dramatically increase CPU usage and calculation time.
  - A possible configuration for **high-end CPUs**:
    - **Player Prediction**: OFF (unless specifically needed)
    - **Advanced Settings**: ON
    - **Fent Ticks**: 1000-10000 (depending on map segment length)
    - **Tweaker Inputs**: High (e.g., 500-1000+)
    - **Tweaker Ticks**: 8-16 (adjust based on maneuver complexity)
    - **Tweaker Dosage**: High (e.g., 100-300+)
- **Tunnels**: Using **Auto Tunnels** with a previously recorded (even imperfect) TAS replay can significantly speed up calculation by drastically reducing the search space. Manually defining tunnels with the **Tile Editor** can achieve the same but requires more effort.
- **Start Calculation**: Use the **Inject Fent** button to start the pathfinding process. Be patient, as calculations can take minutes or even hours depending on settings and map complexity.
