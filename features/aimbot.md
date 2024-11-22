---
icon: bullseye-arrow
---

# 自瞄功能

KRX Client 的**自瞄**功能标签页旨在通过提供精确的目标瞄准和丰富的自定义选项来提升你在 Teeworlds 游戏中的竞争优势。
从**高级版**开始,自瞄功能支持所有武器、边缘钩子机制以及高级设置,如榴弹移动预测、边缘精准度和可调节的射击延迟。

---

## **界面截图**
![自瞄菜单](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/aimbot-menu.png)

---

## **功能特性**

- **Enable**: 开启或关闭自瞄功能
- **Draw FOV**: 显示视角(FOV)圆圈,展示自瞄的作用范围
- **FOV Slider**: 调节FOV半径以微调瞄准精度
- **Target Priority**: 决定目标选择方式:
  - **Closest to Crosshair**: 基于与准星的距离选择目标。这个选项确保更精确的识别,但在某些情况下可能影响锤子自瞄的效果
  - **Closest to Player**: 瞄准距离你最近的玩家。适合HvH场景或更激进的游戏风格
- **Silent**: 使自瞄调整在你的屏幕上不可见,但对其他人可见
- **Ignore Friends**: 防止自瞄瞄准好友或队友(用于同队伍情况)
- **Target Box**: 用方框高亮目标(红色表示钩子,橙色表示武器)。适用于PvP模式,但在休闲游戏中可能会分散注意力
- **Target Glow**: 为目标添加发光效果。注意:对纯黑色的tee角色无效
- **Advanced Settings**: 解锁对自瞄行为的额外控制 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Grenade Move Prediction**: 预测目标移动以提高榴弹精度。**注意:** 这个功能对CPU要求较高,不建议在低配电脑上使用 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Edge Accuracy**: 调节边缘钩子精度: ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
  - **较低数值**: 增加失误几率但使动作看起来更自然 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
  - **较高数值**: 提高困难钩子的准确性,即使在挑战性场景中也能保持效果 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Min/Max Shoot Delay**: 模拟按住射击按钮。延迟以刻度计算(1刻度=20毫秒)。在HvH对战中,建议将两者都设为最小值以最大化射击速度 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)

---

## **配置说明**

1. 打开客户端中的**Aimbot**标签页
2. 自定义设置。以下是**推荐的半正常日常游戏设置**:
   - **Enable**: 开启(绑定到按键,例如`LCTRL`)
   - **Draw FOV**: 关闭以减少干扰
   - **FOV Slider**: ~30,在精度和覆盖范围之间取得平衡
   - **Target Priority**: 大多数情况下使用**Closest to Crosshair**。如果遇到锤子自瞄问题,切换到**Closest to Player**
   - **Silent**: 正常游戏时关闭。休闲游戏或追求便利时开启
   - **Ignore Friends**: 在方块或PvP模式中启用,避免瞄准队友
   - **Target Box**: 休闲游戏时关闭以减少干扰;在PvP中开启可以轻松识别目标
   - **Target Glow**: 比Target Box更微妙的选择—根据个人喜好使用
   - **Advanced Settings**: 除非你清楚知道自己在做什么,否则保持关闭 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
   - **Grenade Move Prediction**: 除非你有强劲的CPU且想充分利用KRX榴弹自瞄功能,否则请禁用 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
   - **Edge Accuracy**: 设置为最大以保持钩子稳定性,或调低以显得更自然 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
   - **Min/Max Shoot Delay**: 保持默认设置,除非你清楚知道需要做什么调整 ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
