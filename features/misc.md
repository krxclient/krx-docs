---
icon: sparkles
---

# Misc 杂项功能

KRX Client 的**杂项**标签页提供了一系列工具和功能，用于增强游戏体验、提供保护机制以及启用有趣的整活机制。

---

## **界面截图**
![杂项菜单](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/misc-menu.png)

---

## **功能特性**

### **Bots 机器人**
- **Moonwalk**: 当同时按下左右键时，通过来回切换移动方向使角色做"太空步"动作。(头上会同时显示左右方向键)
- **Auto Fire**: 按住开火键时自动持续射击武器，几乎冷却。
- **Auto Rehook**: 成功钩住玩家后，如果继续按住钩子键，会自动尝试重新钩住目标。
- **Auto Jump Save**: 快要落水时，会触发自动跳跃以避免进入冰冻状态。
- **Quick Stop**: 通过调整移动方向来抵消当前速度，使角色快速平稳停止。
- **Avoid Freeze**: 通过左右移动来帮助避免冰冻区域。
- **Dummy Fly**: 你的分身会自动跟随你进行钩子飞行，同时也会使用锤子和钩子。 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Jet Ride**: 类似钩子骑乘机器人但使用的是手枪飞。用A/W/S/D控制。 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Auto Aled**: 当可以进行aled操作时会自动使用锤子。 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)

### **Protections 保护功能**
- **Random Timeout Seed**: 在连接服务器前生成新的超时种子以避免被追踪。注意：启用此功能后，超时后将无法返回原位置。
- **Version Spoofer**: 伪装客户端版本/ID以绕过限制。如不确定请保持关闭。

### **Mod Detector 管理员检测**
- **Enable**: 开启管理员检测功能，用于识别潜在的管理员或可疑玩家。
- **Detect by Names**: 扫描玩家名字以识别已知管理员。
- **Detect Suspicious Players**: 扫描玩家名字以检测潜在的管理员或可能举报你的玩家。
- **Leave on Mod Detection**: 检测到潜在管理员时自动断开服务器连接。
- **Leave on Warn Detected**: 检测到潜在管理员或可能举报你的玩家时自动断开连接。

### **Auto Unfreeze 自动解冻** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Enable**: 激活自动解冻功能，当你穿过冰冻区域时自动向墙壁发射激光以解除冰冻。
- **Advanced Settings**: 启用更详细的配置选项以实现精确控制。
    - **Bounces**: 决定激光如何反弹：
        - **Least**: 选择最少反弹次数的方向，确保更快解冻。
        - **Most**: 选择最多反弹次数的方向。在TAS场景中有用，因为更长的反弹会导致更快的重装时间。
    - **Silent**: 使瞄准调整在你的屏幕上不可见，但对其他人可见。
    - **Points**: 配置检查解冻方向时考虑的点数。更高的值提供更精确的检查。
    - **Current Dir Ticks**: 设置用于计算当前方向的激光刻度数。调整以获得更好的精确度。
    - **Ticks**: 定义分析最佳解冻方向时使用的激光刻度数。
    - **FOV**: 调整视场角以确定激光的目标范围。

### **Fake Aim 假瞄准**
- **Enable**: 开启假瞄准行为以迷惑或误导其他玩家。
- **Send Always**: 启用后，每个刻度都会向服务器发送瞄准方向(对其他人来说看起来更流畅)。
- **Visible**: 在你的屏幕上显示假瞄准。
- **Modes**: 决定假瞄准的行为方式：
  - **Mouse Pos**: 调整瞄准以跟随鼠标位置，使防冻机器人自瞄看起来不那么明显。
  - **Robot Aim**: 仅在钩子或开火时更新瞄准位置。
  - **Spinbot**: 快速旋转你的瞄准方向。
  - **Random**: 随机移动瞄准方向。
  - **Fake Angles**: 瞄准光标相反的方向。
  - **Aimbot Troll Aim**: 始终瞄准最近的玩家。

### **Other 其他功能**
- **Change Name on Finish**: 在通过终点线前自动更改你的名字。
- **Auto Team**: 自动加入选定的队伍并锁定。
- **Anti AFK**: 防止被标记为挂机。
- **Kill on Freeze**: 被冰冻时自动杀死你的角色。
- **Fast Input**: 使你的输入感觉快1个刻度(20ms)，但这只是视觉效果。
- **Ignore Replay Warnings**: 抑制与TAS回放相关的警告消息。
- **Hide Chat Bubble**: 隐藏聊天气泡，使其他玩家不知道你在打字。
- **Auto Verify**: 在需要白名单的服务器(如`ger10.ddnet.tw`)上自动验证。
- **Send Occasional Ads**: 在聊天中偶尔发送广告。

### **Troll 恶搞功能**
- **Emote Spam**: 尽可能快地刷屏随机表情。
- **Killsay/Deathsays**: 击杀或死亡时发送预设消息。
- **Fancy Chat Font**: 更改聊天字体以获得独特外观。
- **Mass Mention Spam**: 重复提及多个玩家。
- **Chat Repeater**: 自动重复其他玩家的聊天消息，使用交替的大小写字母(如"MeSsAgE")。

### **ID Stealer ID窃取器**
- **Enable**: 激活ID窃取功能，允许你复制其他玩家的信息。
- **Closest Player**: 启用时瞄准最近的玩家复制其详细信息。禁用时随机选择服务器上的玩家。
- **Steal Name**: 复制目标玩家的名字。
- **Steal Clan**: 复制目标玩家的战队名称。
- **Steal Skin**: 复制目标玩家的皮肤。
- **Steal Flag**: 复制目标玩家的国家旗帜。
- **Steal Eye Emote**: 复制目标玩家的眼睛表情。
- **Stealer Speed**: 调整更新窃取详细信息的间隔(以秒为单位)。

### **Silent Walk 静默行走**
- **Enable**: 激活静默行走功能，隐藏某些指示器使你的动作不易被其他玩家注意。
- **Direction**: 隐藏显示你移动方向的箭头。
- **Jump**: 隐藏跳跃箭头，使其他人更难看到你何时跳跃。
- **Hook**: 在你的瞄准方向发射不可见的钩子。请注意钩子射程是有限的。
- **Hook Closest**: 向最近的玩家发射不可见的钩子。请注意钩子射程是有限的。

---

## **配置建议**

对于大多数使用场景，建议启用以下功能：
- **Auto Fire**: 自动开火，让你更专注于瞄准和移动。
- **Avoid Freeze**: 特别适用于玩gores地图时，帮助你避开冰冻区域。
- **Quick Stop**: 非常适合gores地图，帮助你快速精确停止。
- **Auto Jump Save**: 情境性功能，用于防止掉入冰冻区域；需要时启用。
- **Mod Detector**: 如果你担心被管理员监视或封禁，请使用此功能。
- **Fast Input**: 许多用户认为这能显著改善响应性，值得一试。
- **Auto Verify**: 自动验证DDOS保护服务器的便利功能。建议保持启用以提高便利性。

根据你的具体游戏需求调整这些功能，通过实验找到最适合你风格的组合。
