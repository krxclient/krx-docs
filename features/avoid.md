---
icon: shield
description: >-
    Discover the Avoid feature in KRX Client, an advanced Gores Bot system that prevents
    freezing in Teeworlds. Learn about different bot types, including Legit, Blatant,
    and Fentbot, for optimal movement.
---

# Gores Bot

The **Avoid** feature provides several types of Gores Bots designed to help you avoid freezing in Teeworlds maps. These bots automate certain inputs to keep your character safe.

- **Console Bind**: You can toggle the currently selected Avoid bot using a key bind in the F1 console: `bind KEY toggle krx_avoidfreeze 1 0` (replace `KEY` with your desired key).
- **Important Note on Prediction**: When using *any* Avoid bot, it's crucial to configure your prediction settings appropriately based on your ping. Set `cl_prediction_margin` in the F1 console to a value slightly higher than your average ping (e.g., `cl_prediction_margin 70` for 50ms ping). Refer to the [Settings](settings.md) page for more details.

---

## **Screenshot**
![Avoid Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/avoid-menu.png)
*(Note: The specific options visible below the dropdown depend on the selected Gores Bot Type).*

---

## **Gores Bot Types**
In KRX, you can select different Gores Bot agents, each with its own strategy and configuration:

1.  **Basic** ![Free](https://img.shields.io/badge/Free-%234CAF50?style=flat-square) ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
    -   A simple bot included in Free and Premium tiers. Uses only directional keys (left/right) for basic freeze avoidance. No configurable settings. Suitable for simple situations.
2.  **[Legit](goresbot/legit.md)** ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
    -   Designed for players who want assistance while maintaining a natural, "legitimate" playstyle. It subtly modifies inputs to avoid freeze but relies partially on user skill and can sometimes fail. Highly configurable priority settings. May impact performance on some systems.
3.  **[Blatant](goresbot/blatant.md)** ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
    -   A highly effective bot focused on safety above all else. Uses more aggressive input changes (including hook) to prevent freezing, even on extremely difficult maps. Offers detailed configuration for movement, aiming, and tile avoidance.
4.  **[Fentbot](goresbot/fentbot.md)** ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
    -   An advanced, experimental bot using pathfinding (FlowField) and potentially genetic algorithms ("Tweaker") to calculate input sequences for completing parts or entire maps, primarily KoG-style maps. Runs calculations asynchronously. Highly configurable but resource-intensive and may produce suboptimal paths.

---

Use the dropdown menu in the client's Avoid tab to select the desired bot type. Detailed configuration options for Legit, Blatant, and Fentbot are available in their respective sub-sections linked above.
