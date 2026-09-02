---
id: AboutApp
title: 关于 MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - 拼装它。驾驶它。控制一切。

**MOCPilot** 是一款用于为 LEGO® 和兼容蓝牙动力作品创建自定义控制配置文件的应用。

它为玩家提供一个统一的位置，用来连接 hub、控制电机、读取传感器、设计仪表盘，并为模型、机构、汽车、卡车、火车、机器人和自定义 MOC 创建可视化程序。

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="手机上运行的 MOCPilot 应用" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>MOCPilot 可以提供什么</h2>
    <ul>
      <li>为你自己的模型创建自定义配置文件。</li>
      <li>为受支持的官方套装使用现成配置文件。</li>
      <li>连接和管理 Bluetooth hub。</li>
      <li>用于自动化和逻辑的可视化积木编程。</li>
      <li>用于驾驶和操作模型的仪表盘控制器。</li>
      <li>支持 LEGO® Powered Up、Technic、BuWizz、SBrick、Mould King、电机、传感器以及兼容的蓝牙设备。</li>
    </ul>
  </div>
</div>

## 核心理念

大多数电动模型需要的不只是一个简单遥控器。汽车可能需要转向、油门、灯光、电池监控、变速箱顺序或特殊启动流程。机器人可能需要传感器、事件、条件逻辑，以及多个 hub 协同工作。

MOCPilot 面向基础遥控和完整编程环境之间的空间。你可以先从屏幕仪表盘驾驶模型开始，然后在作品变得更复杂时加入逻辑、传感器和自动化。

## 配置文件

**配置文件** 是一个模型的控制中心。

在配置文件中，你可以选择哪些 hub 属于该模型，创建运行模型的程序，并设计用于控制它的仪表盘。

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="MOCPilot 配置文件页面" width="420" />

<details>
<summary>预置配置文件</summary>

预置配置文件是为受支持官方套装准备好的示例。当你想快速开始，或学习一个可运行配置文件如何搭建时，它们非常有用。

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="MOCPilot 预置配置文件" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="预置 MOCPilot 积木程序" width="1100" />

</details>

<details>
<summary>自定义配置文件</summary>

自定义配置文件用于你自己的 MOC 和实验。你可以创建配置文件、添加 hub、连接电机和传感器、构建程序，并设计与具体模型匹配的控制仪表盘。

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="创建自定义 MOCPilot 配置文件" width="420" />

</details>

## 连接 hub 和设备

MOCPilot 可以连接受支持的 Bluetooth hub 和兼容设备，然后在你的配置文件中使用它们。

简单作品可以只使用一个 hub；当模型需要更多端口、独立供电系统或独立模块时，也可以连接多个 hub。

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="MOCPilot 中的 我的 Bluetooth Hub 页面" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="MOCPilot 中已连接的 Bluetooth hub" width="1100" />

<details>
<summary>受支持硬件示例</summary>

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(140px, 1fr))', gap: '16px', alignItems: 'end', margin: '16px 0'}}>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_hub_p.webp')} alt="LEGO Technic Hub" style={{maxWidth: '130px'}} />
    <div><strong>Technic Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_move_hub_p.webp')} alt="LEGO Technic Move Hub" style={{maxWidth: '130px'}} />
    <div><strong>Technic Move Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/buwizz3_hub_p.webp')} alt="BuWizz 3.0 Pro Hub" style={{maxWidth: '130px'}} />
    <div><strong>BuWizz 3.0</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/sbrick_hub_p.webp')} alt="SBrick Hub" style={{maxWidth: '130px'}} />
    <div><strong>SBrick</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/mould_king_4_p.webp')} alt="Mould King Hub" style={{maxWidth: '130px'}} />
    <div><strong>Mould King</strong></div>
  </div>
</div>

完整列表请参阅[受支持的 hub、电机和传感器](/docs/Introducing/SupportedDevices/)页面。

</details>

## 用积木构建逻辑

