---
icon: fire
description: >-
    Learn about the Blatant Gores Bot in KRX Client, designed to complete Teeworlds
    Gores maps efficiently. Explore features like hook assistance, direction prediction,
    and rate-limiting for optimal movement.
---

# Blatant ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
The **Blatant** Gores bot in KRX Client is expertly designed for maximum safety and effectiveness in avoiding freeze on Gores maps, from easy to extreme. It uses more direct input manipulation, including hook control, compared to the Legit bot.

- **Console Bind**: You can toggle the Avoid bot (when Blatant is selected) using: `bind KEY toggle krx_avoidfreeze 1 0` (replace `KEY` with your desired key).
- **Prediction Note**: Remember to set `cl_prediction_margin` based on your ping (e.g., `cl_prediction_margin 70` for 50ms ping) for optimal performance.

---

## **Screenshot**
![Blatant Menu - Recommended Settings](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/blatant-menu.png)

---

## **Avoid**
- **Enable**: Enables the Blatant avoid functionality *when the main Avoid toggle (`krx_avoidfreeze`) is active*.
- **Player Prediction**: Predicts the movements of other players for potentially better avoidance.
- **NSIF** (No Safe Input Found): If the bot cannot find an input sequence that guarantees survival for the full `Check Ticks` duration, NSIF allows it to use the *first* input from the previously known safest sequence, hoping it remains valid temporarily.
- **Afk Protection**: Automatically disables the Gores bot when the user is detected as AFK after the specified **Afk Time**.
  - **Afk Time**: Configurable in seconds.

## **Settings**
- **Hook Assistance**: Activates hook inputs for the Gores bot (allows the bot to use hook/unhook actions).
- **Direction Assistance**: Enables directional inputs (left/right/neutral) for the Gores bot.
- **Check Ticks**: Specifies how far into the future (in ticks) the Blatant bot's primary simulation (`TestFreezeOptimal`) runs to guarantee safety for an input sequence. Higher values provide more safety but increase CPU load.
- **Kick in Ticks**: The bot will *not* intervene or override your current input if that input is predicted to be safe for at least this many ticks. Lower values make the bot intervene sooner.
- **Action Ticks**: *[This setting might be outdated or its effect subtle. It likely related to older/alternative simulation logic. `Check Ticks` is the primary control for prediction depth.]*

## **Ratelimiting**
*(These settings prevent the bot from spamming inputs too quickly, making its actions seem slightly more human)*
- **Enable**: Enables rate-limiting for various actions.
- **Hook/Unhook**: Limits the frequency of the bot initiating hook and unhook actions.
- **Direction/No Direction**: Limits the frequency of the bot changing directional input (Move) or stopping (Stand).
- **Hook Check**: *[Description unclear, might be related to applying direction limits only when not hooking? Needs verification.]*
  - **Hook Ticks**: Minimum duration (in ticks) the bot must wait between consecutive hook actions.
  - **Unhook Ticks**: Minimum duration the bot must wait between consecutive unhook actions.
  - **Move Ticks**: Minimum duration the bot must wait between changing directional movement inputs.
  - **Stand Ticks**: Minimum duration the bot must wait between stopping movement inputs.

## **Misc**
- **Drag Support**: Provides additional data to the aimbot (if used separately), helping it avoid aiming directions that could lead to freezing while Blatant Avoid is active.
- **Track Point**: If enabled, the bot identifies the last direction the player aimed at which was hookable onto a tile. It will prioritize maintaining aim towards this "track point" during its safety calculations, potentially overriding mouse aim if the tracked direction is safer.
  - **Safe Aim Tracking**: If Track Point is enabled, this ensures the bot only locks onto the tracked direction if that direction remains valid (doesn't lead to freeze) for the *entire* `Check Ticks` scan duration. Disabling this allows tracking even if the direction becomes unsafe later in the prediction, potentially leading to riskier but more persistent aim tracking.
- **Rehook Action**: *[Description unclear, likely enables logic specifically considering quick rehook scenarios during prediction? Needs verification.]*
- **Auto Drag**: ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square) Automatically aims at and hooks the closest tee *if* doing so is predicted to be safe (doesn't cause freeze). Uses aimbot logic internally for target selection and edge hooking.
- **Tile Distance**: *[Description unclear, possibly adjusts the hitbox size used for tile avoidance? Needs verification.]*

## **Tiles**
- **Teles**: Avoids teleport tiles when enabled.
- **Unfreeze**: Avoids unfreeze tiles when enabled.
  - **Ticks**: Configurable check duration (lookahead in ticks) specifically for avoiding unfreeze tiles.
- **Death**: Avoids death tiles when enabled.

## **Aimbot**
*(Internal aimbot used for specific Blatant features like Auto Drag and aiming at Track Points)*
- **Enable**: Activates the Blatant bot's internal aimbot logic for features that require aiming assistance.
- **Auto Aim**: Scans all directions within FOV and selects the aim direction that is predicted to be safe for the longest duration.
- **Aim Assist**: Targets the valid, safe direction (within FOV) that is closest to your current mouse cursor and remains safe the longest.
- **Upward Aim**: *[Description unclear, possibly prioritizes upward safe directions? Needs verification.]*
- **Points**: Specifies the number of aim points to evaluate per segment during aimbot scans. Higher values increase precision but cost more performance.
- **Segments**: Defines the number of angular segments the aimbot scans within its FOV. Higher values increase coverage but cost more performance.
- **FOV**: Configurable field of view (degrees) for the internal aimbot's targeting.
- **Check Ticks**: Adjusts the prediction duration (in ticks) specifically used for the internal aimbot's safety calculations when evaluating aim directions.

## **Visuals**
- **Track Point**: Displays the currently tracked aim point visually if the Track Point feature is active.
- **Aimbot**: Highlights the target point selected by the internal aimbot visually.
- **Path**: Shows the predicted path the bot intends to follow based on its calculated safe input sequence.

## **Configuration**
- The provided default/recommended settings are a good starting point.
- **NSIF**: Generally recommended ON for better recovery when no perfectly safe path is found instantly.
- **Hook/Direction Assistance**: Recommended ON for full bot capability.
- **Check Ticks / Kick in Ticks**: Balance these. Higher `Check Ticks` (e.g., 26) gives more safety margin. `Kick in Ticks` should be lower than `Check Ticks` (e.g., 20) to allow the bot to intervene before it's too late. Lower values mean the bot reacts sooner but might feel more intrusive.
- **Track Point / Safe Aim Tracking**: Enable Track Point if you want the bot to help maintain aim on hookable ground. Enable Safe Aim Tracking ON for maximum safety (won't track if it might lead to freeze later), OFF for more persistent tracking even if slightly risky.
- **Auto Drag**: Useful for automatically dragging nearby tees safely, but requires the internal Aimbot to be configured reasonably (FOV, Segments, Points).
