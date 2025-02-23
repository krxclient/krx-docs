---
icon: sparkles
description: >-
    Explore the Miscellaneous features of KRX Client, including automation tools,
    protections, trolling features, and mod detection. Enhance your Teeworlds gameplay
    with bots, auto-unfreeze, fake aim, and more.
---

# Misc

The **Misc** tab in KRX Client offers a range of tools and features designed to enhance gameplay, provide protections, and enable fun trolling mechanics.

---

## **Screenshot**
![Misc Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/misc-menu.png)

---

## **Features**

### **Bots**
- **Moonwalk**: Makes the player do a "moonwalk" when pressing both left and right keys by switching the movement direction back and forth.  
- **Auto Fire**: Automatically fires your weapon when holding the fire button.  
- **Auto Rehook**: After successfully hooking a player, if you keep holding the hook button, it automatically tries to rehook them.  
- **Auto Jump Save**: Automatically jumps to avoid going into freeze.  
- **Quick Stop**: Stops the player quickly and smoothly by adjusting movement direction to counter their current velocity.  
- **Avoid Freeze**: Helps avoid freeze zones by using left/right movement.  
- **Dummy Fly**: Your dummy automatically does hook fly with you, making the dummy hammer and hook too. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Jet Ride**: Works like hook ride bot but with a jetpack. Control it with A/W/S/D. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Auto Aled**: Automatically hammers when an aled is possible. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  

### **Protections**
- **Random Timeout Seed**: Generates a new timeout seed before connecting to a server to avoid fingerprinting. Note: You cannot rejoin your old position after timing out with this enabled.
- **Version Spoofer**: Spoofs the client version/ID to bypass restrictions. If unsure, leave it off.

### **Mod Detector**  
- **Enable**: Turns on the Mod Detector feature to identify potential moderators or suspicious players on the server.  
- **Detect by Names**: Scans player names for known moderators.  
- **Detect Suspicious Players**: Scans player names to detect potential moderators or players who could report you.  
- **Leave on Mod Detection**: Automatically disconnects from the server if a potential moderator is detected.  
- **Leave on Warn Detected**: Automatically disconnects from the server if a potential moderator or player who could report you is detected.  

### **Auto Unfreeze** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Enable**: Activates the Auto Unfreeze feature, which automatically shoots a laser at a wall to unfreeze you when you jump through freeze zones.
- **Advanced Settings**: Enables more detailed configuration options for precise control.
    - **Bounces**: Determines how the laser bounces off walls:
        - **Least**: Selects a direction with the fewest bounces, ensuring quicker unfreezing.
        - **Most**: Selects a direction with the most bounces. Useful in TAS scenarios, as longer bounces result in faster reload times.
    - **Silent**: Makes aim adjustments invisible on your screen while remaining visible to others.
    - **Points**: Configures the number of points considered when checking for unfreeze directions. Higher values provide more precise checks.
    - **Current Dir Ticks**: Sets how many ticks of the laser are used to calculate the current direction. Adjust for better accuracy.
    - **Ticks**: Defines how many ticks of the laser are analyzed when determining the best unfreeze direction.
    - **FOV**: Adjusts the field of view to determine the laser's targeting range.

### **Fake Aim**
- **Enable**: Turns on fake aim behavior to confuse or mislead other players.
- **Send Always**: If enabled, the aim direction will be sent every tick to the server (looks smoother for others).
- **Visible**: Shows the fake aim on your screen.
- **Modes**: Determines how the fake aim behaves:
  - **Mouse Pos**: Adjusts your aim to follow your mouse position, making the gores bot aimbot appear less blatant.
  - **Robot Aim**: Updates your aim position only when hooking or firing.
  - **Spinbot**: Rotates your aim rapidly in a spinning motion.
  - **Random**: Moves your aim in random directions.
  - **Fake Angles**: Aims in the opposite direction of your cursor.
  - **Aimbot Troll Aim**: Always aims at the closest player.

### **Other**
- **Change Name on Finish**: Automatically changes your name just before crossing the finish line.
- **Auto Team**: Automatically joins the selected team and locks it.
- **Anti AFK**: Prevents being marked as AFK.
- **Kill on Freeze**: Kills your player automatically when you get frozen.
- **Fast Input**: Makes your input feel 1 tick faster (20ms), but this is only a visual effect.
- **Ignore Replay Warnings**: Suppresses warning messages related to TAS replays.
- **Hide Chat Bubble**: Hides the chat bubble so other players don’t know when you are typing.
- **Auto Verify**: Automatically verifies you on whitelist-protected servers like `ger10.ddnet.tw`.
- **Send Occasional Ads**: Sends occasional advertisements in chat.

### **Troll**
- **Emote Spam**: Spams random emotes as fast as possible.
- **Killsay/Deathsays**: Sends pre-defined messages upon kills or deaths.
- **Fancy Chat Font**: Changes your chat font for a unique appearance.
- **Mass Mention Spam**: Mentions multiple players repeatedly.
- **Chat Repeater**: Automatically repeats another player's chat message with alternating uppercase and lowercase letters (e.g., "MeSsAgE").

### **ID Stealer**
- **Enable**: Activates the ID Stealer feature, allowing you to copy another player’s information.
- **Closest Player**: If enabled, targets the closest player to copy their details. If disabled, selects a random player on the server.
- **Steal Name**: Copies the targeted player’s name.
- **Steal Clan**: Copies the targeted player’s clan name.
- **Steal Skin**: Copies the targeted player’s skin.
- **Steal Flag**: Copies the targeted player’s country flag.
- **Steal Eye Emote**: Copies the targeted player’s eye emote expression.
- **Stealer Speed**: Adjusts the interval (in seconds) for how frequently the feature updates the stolen details.

### **Ghost Move**
- **Enable**: Activates the Ghost Move feature, which hides certain indicators to make your actions less noticeable to other players.
- **Direction**: Hides the directional arrows that show your movement direction.
- **Jump**: Hides the jump arrow, making it harder for others to see when you’re jumping.
- **Hook**: Spams an invisible hook at your aim direction. Keep in mind that hook reach is limited.
- **Hook Closest**: Spams an invisible hook at the closest player. Keep in mind that hook reach is limited.

---

## **Configuration**

For most use cases, it's worth enabling the following features:
- **Auto Fire**: Automatically fires your weapon, making it easier to focus on aiming and movement.
- **Avoid Freeze**: Especially useful when playing gores maps, this feature helps you avoid freeze zones.
- **Quick Stop**: Great for block maps, this helps you stop quickly and precisely.
- **Auto Jump Save**: A situational feature to prevent falling into freeze; enable it when needed.
- **Mod Detector**: Use this if you're worried about being watched or banned by moderators.
- **Fast Input**: Many users say this is a game-changer for improving responsiveness, so give it a try.
- **Auto Verify**: A quality-of-life feature that automates verification for DDOS-protected servers. It’s worth keeping enabled for convenience.

Adjust these features depending on your specific gameplay needs, and experiment to find the best combination for your style.