MOCPilot 包含可视化积木构建器。你可以通过连接积木创建程序，而不需要编写代码。

积木可以响应事件、控制电机、读取传感器、处理变量、使用手柄输入、更新仪表盘控制器，并协调多个动作。

MOCPilot 完全支持已连接的实体游戏手柄。手柄积木可以读取按钮、扳机、方向键和摇杆，因此当实体控制比触摸屏更适合时，你可以把真实手柄映射到模型。

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="使用积木构建的 MOCPilot 用户程序" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="当程序启动积木" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="按速度启动电机积木" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Hub 电池电量积木" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="方向盘数值积木" />
</div>

<details>
<summary>积木程序可以做什么</summary>

- 启动、停止和转向电机。
- 读取电池电量、电压、倾斜、方向、温度和传感器值。
- 为转向、油门、扳机、动作和模式切换配置实体游戏手柄控制。
- 在按钮、传感器、计时器或仪表盘控制器变化时作出响应。
- 在模型开始移动前创建启动检查。
- 为灯光、转向校准、动力模式和 hub 配置添加自定义逻辑。
- 使用变量、列表、条件、循环、广播和自定义积木组织复杂行为。

</details>

## 设计驾驶仪表盘

仪表盘是你控制模型时使用的屏幕。它可以包含方向盘、摇杆、滑块、按钮、开关、踏板、监视器和其他控制器。

你可以把仪表盘控制器和实体游戏手柄输入连接到积木和 hub 动作，让界面匹配模型，而不是把所有作品都塞进同一种遥控布局。

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="MOCPilot 仪表盘控制器" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="带方向盘和踏板的 MOCPilot 控制屏幕" width="1100" />

<details>
<summary>仪表盘示例</summary>

- 为汽车使用方向盘和踏板。
- 为吊车、升降机构和线性执行器使用滑块。
- 为灯光、喇叭、换挡或脚本动作使用按钮。
- 使用监视器显示电池、速度、传感器值或自定义程序状态。
- 当你更喜欢实体按钮、摇杆和扳机而不是触摸屏控制时，使用已连接的游戏手柄。

</details>

## 让高级作品保持可管理

随着模型变复杂，配置文件也可以一起成长。MOCPilot 通过 **My Blocks** 支持可复用逻辑、针对配置文件的 hub 设置、多个控制器，以及把手动控制与自动化结合起来的程序流程。

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="MOCPilot My Blocks 使用示例" width="1100" />

这有助于让大型程序保持易读。例如，一个配置文件可以有一个用于电池更新的自定义积木、另一个用于转向校准、再另一个用于特殊驾驶模式。

## 典型流程

1. 创建或打开配置文件。
2. 添加模型使用的 Bluetooth hub 和设备。
3. 用积木构建程序。
4. 设计用于驾驶和交互的仪表盘。
5. 按下 **Play**。
6. 测试、调校并改进配置文件，直到模型按你想要的方式运行。

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="MOCPilot 中的 hub 连接流程" width="1100" />

## MOCPilot 适合谁

MOCPilot 适合希望实现以下目标的玩家：

- 为电动 LEGO® 模型获得更好的遥控方式。
- 控制第三方兼容 Bluetooth hub。
- 为机构和机器人使用可视化编程环境。
- 为受支持的官方套装使用预置配置文件。
- 为汽车、卡车、火车、攀爬车、吊车和其他 MOC 创建自定义仪表盘。
- 用一个应用组合 hub、电机、传感器、游戏手柄和屏幕控制器。

## 开始探索

- 按照[快速入门教程](/docs/Introducing/QuickStart/)创建你的第一个配置文件。
- 选择硬件前查看[受支持设备](/docs/Introducing/SupportedDevices/)。
- 准备添加逻辑时，浏览 [BlockBuilder 文档](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/)。
- 如果 hub 需要受支持的固件版本，请查看 [hub 固件更新](/docs/Application/Hubs/FirmwareUpdating/)。
