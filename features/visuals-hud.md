---
icon: eye
description: >-
    Customize your game with the Visuals & HUD settings in KRX Client for Teeworlds.
    Learn how to enable aim lines, bullet trails, rainbow effects, and HUD enhancements
    for better gameplay experience.
---

# Visuals & HUD

The **Visuals & HUD** tab in the KRX Client allows you to enhance the visual elements of your game and customize the user interface (HUD) for better clarity, style, and gameplay precision.

---

## **Screenshot**
![Visuals & HUD Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/visuals-hud-menu.png)
*(Note: Screenshot may slightly differ from the latest version).*

---

## **HUD**
*(Overlays displaying specific game information)*
- **Features HUD** (`krx_featureshud`): Displays a customizable overlay showing the status of enabled KRX features (e.g., Aimbot, Avoid).
    - **Opacity** (`krx_featureshudopacity`): Adjusts the background transparency.
    - **Font Size** (`krx_featureshudfontsize`): Adjusts the text size.
    - **Segmented** (`krx_featureshudsegmented`): Renders text character by character for smoother gradient effects.
    - **Gradient Speed** (`krx_featureshudgradientspeed`): Controls the speed of color transition if gradients are used.
    - **Start Color** (`krx_featureshudgradientstartcol`): Starting color for the text gradient.
    - **End Color** (`krx_featureshudgradientendcol`): Ending color for the text gradient.
    - **Rainbow** (`krx_featureshudgradientrainbow`): Overrides start/end colors with a cycling rainbow effect.
- **TAS HUD** ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square) (`krx_tashud`): Displays an overlay with useful information for Tool-Assisted Speedruns (TAS), such as current input, reload timer, jumps remaining, grounded status, etc.
- **Notifications** (`krx_notifications`): Enables on-screen popup notifications in the top-right corner triggered by certain bot actions or events (e.g., warnings, errors, task completion).

## **Miscellaneous Visuals**
- **Rainbow Tee** (`krx_customcolortee` & `krx_customcolorteerainbow`): Applies a cycling rainbow color effect to your tee's body and feet. Requires **Custom Color Tee** to be enabled. Speed controlled by `krx_customcolorrainbowspeed`.
- **Rainbow Hook** (`krx_customcolorhook` & `krx_customcolorhookrainbow`): Applies a cycling rainbow color effect to your hook chain and head. Requires **Custom Color Hook** to be enabled. Speed controlled by `krx_customcolorrainbowspeed`.
- **Trail** (`krx_trail`): Enables a particle trail effect behind your tee. Type and color are configurable.
    - **Type** (`krx_trail_type`): Selects the trail effect (Smoke, Bullet, Powerup, Sparkle, Tater).
    - **Color** (`krx_trail_color`): Sets the base color for the trail (if not Rainbow).
    - **Rainbow** (`krx_trail_color_rainbow`): Overrides the base color with a cycling rainbow effect.
    - **Tater Trail Options**: Additional settings specific to the "Tater" trail type appear if selected (Width, Length, Alpha, Taper, Fade, Color Mode).
- **Rainbow Menu** (`krx_rainbowmenu`): Applies a rainbow color effect to the KRX Client menu interface elements when **Custom Theme** is also enabled.
- **Custom Theme** (`krx_customtheme`): Enables custom coloring for the KRX menu interface.
    - **Accent Color** (`krx_custom_accent_color`): Sets the primary highlight/accent color for menu elements.
    - **Background Color** (`krx_custom_bg_color`): Sets the background color for menu sections.
- **Fall Prediction**: Displays a prediction line showing where your tee will land based on current velocity and gravity (does not account for inputs or collisions).
- **Tile Outlines** (`cl_outline`): Draws outlines around specific tile types (configurable).
    - **Freeze** (`cl_outline_freeze`): Outline freeze/deepfreeze tiles.
    - **Kill** (`cl_outline_kill`): Outline death tiles.
    - **Unfreeze** (`cl_outline_unfreeze`): Outline unfreeze/undeepfreeze tiles.
    - **Teleports** (`cl_outline_tele`): Outline teleporter tiles.
    - **Walls** (`cl_outline_solid`): Outline solid/nohook tiles.
    - **Width/Alpha/Colors**: Further customization for outline appearance.
