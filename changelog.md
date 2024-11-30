---
icon: rocket
---

# Список изменений

На этой странице задокументированы все основные изменения проекта.

Формат основан на [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), и в этом проекте используется \[MAJOR.MINOR], вдохновленный [Semantic Versioning](https://semver.org/spec/v2.0.0.html), без `PATCH` для простоты.

## \[1.27] - 2024-11-17

### Добавлено

* Quick stop. 🛑✨
* Silentwalk hook. 🎣🔇

### Изменено

* Memory size is now only displayed while recording (Ultimate version only). 💾📊

### Исправлено

* Fentbot crashing when spectating. 👀🔧
* TAS crashing when spectating. 🎮⚙️
* Teleport gun prediction issues. 🔫📌
* Teleports not working in TAS. 🌌🎮
* Auto drag issues. 🎣🔨

> 🚫❓ _Bans? Never heard of 'em. We run the game now._ 🎮👑

***

## \[1.26] - 2024-11-10

### Добавлено

* Silent walk exploit (hides direction & jump arrows + invisible hook). 🚶‍♂️🔇
* Auto unfreeze with customizable FOV and silent options. ❄️👀

### Изменено

* Misc menu improvements. 🛠️📋
* Enhanced bullet and aim lines menu with translation support. 🌐🎯
* Improved prediction lines in TAS. 🎮📈

### Удалено

* Special weapons (shotgun, laser) from the free version. 🔫🚫
* Herobrine. 👻

### Исправлено

* Weapon cursor not showing in TAS. 🎮🔧
* Fake aim settings missing from the menu. 🎯🛠️
* Fall prediction settings missing from the menu. 📉👤

***

## \[1.25] - 2024-11-03

### Добавлено

* Colored ping circles. 🟢🟡🔴
* Fast input. ⚡⌨️
* Advanced settings for prediction adjustments. 🔧🎯
* TAS mode saves current input and resumes upon exit, simulating AFK behavior. 🕰️🎮
* Additional auto unfreeze settings. ❄️🔄
* Complete menu rework! 🎨📋

### Изменено

* Updated to the latest DDNet candidate. 🔄📥
* Enhanced features HUD. 📊🎮

### Исправлено

* Resolved "No finish found" spam with the name changer. 🛠️👤
* Aimbot issues on noby fng. 🎯🔧
* Hammer aimbot bugs. 🔨🎯
* Autofire glitches. 🔥🛠️
* Freeze bars not displaying correctly on fng. ❄️🎮
* Auto aled firing randomly. 🛠️

***

## \[1.24] - 2024-10-19

### Добавлено

* Grenade aimbot. 🎯💥
* Balance bot target locking. 🎯🤖

### Изменено

* Updated client to DDNet 18.7. 🔄🎮
* Improved aimbot. 🚀🔄
* Enhanced clarity for TAS prediction lines. 📊
* Smoother forward/rewind in TAS. ⏩⏪
* Optimized performance to reduce FPS drops from bots. ⚙️🎮

### Исправлено

* Bot functionality (aimbot, auto unfreeze, etc.) after previous crashes. 🐞🤖
* TAS handling of bad starting positions. ⏪🎮
* Weapon firing when rewinding in TAS mode. 🔫⏪
* Autofire bugs. 🔥🔧
* Auto shoot rehooking randomly. 🎯🔧

***

## \[1.23] - 2024-09-22

### Заметка

* Этот релиз содержит секретные обновления и улучшения. 🤫🔒

***

## \[1.22] - 2024-08-04

### Добавлено

* Change name on finish bot. 🏁🔄
* Auto team with auto-lock functionality. 🤖🔒
* Anti-AFK feature. 💤❌
* Kill on freeze feature. ❄️💀
* Suspicious player detection. 🔍⚠️
* Hook nearest collision. 🪝🔄
* Custom theme support. 🎨
* Random name/clan generator. 🔄🆕
* Name/clan converter to fancy name/clan. ✨🆔
* Balance bot hotkey for hooked players. ⚖️🎯
* Global settings for prediction (tele, player collision check, death tiles, move restriction). 🌐⚙️
* Useful binds section (currently includes 45-degree aim bind). 🤖🔄
* Rainbow tee & rainbow hook. 🌈
* Balance bot for hooked-only players. ⚖️
* Auto jump bot. 🤖🆙
* 45-degree aim bind. 🎯🏹

### Изменено

* Updated client to DDNet 18.4. 🔄
* Updated spoof version min and max numbers. 🔄
* Renamed hotkeys to settings. 🔄⚙️
* Improved random ID functionality in ID stealer. 🆔🔄
* Enhanced mod detection capabilities. 🛡️🔍

### Исправлено

* Fake aim mode robot aim issues. 🤖🔧
* DDNet prediction bug with jump tiles in tutorial maps. 🛠️🦘
* Tee falling in stuck tiles. 🛠️⬇️
* Replay issues in free/premium versions. 🔧📹
* Fake aim inconsistencies. 🎯🔧 [Video](https://streamable.com/u6r31m)
* Fake ping inaccuracies. 📶🔧
* Display \[MOD] in red in the scoreboard when mod is detected. 📊🔴
* Display \[WARN] in yellow in the scoreboard when a suspicious player is detected. 📊🟡

### Premium/Ultimate функции

#### Добавлено

* Show real aim in TAS. 🎯🏁
* TAS continues on saved replay. ▶️📹
* Tutorial button in TAS menu. 📚🎯
* Replay folder shortcut in TAS menu. 📁📹
* TAS uses rewind input (uses input at current tick for legit gameplay). ⏪🎮
* TAS integrity verification for recorded inputs. ✅🎯
* TAS basic sounds and effects. 🗣️📢
* Auto aled, dummy fly, and jet ride in the menu. 🛠️🛫
* Separate config values for blatant/legit bot. ⚙️🆕
* Pause after rewind/forward in TAS. ⏸️⏪⏩
* Wall-only laser setting. 🔫🧱
* God mode features in TAS (super, give weapons). 🦸🔫
* TAS stop mouse functionality when paused. ⏸️🐭

#### Changed

* Increased prediction lines length in TAS. 📏🔄

#### Fixed

* Legit bot issues. 🎯🔧
* Game-breaking bug in KRX prediction. 🛠️🧩
* How player prediction works for avoid functionality. 🔧🧠
* Improved rendering of prediction lines in TAS. 🎨📈
* TAS variables (load, record, pause, etc.) no longer save. 📝🚫
* TAS simulation stops further when rewinding/forwarding. ⏪⏩🚫
* Player prediction for gores bot (previously didn't remove all players). 🔧🧠
* TAS prediction lines now work for every tee. 🎨📈

***

## \[1.21] - 2024-07-19

### Добавлено

* Option to hide features HUD. 🖥️
* Fake ping functionality. 📶

### Changed

* Updated client to DDNet 18.3.1. 🆕
* Reorganized KRX menus for better navigation. 🗂️
* Improved ID Stealer (now includes the option to steal emote). 🔄
* Improved ban-logs for better analysis. 📊
* Huge improvement in bot speed. 🚀

### Исправлено

* Aimbot target box issues. 🎯
* Various crashes and bugs. 🛠️
* Wibble wobble bug. 🤫🧏‍♂️

### Premium/Ultimate функции

#### Добавлено

* TAS to the menu. 🏁
* Replay saving to TAS (stored in "appdata/krxclient.xyz/replays"). 🎥
* Dummy support in TAS (might be broken sometimes; try shorter maps first). 🗺️
* Auto forward in TAS (automatically forwards when frozen until unfrozen). ❄️➡️
* "Unlimited" replays in TAS (RAM-dependent; up to 1000 hours on 32GB). ♾️
* TAS fake aim (modifies unused inputs based on the fake aim mode). 🎯
* TAS starting conditions verification (weapons, position, strong/weak hook) + option to ignore. ✔️
* Basic pathfinding (work in progress). 🗺️

#### Исправлено

* Auto-aled issues. 🔧
* Memory leak with avoid freeze. 🧠
* HUD features in TAS (freezebars, etc.). 📊
* Checkpoint teleports in TAS. 🚏
* Aim locking in TAS. 🔒
* Auto-rewind in TAS. ⏪

***

## \[1.20] - 2024-02-18

### Изменено

* Updated client to DDNet 18.0.3. 🔄
* Enhanced avoid freeze functionality. 🚫🆓

### Исправлено

* Minor bugs and glitches. 🐞🔧

***

## \[1.19] - 2024-01-21

### Добавлено

* Fake angles for better spinbot functionality. 🌀🤖️

### Изменено

* Updated client to DDNet 17.4.2. 🔄🎮

### Исправлено

* Minor bug fixes. 🐞🔧

***

## \[1.18] - 2023-11-26

### Изменено

* Improved Balance Bot significantly. ⚖️🚀
* Enhanced bypass for DDNet detection. 🕶️✅️

### Исправлено

* Auto Hook issues. 🪝🔧
* Laser aimbot bugs. 🔫🔧️
* Resolved FNG crashes. 🚫🛠️️

***

## \[1.17] - 2023-11-19

### Добавлено

* **KoG Tab**:
  * Frozen tee display. 👕🔍
  * Render all custom-colored feet as white feet skin. 🦶🎨
  * Alert when you're the last player. ⚠️🏃
  * Auto verify feature. ✅
  * Show cursor in spectate mode. 🖱️👀
  * Prediction margin in freeze. ❄️🔮
* **Profiles Tab**:
  * Custom user profiles support. 👥📁
* Improved Laser Aimbot for better targeting accuracy. 🔫🎯🔄
* Reintroduced Herobrine. 👻

### Изменено

* Updated client to DDNet 17.4. 🔄
* Improved HUD for better in-game visibility. 🖥️🔍
* Enhanced Spinbot visibility, making spins much more noticeable to other players. 🔄🌪️

### Исправлено

* Balance Bot issues. ⚖️🔧

### Безопасность

* Bypassed DDNet automatic detection. 🕶️
* Bypassed DDNet mass spam detection. 📣🚫

***

## \[1.16] - 2023-07-04

### Добавлено

* Ability to edit killsays via "killsays.json" in the data folder. ✏️

### Исправлено

* Client launch issues for some users. 🛠️️

***

## \[1.15] - 2023-07-03

### Добавлено

* Avoid Freeze functionality restored. ❄️
* Fancy Chat Font. ✨
* Killsay/Deathsay feature. 🔪💀
* Mass Mention Spam. 📣📣📣

### Изменено

* Improved Replay Bot visuals. 🔄📷

### Исправлено

* Minor bugs and glitches. 🐞🔧

***

## \[1.14] - 2023-06-29

### Добавлено

* Allowed Hook Ride in KoG. 🪝🎢
* Aimbot use in FNG with FOV limitation to 10. 🚫🎯

### Изменено

* Updated client to DDNet 17.0.3. 🔄

### Исправлено

* Aimbot FOV bug. 🎯🔧
* Vulkan-related crashes. 🖥️💥

### Удалено

* Avoid Freeze feature. ❌

***

## \[1.13] - 2023-01-21

### Изменено

* Enhanced bypass for DDNet detection. 🕶️

***

## \[1.12] - 2023-01-15

### Добавлено

* Rainbow Menu works in-game. 🌈

### Изменено

* Updated client to DDNet 16.7.1. 🔄

### Исправлено

* Minor fixes. 🔧

***

## \[1.11] - 2023-01-08

### Добавлено

* Rainbow Menu. 🌈

### Изменено

* Updated client to DDNet 16.6. 🆕
* Improved sound effects. 🔊
* Improved Aimbot. 🎯
* Improved Balance Bot. ⚖️
* Improved Avoid Freeze functionality. ❄️

### Исправлено

* Client detection on some servers. ✅
* Minor bugs. 🐞

### Удалено

* Disabled Aimbot on FNG. 🚫
* Edge Aimbot. ❌
* KRX Chat. 🗑️
* Laser Unfreeze Bot. 🗡️
* Auto Edge. ⛔
* Herobrine. 👻

***

## \[1.10] - 2021-12-31

### Добавлено

* Version Spoofer. 🎭

### Изменено

* Updated client to DDNet 15.8. 🔄

***

## \[1.09] - 2021-11-22

### Добавлено

* Laser Unfreeze Bot. 🔫❄️
* Avoid Freeze Bot. ❄️🔒
* Auto Edge Bot. 🔄🪜
* Fall Prediction. 🕒

### Изменено

* Aim Lines improvements. 🎯🔧
* Balance Bot improvements. ⚖️🔧
* Updated client to DDNet 15.6.2. 🔄

***

## \[1.08] - 2021-08-08

### Добавлено

* KRX Chat. 💬
* Hook Ride Bot. 🪝🎢

***

## \[1.07] - 2021-06-22

### Добавлено

* Force Edge. ⚡

### Изменено

* Updated client to DDNet 15.5.4. 🔄
* Enhanced bypass for fokkonaut's anti-bot. 🕶️

***

## \[1.06] - 2021-06-13

### Изменено

* Updated client to DDNet 15.5.1. 🔄
* Aimbot now only works when hooking/firing. ⚙️
* Improved Aimbot menu. 🎯🔧

### Исправлено

* General Aimbot bugs. 🎯🔧

### Удалено

* FNG Mode. ❌

***

## \[1.05] - 2021-06-01

### Добавлено

* Basic Replay Bot with a 30-second time limit. 🔄⏳
* Setting to disable occasional ads. ⚙️🚫

### Исправлено

* Status checking. ✅

### Удалено

* Auto-reply ads. ❌

***

## \[1.04] - 2021-05-06

### Добавлено

* Spinbot. 🔄🌀

### Исправлено

* General Aimbot bugs and improvements. 🎯🔧

***

## \[1.03] - 2021-04-29

### Добавлено

* Hook Spam. 🪝🔥
* Chat Repeater Min Length. 💬⤵️
* Draw Aim Lines. 🎯🔧🔳
* Draw Bullet Lines. 🔫🔧🔳

### Изменено

* Reduced Ads. 🚫

***

## \[1.02] - 2021-04-21

### Добавлено

* Super Dyncam. 🔄📷
* Pixel Walk. 🔄🚶

***

## \[1.01] - 2021-04-15

### Добавлено

* Aim on Hook Only. 🔄🪝
* Zoom Hack. 🔄🔍
