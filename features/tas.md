---
icon: stopwatch
---

# TAS (Tool-Assisted Speedrun) 辅助加速工具 ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)

KRX Client 旗舰版中的 **TAS** 标签页是一个测试功能，专为高级辅助游戏设计，可实现精确和可重复的输入操作。
为获得最流畅的 TAS 体验，我们建议在加入服务器时使用 `/showall` 命令。
*注意：此功能目前正在重做中，未来功能可能会发生变化。*

---

## **Screenshot 界面截图**
![TAS菜单](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/tas-menu.png)

---
## **TAS 基础功能**
- **Enable**: 激活TAS并将你传送到TAS世界
- **TPS (Ticks Per Second)**: 调整工具辅助输入的刻度率(Teeworlds默认TPS: 50)
- **Dummy Replay**: 在TAS模式下启用分身支持
- **Player Prediction**: 将其他玩家添加到TAS世界
- **Ignore Start Warnings**: 在TAS开始时抑制警告消息
- **Stop Mouse When Paused**: TAS暂停时禁用鼠标输入，允许合法运行
- **Use Rewind Input**: 设置鼠标输入以匹配回退输入，使回放更真实
- **Show Real Aim**: 在TAS回放期间显示实际瞄准方向

---

## **Tools 工具**
- **Auto Rewind**: 自动回退到冰冻前的最后一个安全刻度
- **Auto Forward**: 自动前进到解冻前的第一个刻度
- **Rewind Ticks**: 设置回退的刻度数(默认: 1刻度)
- **Forward Ticks**: 设置前进的刻度数(默认: 1刻度)
- **Pause**: 自动回退或前进后暂停TAS
- **Step**: 精确回退或前进一个刻度，可以为每个刻度选择精确的移动

---

## **Fake Aim 假瞄准**
- **Enable**: 激活假瞄准模式以实现欺骗性瞄准
- **Mode**: 选择假瞄准类型(如机器人瞄准)

---

## **Auto Replay 自动回放**
- **Enable**: 自动加载并重新开始回放
- **Reset on Freeze**: 冰冻时重新开始回放
- **Kill on Reset**: 回放结束时杀死玩家

---

## **God Mode 上帝模式**
- **Super**: 在TAS世界中切换RCON命令`super`
- **Weapon**: 允许你给自己武器(由于已知问题，忍者除外)
- **Give Weapon**: 授予选定的武器

---

## **Hotkeys 快捷键**
- **Enable TAS**: 分配按键以激活TAS
- **Record Replay**: 分配按键以开始录制回放
- **Load Replay**: 分配按键以加载回放
- **Respawn TAS**: 分配按键以在TAS模式下重生
- **Pause TAS**: 分配按键以暂停TAS
- **Rewind TAS**: 分配按键以在TAS中回退
- **Forward TAS**: 分配按键以在TAS中前进

---

## **Additional Options 附加选项**
- **Replays Folder**: 打开存储TAS回放的文件夹
- **Load/Save**: 加载或保存回放
- **Continue**: 从选定回放的最后一个刻度继续播放
- **Custom Name Field**: 使用自定义名称保存回放(如`my_tas`)

---

## **FAQ 常见问题**
1. **Q: 为什么我在TAS中看不到武器？**  
   **A:** 你没有运行`/showall`命令。

2. **Q: 为什么地图更换后我无法继续我的运行？**  
   **A:** 很遗憾，跨地图继续不受支持。停止录制，在其他服务器加入地图，然后从那里继续。

3. **Q: 这些像`Verify TAS Integrity failed...`的警告是什么？**  
   **A:** 这些警告是为了确保TAS运行顺畅。通常可以忽略它们，但它们有助于调试问题—如果遇到问题请与我们分享。

4. **Q: 为什么我的TAS在运行中失败了？**  
   **A:** TAS失败通常是由于延迟造成的。使用适当的`cl_prediction_margin`设置，并从正确的起始位置重新开始回放。如果问题持续存在，请联系支持。

5. **Q: 为什么我在TAS中无法移动？**  
   **A:** 很可能是TAS被暂停或`krx_tasrespawn`设置为1。取消TAS暂停或在控制台运行`krx_tasrespawn 0`来解决这个问题。

6. **Q: 为什么进入TAS时我什么都看不到？**  
   **A:** 你需要重生。使用重生快捷键来解决这个问题。

7. **Q: 为什么我无法回退或前进？**  
   **A:** 你需要在TAS中开始录制才能使用回退或前进。如果启用了单步回退/前进，更改可能太微妙而无法注意到—如果需要请禁用它。
