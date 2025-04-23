---
icon: fire
description: >-
    Learn about the Blatant Gores Bot in KRX Client, designed to complete Teeworlds
    Gores maps efficiently. Explore features like hook assistance, direction prediction,
    and rate-limiting for optimal movement.
---

# Blatant ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)

The **Blatant** Gores bot in KRX Client is expertly designed for maximum safety and effectiveness in avoiding freeze on Gores maps, from easy to extreme. It uses more direct input manipulation, including hook control, compared to the Legit bot.

{% hint style="info" %}
**Console Bind**: You can toggle the Avoid bot (when Blatant is selected) using:
`bind KEY toggle krx_avoidfreeze 1 0`
*(Replace `KEY` with your desired key).*
{% endhint %}

{% hint style="danger" %}
**Prediction Prerequisite**: Remember to set `cl_prediction_margin` based on your ping (e.g., `cl_prediction_margin 70` for 50ms ping) for optimal performance. Incorrect prediction settings will lead to poor bot performance. See [Settings](../settings.md) for more details.
{% endhint %}

---

## **Screenshot**

![Blatant Menu - Recommended Settings](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/blatant-menu.png)

---

## Features Breakdown

<details>
<summary><strong>Avoid Settings</strong></summary>

*   **Enable**: Enables the Blatant avoid functionality *when the main Avoid toggle (`krx_avoidfreeze`) is active*.
*   **Player Prediction**: Predicts the movements of other players for potentially better avoidance.
*   **NSIF** (No Safe Input Found): If the bot cannot find an input sequence that guarantees survival for the full `Check Ticks` duration, NSIF allows it to use the *first* input from the previously known safest sequence, hoping it remains valid temporarily.
    {% hint style="info" %}
    It's generally recommended to keep NSIF `ON` for better recovery when no perfectly safe path is found instantly.
    {% endhint %}
*   **Afk Protection**: Automatically disables the Gores bot when the user is detected as AFK after the specified **Afk Time**.
    *   **Afk Time**: Configurable in seconds.
</details>

<details>
<summary><strong>Movement Settings</strong></summary>

*   **Hook Assistance**: Activates hook inputs for the Gores bot (allows the bot to use hook/unhook actions).
    {% hint style="info" %} Recommended setting: `ON` for full bot capability. {% endhint %}
*   **Direction Assistance**: Enables directional inputs (left/right/neutral) for the Gores bot.
    {% hint style="info" %} Recommended setting: `ON` for full bot capability. {% endhint %}
*   **Check Ticks**: Specifies how far into the future (in ticks) the Blatant bot's primary simulation (`TestFreezeOptimal`) runs to guarantee safety for an input sequence.
    {% hint style="warning" %} Higher values provide more safety but increase CPU load. (Default/Recommended: ~26) {% endhint %}
*   **Kick in Ticks**: The bot will *not* intervene or override your current input if that input is predicted to be safe for at least this many ticks.
    {% hint style="info" %} Lower values make the bot intervene sooner, but might feel more intrusive. Should be lower than `Check Ticks`. (Default/Recommended: ~20) {% endhint %}
</details>

<details>
<summary><strong>Ratelimiting (Humanization)</strong></summary>

*(These settings prevent the bot from spamming inputs too quickly, making its actions seem slightly more human)*

*   **Enable**: Enables rate-limiting for various actions.
*   **Hook/Unhook**: Limits the frequency of the bot initiating hook and unhook actions.
*   **Direction/No Direction**: Limits the frequency of the bot changing directional input (Move) or stopping (Stand).
    *   **Hook Ticks**: Minimum duration (in ticks) the bot must wait between consecutive hook actions.
    *   **Unhook Ticks**: Minimum duration the bot must wait between consecutive unhook actions.
    *   **Move Ticks**: Minimum duration the bot must wait between changing directional movement inputs.
    *   **Stand Ticks**: Minimum duration the bot must wait between stopping movement inputs.
</details>

<details>
<summary><strong>Misc Features</strong></summary>

*   **Drag Support**: Provides additional data to the aimbot (if used separately), helping it avoid aiming directions that could lead to freezing while Blatant Avoid is active.

