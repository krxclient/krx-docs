---
icon: robot
---

# Fent Bot ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
The **Fent Bot** tab in KRX Client provides advanced tool for automating via pathfinding and tunneling.  
*Note: When using avoid bots, please use a higher `cl_prediction_margin` refer to [settings](../settings.md) and choose pred margin based on ping*

---

## **Screenshot**
![Fent Bot Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/fentbot-menu.png)

---

## **Avoid**
- **Player Prediction**: Enables prediction of other players movements.
- **Advanced Settings**: Unlocks advanced customization options for the bot's behavior.
- **Use Skibidiforce**: Activates the Skibidiforce algorithm for advanced pathfinding.
  - **Skibidiforce Depth**: Configures the depth of Skibidiforce calculations.
- **Fent Ticks**: Defines the tick duration for fent-based pathfinding.
- **Tweaker Inputs**: Number of tweaker inputs.
- **Tweaker Ticks**: Adjusts the tick duration for tweaker inputs.
- **Inject Fent**: A one-click action to start scanning.  

## **Misc**
- **Skibidiforce Aim Points**: Configures the number of aim points used by Skibidiforce.
- **Render Path**: Displays the calculated path visually.
- **Render Tunnels**: Highlights tunnels used for pathfinding.
- **Spectate Scan**: Allows spectating the progress scan during scanning.  
- **Tunnel Editor**: Provides a UI for customizing tunnels manually.
- **Auto Tunnels**: Automatically generates tunnels for optimized movement from a loaded replay.
- **Tunnel Width**: Adjusts the width of auto-generated tunnels.
- **Clear Tunnels**: Removes all tunnels.

---

## **Configuration**
- Most times using the default settings provided by KRX is enough. Here's a possible configuration for more advanced users with good CPUs:
- **Player Prediction**: OFF
- **Advanced Settings**: ON
- **Use Skibidiforce**: ON
- **Skibidiforce Depth**: 4
- **Fent Ticks**: 1000
- **Tweaker Inputs**: maximum
- **Tweaker Ticks**: 4-8
