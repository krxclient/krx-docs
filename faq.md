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
Download the official KRX Client *only* from our website: [krxclient.xyz](https://krxclient.xyz). Always extract the downloaded `.zip` file into a **new, separate folder** before running. Do **not** place KRX files inside your standard DDNet folder or overwrite existing DDNet files.

### **Is KRX Client safe to use?**
Yes, the official client downloaded from `krxclient.xyz` is safe. We use protection methods (like Themida) to prevent reverse-engineering, which unfortunately causes many antivirus programs (including Windows Defender) to show **false positive** warnings (detecting it as a virus, trojan, etc.). You may need to temporarily disable your antivirus or add an exception for the KRX folder/executable to install and run it. **Never download KRX from unofficial sources, as those may contain actual malware.**

### **Is KRX Client open source?**
No, it’s a closed-source project. This helps protect its features and prevents the quick development of detection methods by servers.

### **What are the system requirements?**
We recommend Windows 10 or 11 (64-bit). While Linux might work with Wine, it's not officially supported. Older Windows versions (like Windows 7) are **not supported** due to missing dependencies. A CPU with at least 4 cores and 8GB RAM is recommended for smoother performance, especially when using advanced bot features.

---

## Installation and Setup

### **How do I install the client?**
1.  Download the `.zip` file from [krxclient.xyz](https://krxclient.xyz).
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
3.  Replace `KEY` with your desired key (e.g., `x`, `mouse2`, `ctrl`).
4.  Replace `COMMAND` with the feature's command variable (e.g., `krx_avoidfreeze` for Avoid Freeze, `krx_aimbot` for Aimbot). You can find many bindable commands listed in the in-game Settings -> Controls -> KRX menu.
5.  Example: `bind x toggle krx_avoidfreeze 1 0` binds the 'X' key to toggle Avoid Freeze.

### **Why don't I see/pick up weapons in TAS?**
You need to enable rendering for all entities *before* starting TAS.
1.  Type `/showall` in the **in-game chat** (not the F1 console).
2.  Also ensure weapon prediction is enabled in your client settings: Settings -> DDNet -> Antiping -> Enable 'Predict weapons'.
3.  Sometimes, restarting the map (`/map mapname`) after using `/showall` but before starting the TAS process can help ensure it takes effect.

### **My TAS replay fails/breaks/desyncs. How to fix?**
TAS relies on predicting game ticks precisely. Network lag or certain map features can cause failures.
1.  **Increase Prediction Margin:** Open the F1 console and type `cl_prediction_margin 200` (or higher, e.g., 300, depending on your ping and server stability). This helps compensate for lag.
2.  **Check Map Compatibility:** Maps with server-side randomization (like multiple teleporter exits with the same ID or complex stoppers) can break TAS prediction and may be inherently unreliable for TAS playback.
3.  **Enable Teleport Prediction:** If the map uses teleporters, go to the KRX TAS settings menu and ensure 'Teleport Prediction' is enabled.
4.  **Ensure Stable Ping:** TAS works best with low, stable ping. High or fluctuating ping is a common cause of failure.

### **Why does Legit Avoid Freeze cause FPS drops/lag?**
Legit Avoid performs complex calculations, which can impact performance on some systems, especially with many players nearby. To improve performance:
1.  **Lower Settings:** Reduce 'Check Ticks' (try 4-6), 'Quality' (try ~50), and maybe 'Randomness' in the Legit Avoid menu.
2.  **Disable Prediction:** Turn off 'Player Prediction' in the Avoid settings if you don't need it for your current task.
3.  **Try Configs:** Check our [Discord](https://discord.gg/MwzsHadQAe) for community-shared configurations that might be optimized for performance.

---

## Troubleshooting

### **Error: GET: SSL connect error / Failed to retrieve version / Failed to check status**
This usually indicates a network issue blocking connection to the KRX authentication servers.
1.  **Use a VPN:** Connect via a VPN (try different servers/countries like Germany) *before* launching KRX. This often resolves regional blocks or network filtering.
2.  **Check Installation:** Ensure KRX is extracted to its own folder and *not* placed inside the official DDNet folder or overwriting DDNet files.
3.  **Check DNS:** If you previously used a *cracked* client, it might have altered your DNS. Reset your system's DNS settings to "Automatic" or use a public DNS like `1.1.1.1` or `8.8.8.8`.

### **Error: HWID verification failed**
This means the client is locked to a different PC hardware configuration than the one currently detected.
1.  **Use Website Reset:** Log in to `krxclient.xyz`, go to your Profile/Dashboard, and click "Reset HWID". You can do this **once every 7 days**. This is the standard solution for changing PCs or after significant hardware changes/OS reinstalls.
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
You can view pricing options on our homepage [krxclient.xyz](https://krxclient.xyz/) and detailed plans after logging in at [krxclient.xyz/pricing](https://krxclient.xyz/pricing). We accept several methods:
*   **Credit/Debit Card & PayPal:** Securely processed via Paddle directly on our website.
*   **Cryptocurrencies:** Processed via **Coinbase Commerce** or **NowPayments** on our website (accepts various cryptos like LTC, BTC, ETH, etc. - LTC often has the lowest transaction fees).
*   **Resellers:** Authorized regional resellers may offer local payment methods. Find the current list after logging in at [krxclient.xyz/resellers](https://krxclient.xyz/resellers) or check our [Discord server](https://discord.gg/MwzsHadQAe).

### **I paid but didn't receive my license key?**
License keys are typically emailed instantly after payment confirmation.
1.  **Check Spam/Junk Folder:** Ensure the email didn't land there.
2.  **Wait 15-30 Minutes:** Allow for potential payment processing and email delivery delays.
3.  **Check Payment Status:** Ensure your payment was fully completed and confirmed by the provider (Paddle, Coinbase, NowPayments, or Reseller).
4.  **Contact Support:** If the key still hasn't arrived, open a ticket on our [Discord](https://discord.gg/MwzsHadQAe) with your payment details (Order ID, email used for purchase, transaction ID if crypto).

### **Can I get a free trial or discount?**
We generally do not offer free trials outside of announced special events (like the occasional Free Weekend). Discounts may be available during promotional periods – check the announcements on our [Discord](https://discord.gg/MwzsHadQAe).

### **How do I get the Premium/Ultimate role on Discord?**
After purchasing and activating your license:
1.  Open a ticket on our [Discord server](https://discord.gg/MwzsHadQAe) using the appropriate "Get Role" option in `#create-a-ticket`.
2.  Provide a **full, uncropped screenshot** of your dashboard on `krxclient.xyz` showing:
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
- Email: support@krxclient.xyz (Response times may be slower)
- Telegram: [Join Here](https://t.me/joinchat/4sp4Mduuf0RiZGM0) (Community chat, less suitable for direct support)