*   **Track Point**: If enabled, the bot identifies the last direction the player aimed at which was hookable onto a tile. It will prioritize maintaining aim towards this "track point" during its safety calculations, potentially overriding mouse aim if the tracked direction is safer.
    {% hint style="info" %}
    **Hotkey:** You can toggle this feature using the bind set in `Settings -> Hotkeys -> Avoid Track Points`. The default command is `toggle krx_avoid_tile_track_points 1 0`.
    {% endhint %}

    *   **Safe Aim Tracking**: If Track Point is enabled, this ensures the bot only locks onto the tracked direction if that direction remains valid (doesn't lead to freeze) for the *entire* `Check Ticks` scan duration.
        {% hint style="info" %}
        *   Setting it `ON`: Provides maximum safety (won't track if it might lead to freeze later).
        *   Setting it `OFF`: Allows more persistent tracking even if slightly risky.
        {% endhint %}

*   **Auto Drag**: Automatically aims at and hooks the closest tee *if* doing so is predicted to be safe (doesn't cause freeze). Uses aimbot logic internally for target selection and edge hooking.
    {% hint style="info" %}
    **Hotkey:** You can activate this feature by holding the key set in `Settings -> Hotkeys -> Avoid Auto Drag`. The default command is `+toggle krx_avoid_tile_auto_drag 1 0`. This requires the internal Aimbot to be enabled and configured.
    {% endhint %}
</details>

<details>
<summary><strong>Tile Avoidance</strong></summary>

*   **Teles**: Avoids teleport tiles when enabled.
*   **Unfreeze**: Avoids unfreeze tiles when enabled.
    *   **Ticks**: Configurable check duration (lookahead in ticks) specifically for avoiding unfreeze tiles.
*   **Death**: Avoids death tiles when enabled.
</details>

<details>
<summary><strong>Internal Aimbot (for Auto Drag / Track Point)</strong></summary>

*(Internal aimbot used for specific Blatant features like Auto Drag and aiming at Track Points)*

*   **Enable**: Activates the Blatant bot's internal aimbot logic for features that require aiming assistance.
*   **Auto Aim**: Scans all directions within FOV and selects the aim direction that is predicted to be safe for the longest duration.
*   **Aim Assist**: Targets the valid, safe direction (within FOV) that is closest to your current mouse cursor and remains safe the longest.
*   **Points**: Specifies the number of aim points to evaluate per segment during aimbot scans. Higher values increase precision but cost more performance.
*   **Segments**: Defines the number of angular segments the aimbot scans within its FOV. Higher values increase coverage but cost more performance.
*   **FOV**: Configurable field of view (degrees) for the internal aimbot's targeting.
*   **Check Ticks**: Adjusts the prediction duration (in ticks) specifically used for the internal aimbot's safety calculations when evaluating aim directions.
</details>

<details>
<summary><strong>Visuals</strong></summary>

*   **Track Point**: Displays the currently tracked aim point visually if the Track Point feature is active.
*   **Aimbot**: Highlights the target point selected by the internal aimbot visually.
*   **Path**: Shows the predicted path the bot intends to follow based on its calculated safe input sequence.
</details>

---

## **Configuration Recommendations**

The provided default/recommended settings (shown in the screenshot) are a good starting point. Here's a quick guide:

{% hint style="info" %}
**Basic Setup Steps:**
- [x] Ensure `cl_prediction_margin` is set correctly (See Prerequisite hint above).
- [x] Enable the main Avoid toggle (`krx_avoidfreeze`) via bind or the menu.
- [x] Enable `Hook Assistance` and `Direction Assistance` for full functionality.
- [x] Adjust `Check Ticks` and `Kick in Ticks` based on desired safety vs. performance/intrusiveness.
{% endhint %}

*   **NSIF**: Generally recommended `ON`.
*   **Check Ticks / Kick in Ticks**: Balance these. Higher `Check Ticks` (e.g., 26) gives more safety margin. `Kick in Ticks` should be lower than `Check Ticks` (e.g., 20) to allow the bot to intervene before it's too late.
*   **Track Point / Safe Aim Tracking**: Enable `Track Point` if you want aim assistance on hookable ground. Enable `Safe Aim Tracking ON` for maximum safety, `OFF` for more persistent (potentially riskier) tracking.
*   **Auto Drag**: Enable if you want automatic safe drags on nearby tees. Requires configuring the internal `Aimbot` settings (FOV, Segments, Points) reasonably.