- **Player Indicator** (`cl_player_indicator`): Shows circles or small tees around your character indicating the direction and status (alive/frozen/saved) of teammates.
    - **Various Options**: Configure size, offset, opacity, team-only display, etc. (see `cl_indicator_*` variables).

## **KoG Specific HUD**
*(Options primarily useful for KoG (Keep Opponent Grounded) gameplay)*
- **Show Frozen HUD** (`cl_frozen_tees_hud`): Displays a dedicated HUD element showing the status of all tees in your team.
- **Use Skins Instead of Ninja Tees** (`cl_frozen_tees_hud_skins`): When frozen, display teammates with their actual skins (darkened) instead of the default ninja skin in the Frozen HUD.
- **Only Show After Joining a Team** (`cl_frozen_tees_only_inteam`): The Frozen HUD only appears once you have joined a team.
- **Max Rows** (`cl_frozen_tees_max_rows`): Adjusts the maximum number of rows used to display tees in the Frozen HUD.
- **Tee Size** (`cl_frozen_tees_size`): Adjusts the size of tee icons within the Frozen HUD.
- **Tees Right Alive Text** (`cl_frozen_tees_text`): Displays text indicating the number of alive or frozen teammates (Mode 1: Alive/Total, Mode 2: Frozen/Total).
- **Show When You Are Last** (`cl_last_notify`): Displays a configurable message on screen when only one player remains unfrozen in your team.
    - **Text** (`cl_last_notify_text`): The message to display.
    - **Color** (`cl_last_notify_color`): The color of the message.
- **Show Cursor in Free Spectate** (`cl_cursor_in_spec`): Renders your mouse cursor even when in free spectator mode.

## **Aim Lines**
*(Visual aids showing potential weapon trajectories)*
- **Draw Aim Lines** (`krx_drawaimlines`): Enables drawing aim assist lines.
- **Self Only** (`krx_drawaimlines_selfonly`): Limits aim lines display to only your own character.
- **Pistol** (`krx_drawaimlines_gun`): Displays aim line for the pistol.
- **Shotgun (Vanilla)** (`krx_drawaimlines_shotgun`): Displays aim lines for the vanilla shotgun spread.
- **Grenade** (`krx_drawaimlines_grenade`): Displays aim line for the grenade launcher trajectory.
- **Laser / Shotgun (DDRace)** (`krx_drawaimlines_laser`): Displays aim line for the laser rifle / DDRace shotgun.
- **Alpha** (`krx_drawaimlines_alpha`): Adjusts the transparency of the aim lines.

## **Bullet Lines**
*(Visual aids showing the path of fired projectiles)*
- **Draw Bullet Lines** (`krx_drawbulletlines`): Enables drawing bullet trajectory lines.
- **Self Only** (`krx_drawbulletlines_selfonly`): Limits bullet trajectory lines display to only your own projectiles.
- **Pistol** (`krx_drawbulletlines_gun`): Displays lines for pistol bullets.
- **Shotgun (Vanilla)** (`krx_drawbulletlines_shotgun`): Displays lines for vanilla shotgun pellets.
- **Grenade** (`krx_drawbulletlines_grenade`): Displays trajectory line for grenades.
- **Alpha** (`krx_drawbulletlines_alpha`): Adjusts the transparency of the bullet lines.

---

## **Configuration**

1. Open the **Visuals & HUD** tab in the client.
2. Customize the settings. Here are some **recommendations**:
   - **Features HUD**: Very useful for keeping track of active bots/features. **Recommended: On**. Configure gradient/segmentation to preference.
   - **TAS HUD**: Essential information when creating or playing back TAS runs. **Recommended: On** during TAS activities.
   - **Notifications**: Helpful feedback from bots. **Recommended: On**.
   - **Trail**: Primarily cosmetic. Can be distracting during gameplay but nice for recordings. Configure type and color/rainbow as desired. Tater trail offers more customization.
   - **Custom Theme / Rainbow Menu**: Personal preference for menu appearance. **Recommended: On** and tweak colors if desired.
   - **Tile Outlines / Player Indicator**: Useful visual aids, especially in complex maps or team modes. Enable and configure based on preference.
   - **KoG Specific HUD**: Enable most options if playing KoG seriously; adjust Max Rows/Tee Size for optimal layout.
   - **Aim/Bullet Lines**: Generally off for casual play to reduce clutter. Useful for TAS, precise weapon practice, or understanding trajectories.
