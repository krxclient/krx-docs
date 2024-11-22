---
icon: gear
---

# Settings 设置

KRX Client 的**设置**标签页允许你配置快捷键并微调特定功能以提升游戏体验。

---

## **界面截图**
![设置菜单](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/settings-menu.png)

---

## **Hotkeys 快捷键**
- **Aimbot**: 切换自瞄功能的开关
- **Aimbot Auto Hook**: 自瞄启用时自动钩住目标
- **Aimbot Auto Shoot**: 自瞄启用时自动射击目标
- **Balance Bot**: 切换平衡机器人以保持角色平衡
- **Emote Spam**: 启用连续表情刷屏
- **Hook Spam**: 启用快速钩子刷屏
- **Super DynCam**: 启用动态相机的无限缩放
- **Pixel Walk**: 使用方向键时允许逐像素精确移动
- **Hook Nearest Collision**: 自动钩住最近的碰撞点
- **Quick Stop**: 不按任何方向键时立即抵消移动以实现最快停止
- **Hook Ride (risky)**: 激活钩子骑乘机器人
- **Record Replay**: 开始记录玩家输入
- **Load Replay**: 加载之前记录的输入
- **Avoid Freeze**: 激活机器人以帮助避开冰冻区域
- **Auto Edge**: 启用机器人自动落在冰冻、死亡或传送区域附近的边缘 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Laser Unfreeze Bot**: 激活机器人使用激光自动解除冰冻状态 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Avoid Auto Drag**: 此功能激活时自动钩住最近的角色而不被冰冻 ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
- **Avoid Track Points**: 切换明显防冻机器人的高级点位追踪。详见[明显防冻机器人](./goresbot/blatant.md) ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)

---

## **Settings 设置**
- **Teleport Prediction**: 为TAS或防冻机器人启用传送预测，否则传送会被替换为冰冻 ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
- **Advanced Settings**: 解锁高级预测设置以微调所有KRX机器人获得最大优势: ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
   - **Death Tile Prediction**: 为机器人预测死亡区域，包括TAS和防冻机器人。否则会忽略死亡区域
   - **Move Restrictions Prediction**: 预测空中阻挡。禁用此项可显著提升机器人性能
   - **Player Loop**: 预测角色之间的碰撞。禁用此项只会移除碰撞处理并可显著提升机器人性能
   - **Prediction Margin**: 调整预测边际。更高的值使你受延迟峰值影响更小，但可能使其他人看起来更卡顿
- **Balance Bot Offset**: 配置平衡机器人保持平衡的反应灵敏度。更高的值会减少移动校正
- **Hook Nearest FOV**: 设置**Hook Nearest Collision**功能的视角范围

---

## **Configuration 配置说明**

1. 打开KRX Client中的**设置**标签页
2. 根据个人喜好为功能分配自定义快捷键
3. 根据游戏需求调整设置。以下是一些**推荐配置**:
   - **Teleport Prediction**: 建议保持禁用，除非使用TAS。使用防冻机器人时不要启用 ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
   - **Advanced Settings**: 建议禁用，除非你清楚知道自己在做什么 ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
      - **Death Tile Prediction**: 建议禁用因为会降低机器人速度，但对TAS有用
      - **Move Restrictions Prediction**: 建议在休闲游戏时启用。禁用可显著提升机器人性能
      - **Player Loop**: 建议在休闲游戏时启用。禁用可显著提升机器人性能
      - **Prediction Margin**: 根据你的延迟选择值(例如，50ms延迟设置~50)。建议设置更高的值(>20)以避免机器人问题
   - **Balance Bot Offset**: 建议值: ~2
   - **Hook Nearest FOV**: 建议设置较低的FOV(例如30)以减少低配CPU的延迟
