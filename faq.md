---
icon: book
description: >-
    Find answers to common questions about KRX Client, a bot client for Teeworlds
    built on DDNet. Learn about installation, troubleshooting, payments, feature usage,
    and best practices for using the client effectively.
---

# FAQ

Find answers to frequently asked questions about **KRX Client** below.

**Need a quick answer?** If you have access to ChatGPT, you can try asking our experimental **[KRX Client Support Bot](https://chatgpt.com/g/g-68024c1919908191948a8f9af09aa816-krx-client-support-bot)**.

If your question isn't listed here or the bot can't help, please check the other sections of this documentation or reach out on our [Discord](https://discord.gg/MwzsHadQAe).

---

## General Questions

### **Where can I download the KRX Client?**
Download the official KRX Client *only* from our website: [krxteam.com](https://krxteam.com). Always extract the downloaded `.zip` file into a **new, separate folder** before running. Do **not** place KRX files inside your standard DDNet folder or overwrite existing DDNet files.

### **Is KRX Client safe to use?**
Yes, the official client downloaded from `krxteam.com` is safe. We use protection methods (like Themida) to prevent reverse-engineering, which unfortunately causes many antivirus programs (including Windows Defender) to show **false positive** warnings (detecting it as a virus, trojan, etc.). You may need to temporarily disable your antivirus or add an exception for the KRX folder/executable to install and run it. **Never download KRX from unofficial sources, as those may contain actual malware.**

### **Is KRX Client open source?**
No, it’s a closed-source project. This helps protect its features and prevents the quick development of detection methods by servers.

### **What are the system requirements?**
We recommend Windows 10 or 11 (64-bit). While Linux might work with Wine, it's not officially supported. Older Windows versions (like Windows 7) are **not supported** due to missing dependencies. A CPU with at least 4 cores and 8GB RAM is recommended for smoother performance, especially when using advanced bot features.

---

## Installation and Setup

### **How do I install the client?**
1.  Download the `.zip` file from [krxteam.com](https://krxteam.com).
2.  **Create a new folder** (e.g., on your Desktop).
3.  Extract the contents of the `.zip` file into this new folder.
4.  Run `KRX Client.exe` from inside the extracted folder.
5.  For **Premium/Ultimate**, log in with your KRX **username** (not email) and password.
6.  For more details, see our [Installation Guide](getting-started/installation.md).

### **Why is `KRX Client.exe` missing after extraction?**
Your antivirus software likely quarantined or deleted it due to the false positive mentioned above. Temporarily disable your antivirus/Windows Defender (including Real-time Protection) or add an exclusion for the download/extraction folder, then extract the `.zip` file again.

### **Error: VCRUNTIME140.dll (or similar `.dll`) is missing?**
This means you're missing essential Windows components. Install the latest **Visual C++ Redistributable (x64)** from [Microsoft's official website](https://aka.ms/vs/17/release/vc_redist.x64.exe) and restart your PC. This often fixes errors mentioning `VCRUNTIME` or `api-ms-win-crt` DLLs.

### **KRX Client doesn't start (no error, black screen, process disappears)?**
This is common and can have several causes. Try these steps in order:
1.  **Reset Settings:** Go to `%AppData%\Roaming\DDNet` and rename the `settings_ddnet.cfg` file to `settings_ddnet.cfg_old`. Try launching KRX again. (This resets DDNet settings which KRX uses).
2.  **Install/Repair VC++:** Ensure you have the latest Visual C++ Redistributable installed (see previous point).
3.  **Check Antivirus Thoroughly:** Even if you think it's off, some AVs (especially Windows Defender) can interfere. Double-check real-time protection is off, add exclusions, or consider a tool like 'Defender Control'. Redownload KRX after confirming AV is off.
4.  **Run as Admin:** Right-click `KRX Client.exe` and choose "Run as administrator".
5.  **Check OS:** Ensure you are running a supported Windows version (Win 10/11 64-bit).

---

## Usage & Features

### **How do I use Feature X (Aimbot, Avoid, TAS, etc.)?**
Detailed explanations for all features are available in the respective sections of this documentation. Please use the sidebar navigation to find the feature you're interested in (e.g., under "Features" or "Ultimate Features").

### **How do I bind a key to toggle a feature (e.g., Avoid Freeze)?**
1.  Press `F1` in-game to open the console.
2.  Use the format: `bind KEY toggle COMMAND 1 0`
3.  Replace `KEY` with your desired key (e.g., `x`, `lctrl`).
4.  Replace `COMMAND` with the feature's command variable (e.g., `krx_avoidfreeze` for Avoid Freeze, `krx_aimbot` for Aimbot). You can find many bindable commands listed in the in-game Settings -> Controls -> KRX menu.
5.  Example: `bind x toggle krx_avoidfreeze 1 0` binds the 'X' key to toggle Avoid Freeze.

### **Why don't I see/pick up weapons in TAS?**
You need to enable rendering for all entities *before* starting TAS. There are multiple ways to ensure this:
1.  **In-Game Chat (Manual):** Type `/showall` in the chat (not F1 console) *after* joining the server but *before* starting TAS recording/playback.
2.  **Console (Automatic):** Press `F1` and execute the command `cl_run_on_join "showall 1"`. This makes the client automatically run `/showall 1` every time you join a server.
3.  **DDNet Settings (Automatic):** Go to `Settings -> DDNet -> Miscellaneous -> Run on join` and add `showall 1` to the text field.
Additionally, ensure weapon prediction is enabled in your client settings: `Settings -> DDNet -> Antiping -> Predict weapons`. Sometimes, restarting the map (`/map mapname`) after using `/showall` but before starting TAS can also help ensure it takes effect.

### **My TAS replay fails/breaks/desyncs. How to fix?**
TAS relies on predicting game ticks precisely. Network lag, packet loss, or certain map features can cause the playback to deviate from the recording (desync).
1.  **Increase Prediction Margin:** This is the most common solution. Open the F1 console and type `cl_prediction_margin VALUE` (e.g., `cl_prediction_margin 200` or higher). This value (in milliseconds) tells the client to buffer more time for prediction, making it more resilient to network jitter and slight timing variations between recording and playback. Set it higher than your ping.
2.  **Check Map Compatibility:** Maps with server-side randomization (like multiple teleporter exits with the same ID or complex stoppers/pistons) can inherently break TAS prediction and may be unreliable for playback regardless of client settings.
3.  **Enable Teleport Prediction:** If the map uses standard teleporters, go to the KRX TAS settings menu and ensure 'Teleport Prediction' is enabled (though note this might conflict with some Avoid bot settings).
4.  **Ensure Stable Ping:** TAS works best with low, stable ping. High or fluctuating ping significantly increases the chance of desync.
5.  **Note on Server Checks:** Be aware that some game servers might implement their own anti-TAS mechanisms that could intentionally cause playback failures, even with correct client settings.

### **Why does Legit Avoid Freeze cause FPS drops/lag?**
Legit Avoid performs complex calculations to find subtle, safe movements. This can be CPU-intensive, especially when many other players are nearby (increasing the complexity of the prediction). To improve performance:
1.  **Lower Settings:** Reduce 'Quality' (`krx_avoid_num_iterations`, try ~50-100) and 'Check Ticks' (`krx_avoid_tile_legit_check_ticks`, try 4-8) in the Legit Avoid menu. Maybe also reduce 'Randomness' (`krx_avoid_tile_exploration_constant`).
2.  **Disable Player Prediction:** Turn off 'Player Prediction' in the Avoid settings if not strictly needed.
3.  **Try Configs:** Check the `#configs-and-replays` channel on our [Discord](https://discord.gg/MwzsHadQAe) for community-shared configurations potentially optimized for performance.

---

## Troubleshooting

### **General Connection Fix (Network/SSL errors, Timeout, Could Not Resolve Host, etc.)**

If you get any connection, SSL, or DNS errors when using KRX Client, try these steps first:

1. **Open the [Cloudflare 1.1.1.1 app](https://one.one.one.one/)** and use **‘DNS-only’ mode** (do **NOT** enable WARP mode).
2. If it still doesn't work, try **WARP mode** in the same app.
3. Try turning any other VPN you have ON or OFF.
4. Restart your computer and your router.

*Cloudflare DNS-only mode usually fixes most connection problems without causing game server bans. Only use WARP mode if DNS-only doesn't help.*

### **Error: GET: SSL connect error / Failed to retrieve version / Failed to check status**

This usually means something is blocking your connection to the KRX authentication/status servers.

**First, follow the steps in the “General Connection Fix” section above!**

If you still have issues after that:
1. **Check Installation:** Make sure KRX is in its own folder and *not* inside the official DDNet folder or overwriting DDNet files.
2. **Check DNS:** If you previously used a *cracked* client, it might have changed your system DNS. Reset DNS to "Automatic" or use a public DNS like Cloudflare (`1.1.1.1`, `1.0.0.1`) or Google (`8.8.8.8`, `8.8.4.4`). *(Usually not needed if you use the Cloudflare app.)*

### **Error: HWID verification failed**
This means the client is locked to a different PC hardware configuration than the one currently detected.
1.  **Use Website Reset:** Log in to `krxteam.com`, go to your Profile/Dashboard, and click "Reset HWID". You can do this **once every 7 days**. This is the standard solution for changing PCs or after significant hardware changes/OS reinstalls.
2.  **Wait for Cooldown:** If the button is unavailable, you must wait for the 7-day cooldown period to expire before you can reset it again.
3.  **Avoid Frequent Changes:** Frequent OS reinstalls, using HWID spoofers for other games, or switching PCs often will trigger this. Plan your HWID resets accordingly. KRX Staff generally do not bypass the cooldown.

### **Graphics look blurry / Wrong resolution**
This can happen with high-resolution monitors or certain display scaling settings.
1.  **Check In-Game Settings:** Ensure the correct resolution is selected in Graphics settings. Try switching between Fullscreen/Borderless/Windowed modes and different Renderers (OpenGL/Vulkan).
2.  **Windows DPI Scaling Fix:** Right-click `KRX Client.exe` -> Properties -> Compatibility -> Change high DPI settings -> Check "Override high DPI scaling behavior" and select "Application" from the dropdown. This has resolved the issue for some users.

### **Crash: Vulkan Renderer Issues**
Switch to the **OpenGL** renderer in the Graphics settings. Vulkan can be less stable on some hardware/driver combinations.

### **KRX download button on website doesn't work?**
1.  **Disable Download Managers:** If you use third-party software like IDM, disable it temporarily and use your browser's default downloader.
2.  **Try Different Browser/Clear Cache:** Browser extensions or corrupted cache can interfere. Try an alternative browser or clear your current browser's cache and cookies.
3.  **Use VPN:** In rare cases, regional network issues might affect website scripts. Try accessing the download page via VPN.

---

## Payment and Subscriptions

### **How do I pay? What methods are accepted?**
You can view pricing options on our homepage [krxteam.com](https://krxteam.com/) and detailed plans after logging in at [krxteam.com/pricing](https://krxteam.com/pricing). We accept several methods:
*   **Credit/Debit Card & PayPal:** Securely processed via Paddle directly on our website.
*   **Cryptocurrencies:** Processed via **Coinbase Commerce** or **NowPayments** on our website (accepts various cryptos like LTC, BTC, ETH, etc. - LTC often has the lowest transaction fees).
*   **Resellers:** Authorized regional resellers may offer local payment methods. Find the current list after logging in at [krxteam.com/resellers](https://krxteam.com/resellers) or check our [Discord server](https://discord.gg/MwzsHadQAe).

### **I paid but didn't receive my license key?**
License keys are typically emailed instantly after payment confirmation.
1.  **Check Spam/Junk Folder:** Ensure the email didn't land there.
2.  **Wait 15-30 Minutes:** Allow for potential payment processing and email delivery delays.
3.  **Check Payment Status:** Ensure your payment was fully completed and confirmed by the provider (Paddle, Coinbase, NowPayments, or Reseller).
4.  **Activate Key:** Once you receive the key via email, remember to **activate it on your krxteam.com profile page** under "Activate License".
5.  **Contact Support:** If the key still hasn't arrived after a reasonable time, open a ticket on our [Discord](https://discord.gg/MwzsHadQAe) with your payment details (Order ID, email used for purchase, transaction ID if crypto).

### **Can I get a free trial or discount?**
We generally do not offer free trials outside of announced special events (like the occasional Free Weekend). Discounts may be available during promotional periods – check the announcements on our [Discord](https://discord.gg/MwzsHadQAe).

### **How do I get the Premium/Ultimate role on Discord?**
After purchasing and activating your license:
1.  Open a ticket on our [Discord server](https://discord.gg/MwzsHadQAe) using the appropriate "Get Role" option in `#create-a-ticket`.
2.  Provide a **full, uncropped screenshot** of your dashboard on `krxteam.com` showing:
    *   Your KRX Username (top right).
    *   Your active subscription (Premium or Ultimate) and its expiry date.
    *   The current date and time visible on your computer's taskbar/system clock.
3.  A staff member will review the screenshot and assign the corresponding role.

---

## Community & Policy

### **How can I avoid game server bans (DDNet/KOG)?**
Using any cheat client carries risk. KRX Client can be detected if used blatantly. To minimize detection risk:
*   Use the **Legit** Avoid Freeze mode with conservative settings tailored to your skill level.
*   Avoid highly obvious features like Spinbot, excessive Aimbot FOV, or unnatural movements in public/monitored servers.
*   Use common sense; play smart and don't draw unnecessary attention.
*   **KRX Staff cannot assist with bans issued by game server administrators.**

### **I got IP banned from DDNet/KOG. How do I play again?**
KRX staff cannot lift game server bans. Bypassing IP bans typically involves changing your IP address. Common methods include:
*   **Restarting Router:** Only works if your Internet Service Provider assigns dynamic IPs.
*   **VPN:** Using a high-quality *residential* VPN service is often necessary, as free/datacenter VPNs are usually blocked by DDNet/KOG.
*   **Mobile Data:** Using a mobile hotspot often provides a different, unbanned IP.
*   *Note: Repeated ban evasion can lead to stricter penalties from server admins.*

### **Can I share my KRX account/license?**
**No.** Account sharing is strictly prohibited by our Terms of Service and will result in a ban from using KRX Client. Each license is intended for a single user on their primary machine(s), with periodic HWID resets allowed for legitimate hardware changes.

### **How do I become a Moderator/Reseller/Content Creator?**
*   **Moderator/Reseller:** We are generally **not** actively recruiting for these roles. Any future openings will be announced on our [Discord](https://discord.gg/MwzsHadQAe).
*   **Content Creator:** We have a program for established creators with consistent viewership. Check the guidelines posted in our [Discord](https://discord.gg/MwzsHadQAe) announcements or open a ticket to inquire about current requirements if you have a popular channel (typically requiring 1k+ views on YouTube or 5k+ views on TikTok per video consistently).

---

## Contact Us

- **Primary Support:** Join our [Discord server](https://discord.gg/MwzsHadQAe) and open a ticket in the `#create-a-ticket` channel.
- Email: support@krxteam.com (Response times may be slower)
- Telegram: [Join Here](https://t.me/joinchat/4sp4Mduuf0RiZGM0) (Community chat, less suitable for direct support)