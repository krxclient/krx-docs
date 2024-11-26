---
icon: fire
---

# Blatant

The **Blatant** Gores bot in KRX Client is expertly designed to help you tackle Gores maps of all kinds, from easy to extreme.\
&#xNAN;_&#x4E;ote: When using avoid bots, please use a higher `cl_prediction_margin` refer to_ [_settings_](../settings.md) _and choose pred margin based on ping_

***

![Рекомендуемые настройки "Blatant"](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/blatant-menu.png)

***

## **Avoid**

* **Enable**: Activates the avoid functionality.
* **Player Prediction**: Predicts the movements of other players.
* **NSIF**: An advanced feature that tracks previous input sequences and switches to NSIF when the current blatant input does not persist long enough.
* **Afk Protection**: Automatically disables the Gores bot when the user is detected as AFK after the specified **Afk Time**.
  * **Afk Time**: Configurable in seconds.

## **Settings**

* **Hook Assistance**: Activates hook inputs for the Gores bot.
* **Direction Assistance**: Enables directional input for the Gores bot.
* **Check Ticks**: Specifies how far into the future blatant scans predict.
* **Kick in Ticks**: Determines the minimum lifespan of the current input for blatant not to activate.
* **Action Ticks**: Similar to check ticks but applied to individual actions during blatant scans.

## **Ratelimiting**

* **Enable**: Enables rate-limiting for various actions.
* **Hook/Unhook**: Limits the frequency of hook and unhook actions.
* **Direction/No Direction**: Controls direction-related rate-limiting.
* **Hook Check**: Applies direction limits only when not hooking.
  * **Hook Ticks**: Sets the duration of hook rate-limiting in ticks.
  * **Unhook Ticks**: Defines the duration of unhook rate-limiting in ticks.
  * **Move Ticks**: Configures rate-limiting duration for directional movement.
  * **Stand Ticks**: Adjusts rate-limiting duration for stationary actions.

## **Misc**

* **Drag Support**: Provides additional data to the aimbot, helping avoid directions that could lead to freezing your tee.
* **Track Point**: Tracks the current direction and, if hookable, targets it for the entire scan duration.
* **Rehook Action**: Considers rehooking scenarios in the blatant scan.
* **Safe Aim Tracking**: Ensures tracking only if the tracked direction remains valid for the entire scan duration.
* **Tile Distance**: Adjusts the size of avoided tiles, designed to make blatant actions appear more legitimate.

## **Tiles**

* **Teles**: Avoids teleport tiles.
* **Unfreeze**: Avoids unfreeze tiles.
  * **Ticks**: Configurable check duration for unfreeze tiles.
* **Death**: Avoids death tiles.

## **Aimbot**

* **Enable**: Activates the avoid aimbot.
* **Auto Aim**: Scans all directions and selects the longest viable one.
* **Aim Assist**: Targets the direction closest to your mouse that remains valid the longest.
* **Upward Aim**: Prioritizes upward directions that persist the longest.
* **Points**: Specifies the number of points to evaluate per segment.
* **Segments**: Defines the number of segments to scan.
* **FOV**: Configurable field of view for targeting.
* **Check Ticks**: Adjusts the duration of scans for aimbot calculations.

## **Visuals**

* **Track Point**: Displays tracked points visually.
* **Aimbot**: Highlights aimbot target points.
* **Path**: Shows the current path followed by the bot.

## **Configuration**

* Configuring this bot is not trivial, you need to experiment with each of these settings, here's some basic configuration to start you off:
* **NSIF**: ON
* **Hook Assistance**: ON
* **Direction Assistance**: ON
* **Check Ticks**: 26
* **Kick in Ticks**: 20
* **Action Ticks**: 26
* **Drag Support**: ON
* **Track Point**: ON
* **Rehook Action**: ON
* **Safe Aim Tracking**: For maximum safety ON, otherwise OFF
