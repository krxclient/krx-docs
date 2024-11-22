---
icon: robot
---

# Fent Bot 芬特机器人 ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)

KRX Client 的 **Fent Bot** 标签页提供了通过路径寻找和隧道挖掘来实现自动化的高级工具。
*注意：使用防冻机器人时，请根据你的延迟设置更高的 `cl_prediction_margin` 值，具体请参考[设置](../settings.md)*

---

## **界面截图**
![芬特机器人菜单](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/fentbot-menu.png)

---

## **Avoid 防冻基础**
- **Player Prediction**: 启用其他玩家移动轨迹的预测
- **Advanced Settings**: 解锁机器人行为的高级自定义选项
- **Use Skibidiforce**: 激活Skibidiforce算法以实现高级路径寻找
  - **Skibidiforce Depth**: 配置Skibidiforce计算的深度
- **Fent Ticks**: 定义基于fent的路径寻找的刻度持续时间
- **Tweaker Inputs**: 调整器输入的数量
- **Tweaker Ticks**: 调整调整器输入的刻度持续时间
- **Inject Fent**: 一键开始扫描

## **Misc 杂项**
- **Skibidiforce Aim Points**: 配置Skibidiforce使用的瞄准点数量
- **Render Path**: 视觉显示计算出的路径
- **Render Tunnels**: 高亮显示用于路径寻找的隧道
- **Spectate Scan**: 允许在扫描过程中观察扫描进度
- **Tunnel Editor**: 提供手动自定义隧道的用户界面
- **Auto Tunnels**: 从已加载的回放自动生成优化移动的隧道
- **Tunnel Width**: 调整自动生成隧道的宽度
- **Clear Tunnels**: 清除所有隧道

---

## **Configuration 配置说明**
- 大多数情况下使用KRX提供的默认设置就足够了。以下是针对拥有高性能CPU的进阶用户的可能配置：
- **Player Prediction**: 关闭
- **Advanced Settings**: 开启
- **Use Skibidiforce**: 开启
- **Skibidiforce Depth**: 4
- **Fent Ticks**: 1000
- **Tweaker Inputs**: 最大值
- **Tweaker Ticks**: 4-8
