---
icon: eye
description: >-
    Understand the Legit bot in KRX Client, a subtle assistive bot for Teeworlds.
    Explore features that provide movement assistance while maintaining a natural
    playstyle for improved gameplay without detection.
---

# Legit ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
The **Legit** bot in KRX Client focuses on providing subtle assistance while maintaining a natural playstyle, suitable for users who want help avoiding freeze without obviously appearing to use cheats.

- **Console Bind**: You can toggle the Avoid bot (when Legit is selected) using: `bind KEY toggle krx_avoidfreeze 1 0` (replace `KEY` with your desired key).
- **Performance Note**: Legit Avoid performs complex calculations (likely using a Monte Carlo Tree Search approach) and may cause FPS drops or lag on some systems, especially with many players nearby. Lowering "Quality" and "Check Ticks" can help mitigate this. See the [FAQ](../../faq.md#why-does-legit-avoid-freeze-cause-fps-drops-lag) for more performance tips.
- **Prediction Note**: Remember to set `cl_prediction_margin` based on your ping (e.g., `cl_prediction_margin 70` for 50ms ping) for optimal performance.

---

## **Screenshot**
![Legit Menu - Recommended Settings](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/legit-menu.png)

---

## **Avoid**
- **Enable**: Enables the Legit avoid functionality *when the main Avoid toggle (`krx_avoidfreeze`) is active*.
- **Player Prediction**: Predicts the movements of other players for potentially better avoidance, but can increase performance cost.
- **Better Unhook**: Enhances unhooking mechanics by checking if the potential unhook direction is safe, not just the hook action itself.
- **Drag Support**: Prevents aimbot (if used separately) from aiming at directions that could lead to freezing while Legit Avoid is active.
- **Afk Protection**: Automatically disables the bot after the specified **Afk Time** if inactivity is detected.
  - **Afk Time**: Adjustable in seconds.

---

## **Settings**
- **Hook Assistance**: Activates hook inputs for the Legit bot (allows the bot to use hook/unhook actions).
- **Direction Assistance**: Activates directional inputs (left/right/neutral) for the Legit bot.
- **Check Ticks**: Specifies how far into the future (in ticks) the Legit bot simulates potential moves to evaluate their safety. Higher values are safer but more CPU-intensive.

---

## **Priority**
*(These sliders influence the bot's decision-making process)*
- **Quality** (`krx_avoid_num_iterations`): Adjusts the number of simulations (iterations) the bot runs to find a safe move. Higher values lead to better decisions but significantly increase CPU load.
- **Randomness** (`krx_avoid_tile_exploration_constant`): Controls the balance between exploring new move sequences and exploiting known good ones (related to the UCT exploration parameter in MCTS). Higher values encourage more exploration/randomness.
- **Direction Priority** (`krx_avoid_tile_direction_weight`): Adjusts how strongly the bot prefers maintaining the player's intended movement direction.
- **Hook Priority** (`krx_avoid_tile_hook_weight`): Adjusts how strongly the bot prefers maintaining the player's current hook state (hooked or not hooked).
- **Life Priority** (`krx_avoid_tile_lifespan_weight`): Adjusts how much weight is given to simply surviving longer versus matching player input.

---

## **Tiles**
- **Teles**: Avoids teleport tiles when enabled.
- **Death**: Avoids death tiles when enabled.
- **Unfreeze**: Actively avoids unfreeze tiles.
  - **Unfreeze Ticks**: Adjusts the lookahead duration (in ticks) specifically for checking unfreeze tiles.

## **Configuration**
- Finding the optimal settings for the Legit bot is highly dependent on individual playstyle and system performance. There's no single "best" configuration. Experiment with the **Priority** sliders and **Check Ticks** to find a balance between safety, natural movement, and performance. Check the `#configs-and-replays` channel on the KRX Discord for community examples and discussions.
