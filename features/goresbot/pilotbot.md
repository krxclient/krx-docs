---
icon: plane
description: >-
    Discover the Pilot Bot in KRX Client for Teeworlds. Learn how to configure its
    autonomous navigation modes, performance settings, and visual aids for advanced
    automated gameplay.
---

# Pilot Bot ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
The **Pilot Bot** is an advanced experimental real-time Gores bot that automatically navigates maps. It can operate fully autonomously, follow your cursor, or track another player, making it a versatile tool for various gameplay scenarios.

- **Console Bind**: You can toggle the Avoid bot (when Pilot Bot is selected) using: `bind KEY toggle krx_avoidfreeze 1 0` (replace `KEY` with your desired key).
- **Prediction Note**: Remember to set `cl_prediction_margin` based on your ping (e.g., `cl_prediction_margin 70` for 50ms ping) for optimal performance.

---

## **Screenshot**
![Pilot Bot Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/pilotbot-menu.png)

---

## **Main**
- **Enable**: Enables the Pilot Bot functionality *when the main Avoid toggle (`krx_avoidfreeze`) is active*.
- **Player Prediction**: Predicts the movements of other players for potentially better navigation and avoidance.
- **Mode**:
    - **Autonomous**: The bot navigates the map on its own, trying to find a path to the finish.
    - **Follow Cursor**: The bot attempts to follow your mouse cursor.
    - **Follow Player**: The bot attempts to follow the closest player.

---

## **Settings**
*(These sliders influence the bot's performance and decision-making)*
- **Population Size**: Number of movement sequences to generate and test. Higher values find better paths but use more CPU.
- **Exploration Depth**: How many ticks into the future the bot simulates for each sequence.
- **Top-K Candidates**: The number of best sequences from the population to consider for the final path.
- **Sequence Length**: How many ticks from the best-calculated sequence are used before recalculating.

---

## **Visuals**
- **Render Path**: Displays the path the bot is currently following.
- **Render Pathfinding**: Shows the underlying pathfinding grid (FlowField) the bot uses for navigation.

---

## **Tile Editor**
*(Tools for defining the bot's pathfinding area)*
- **Recalculate**: Manually triggers a recalculation of the pathfinding grid.
- **Auto Finish**: Attempts to automatically detect and mark finish tiles for the bot's navigation goal.
- **Enable Editor**: Allows you to manually add or remove tiles from the navigable area.
- **Tile Type**: Choose between "Tunnel" (navigable area) and "Finish" tiles when editing.
- **Auto Tunnels**: Generates a restricted tunnel based on a loaded TAS replay, forcing the bot to stay within that path.
    - **Auto Tunnel Width**: Adjusts the width of the generated tunnel.
- **Clear All Tiles**: Resets all custom tunnels and finish points.
