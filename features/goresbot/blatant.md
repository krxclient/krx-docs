---
icon: fire
---

# Blatant 明显防冻机器人 ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)

KRX Client 的**明显**防冻机器人专门设计用于帮助你应对各种难度的防冻地图，从简单到极限。
*注意：使用防冻机器人时，请根据你的延迟设置更高的 `cl_prediction_margin` 值，具体请参考[设置](../settings.md)*

---

## **界面截图**
![明显防冻菜单 - 推荐设置](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/blatant-menu.png)

---

## **Avoid 防冻基础**
- **Enable**: 激活防冻功能
- **Player Prediction**: 预测其他玩家的移动轨迹
- **NSIF**: 高级功能，追踪之前的输入序列，当当前明显输入持续时间不够长时切换到NSIF
- **Afk Protection**: 当用户在指定的**Afk Time**后被检测为挂机时，自动禁用防冻机器人
  - **Afk Time**: 以秒为单位可配置

## **Settings 设置**
- **Hook Assistance**: 激活防冻机器人的钩子输入
- **Direction Assistance**: 启用防冻机器人的方向输入
- **Check Ticks**: 指定明显扫描预测的未来时间范围
- **Kick in Ticks**: 决定当前输入的最小生存时间，低于此值时明显模式不会激活
- **Action Ticks**: 类似检查刻度但应用于明显扫描期间的单个动作

## **Ratelimiting 速率限制**
- **Enable**: 启用各种动作的速率限制
- **Hook/Unhook**: 限制钩子和解钩动作的频率
- **Direction/No Direction**: 控制方向相关的速率限制
- **Hook Check**: 仅在不使用钩子时应用方向限制
  - **Hook Ticks**: 设置钩子速率限制的持续时间(以刻度为单位)
  - **Unhook Ticks**: 定义解钩速率限制的持续时间(以刻度为单位)
  - **Move Ticks**: 配置方向移动的速率限制持续时间
  - **Stand Ticks**: 调整静止动作的速率限制持续时间

## **Misc 杂项**
- **Drag Support**: 为自瞄提供额外数据，帮助避免可能导致角色冰冻的方向
- **Track Point**: 追踪当前方向，如果可钩，则在整个扫描持续时间内将其作为目标
- **Rehook Action**: 在明显扫描中考虑重新钩住的场景
- **Safe Aim Tracking**: 仅在追踪的方向在整个扫描持续时间内保持有效时才进行追踪
- **Tile Distance**: 调整避免区块的大小，旨在使明显动作看起来更合法

## **Tiles 区块**
- **Teles**: 避开传送区块
- **Unfreeze**: 避开解冻区块
  - **Ticks**: 可配置解冻区块的检查持续时间
- **Death**: 避开死亡区块

## **Aimbot 自瞄**
- **Enable**: 激活防冻自瞄
- **Auto Aim**: 扫描所有方向并选择最长可行的方向
- **Aim Assist**: 瞄准最接近你鼠标且保持最长有效时间的方向
- **Upward Aim**: 优先选择持续时间最长的向上方向
- **Points**: 指定每个段落要评估的点数
- **Segments**: 定义要扫描的段落数
- **FOV**: 可配置的瞄准视角范围
- **Check Ticks**: 调整自瞄计算的扫描持续时间

## **Visuals 视觉效果**
- **Track Point**: 视觉显示追踪点
- **Aimbot**: 高亮显示自瞄目标点
- **Path**: 显示机器人当前跟随的路径

## **Configuration 配置说明**
- 配置这个机器人并不简单，你需要实验每个设置，以下是一些基础配置供你开始：
- **NSIF**: 开启
- **Hook Assistance**: 开启
- **Direction Assistance**: 开启
- **Check Ticks**: 26
- **Kick in Ticks**: 20
- **Action Ticks**: 26
- **Drag Support**: 开启
- **Track Point**: 开启
- **Rehook Action**: 开启
- **Safe Aim Tracking**: 为了最大安全性开启，否则关闭
