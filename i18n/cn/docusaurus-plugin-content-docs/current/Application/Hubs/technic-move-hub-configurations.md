---
id: TechnicMoveHubConfigurations
title: Technic Move Hub 配置
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Technic Move Hub 配置

## 概述

Technic Move Hub 在 LEGO Powered Up hub 系列中引入了一项独特功能：hub 可以根据当前应用的配置改变自身行为。

MOCPilot 允许你更改 Technic Move Hub 配置，使 hub 的行为匹配你想控制的官方 LEGO 套装。

## 支持的配置

目前已知以下 Technic Move Hub 配置：

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="设置 Hub 配置 积木中的 Technic Move Hub 配置选项" />

## 从我的 Bluetooth Hub 更改配置

你可以从 **我的 Bluetooth Hub** 页面更改配置：

1. 打开 **我的 Bluetooth Hub**。
2. 找到 Technic Move Hub。
3. 打开 hub 上下文菜单。
4. 选择 **选择配置**。
5. 选择所需配置。
6. 确认重新配置对话框。

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="带有 选择配置 操作的 Technic Move Hub 上下文菜单" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Technic Move Hub 配置子菜单" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Technic Move Hub 重新配置确认对话框" />

:::warning 重要
更改 hub 配置会向 hub 刷写一个子程序，这个过程类似于固件更新。

在整个过程中保持 hub 开机。保持手机、平板或电脑有电并靠近 hub，以便蓝牙连接保持稳定。配置更改期间不要关闭 MOCPilot、关闭 Bluetooth 或关闭 hub 电源。

中断配置更改可能会损坏 hub 固件。如果发生这种情况，hub 可能需要先进行固件恢复才能再次使用。如需恢复，请按照 [hub 固件恢复](/docs/Application/Hubs/RecoveryHubFirmware/) 指南操作。
:::

重新配置期间，hub 不会响应普通命令。它的 LED 会以阶梯式彩色指示闪烁，直到过程完成。新配置应用后，hub 会重新初始化。

## 配置积木

MOCPilot 还提供用于在程序中读取和更改 Technic Move Hub 配置的积木。

### 设置 Hub 配置

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="设置 Hub 配置 积木" />

**设置 Hub 配置** 积木会将所选 hub 更改为其支持的配置档案之一。

- Hub 选择器：选择要重新配置的 hub。
- 配置选择器：选择目标配置。
- Technic Move Hub 可用配置：**Porsche GT4 e-Performance**、**Lamborghini Revuelto** 和 **Batmobile™ Tumbler**。

请参阅 [设置 Hub 配置 积木文档](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config)。

### Hub 配置

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Hub 配置 报告积木" />

**Hub 配置** 积木会报告所选 hub 的当前配置。

- Hub 选择器：选择要读取的 hub。
- 输出格式：**文本** 返回配置名称。
- 输出格式：**索引** 返回配置索引，适合在条件比较中使用。

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Hub 配置 积木输出格式选项" />

请参阅 [Hub 配置 积木文档](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config)。

### 电源脉冲

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Technic Move Hub 电源脉冲积木" />

**电源脉冲** 积木会向所选 Technic Move Hub 发送电源脉冲命令。此积木仅在 Technic Move Hub 配置为 **Batmobile™ Tumbler** 时工作。

运行时，hub 会以最大可用功率和速度短时间启动电机，通常约 1-2 秒。

请参阅 [电源脉冲 积木文档](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse)。

## 程序运行期间更改配置

也可以在程序运行时更改 Technic Move Hub 配置。

常用方法如下：

1. 读取当前 hub 配置。
2. 将其与档案所需配置进行比较。
3. 如果配置不同，则设置所需配置。
4. 重新配置后再次读取配置。
5. 仅当 hub 报告预期配置时才继续。
6. 如果未应用所需配置，则断开连接或停止程序。

使用此 hub 的预置档案可作为这种实现方式的参考。

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="展示运行时更改 Technic Move Hub 配置的积木示例" />
