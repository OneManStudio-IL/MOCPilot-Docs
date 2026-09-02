---
id: RecoveryHubFirmware
title: 集线器固件恢复
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# 集线器固件恢复

当集线器在固件更新中断或失败后无法正常启动时，需要使用集线器固件恢复。

恢复期间，MOCPilot 会修复集线器固件路径，使集线器可以再次更新到最新支持的固件。仅当集线器无法正常响应、MOCPilot 显示恢复模式或之前的固件更新失败时，才使用此过程。

:::warning 重要
在整个恢复过程中保持集线器开机，并让设备靠近集线器。上传固件时断开 Bluetooth、关闭 MOCPilot、取出电池或关闭集线器，可能导致恢复失败。
:::

## 何时需要恢复

以下情况可能需要固件恢复：

- 固件更新未成功完成。
- 集线器不再作为普通集线器连接。
- 集线器在 MOCPilot 中显示为 **LEGO Bootloader**。
- MOCPilot 检测到集线器以固件恢复模式连接。

开始恢复前，请确保集线器有足够电量。如果可能，也请确保运行 MOCPilot 的设备已充电并启用 Bluetooth。

## 受支持的集线器

固件恢复支持与固件更新相同的集线器：

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(160px, 1fr))', gap: '16px', margin: '16px 0 24px'}}>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_hub_p.webp')} alt="Technic Hub" style={{maxWidth: '140px'}} />
    <div><strong>Technic Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/city_hub_p.webp')} alt="City Hub" style={{maxWidth: '140px'}} />
    <div><strong>City Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/boost_hub_p.webp')} alt="Boost Hub" style={{maxWidth: '140px'}} />
    <div><strong>Boost Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_move_hub_p.webp')} alt="Technic Move Hub" style={{maxWidth: '140px'}} />
    <div><strong>Technic Move Hub</strong></div>
  </div>
</div>

## 将 Technic Hub、Boost Hub 和 City Hub 置于恢复模式

Technic Hub、Boost Hub 和小型 City Hub 使用 bootloader 连接流程：

1. 关闭集线器。
2. 按住绿色按钮。
3. 持续按住按钮，直到集线器 LED 开始闪烁紫色。
4. LED 闪烁紫色时不要松开按钮。
5. 继续按住按钮，同时在 MOCPilot 中打开 **我的蓝牙集线器** 并连接到集线器。
6. 集线器以 bootloader 模式连接后，可以松开按钮。

集线器处于恢复模式时，可能会显示为 **LEGO Bootloader**，而不是普通集线器名称。

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="LEGO Bootloader" />

## 将 Technic Move Hub 置于恢复模式

Technic Move Hub 使用不同的恢复模式顺序。它不会作为 **LEGO Bootloader** 连接，而是加载出厂固件版本 **1.2.3**；该版本不适合作为日常使用的最终固件。

恢复 Technic Move Hub 固件：

1. 关闭集线器。
2. 按住绿色按钮。
3. 按住绿色按钮约一分钟。
4. 松开按钮。
5. 等待集线器 LED 开始闪烁白色。
6. 在 MOCPilot 中打开 **我的蓝牙集线器** 并连接到集线器。

集线器连接后，MOCPilot 会检测到出厂固件，并提示将集线器更新到最新可用版本。启动固件更新并等待完成。

## 从对话框启动恢复

当 MOCPilot 检测到以固件恢复模式连接的集线器时，应用会显示恢复对话框。

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_1.png')} alt="集线器固件恢复" />

选择 **恢复** 开始向集线器上传固件。

如果还没有准备好开始恢复，请选择 **取消**。之后可以从集线器上下文菜单启动恢复。

## 从集线器菜单启动恢复

手动启动恢复：

1. 打开 **我的蓝牙集线器**。
2. 找到显示为 **LEGO Bootloader** 的集线器。
3. 打开集线器上下文菜单。
4. 选择 **恢复集线器固件**。

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="恢复集线器固件" />

## 固件恢复期间

恢复开始后，MOCPilot 会将固件上传到集线器。应用会在屏幕上显示进度。

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_3.png')} alt="集线器固件恢复" />

等待过程完成。请不要将集线器移离设备、关闭应用、关闭 Bluetooth 或切断集线器电源。

过程中集线器可能会重启或重新连接几次。这是正常现象。保持 MOCPilot 打开并等待恢复完成。

## 完成恢复

恢复成功完成后，MOCPilot 会显示确认对话框。

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_4.png')} alt="集线器固件恢复" />

选择 **OK**。集线器应会重启，并作为普通集线器重新连接，而不是 **LEGO Bootloader**。

恢复完成后，请在 **我的蓝牙集线器** 中检查集线器。如果 MOCPilot 仍提示需要固件更新，请运行正常的[固件更新](/docs/Application/Hubs/FirmwareUpdating/)流程。

## 如果恢复失败

如果恢复没有成功完成：

1. 让集线器靠近你的设备。
2. 重启集线器电源。
3. 再次将集线器置于恢复模式。
4. 在 MOCPilot 中连接到 **LEGO Bootloader**。
5. 再次启动 **恢复集线器固件**。

如果再次出现更新失败消息，请从头重复恢复过程。如果多次尝试后仍无法恢复集线器，请更换电池或充电后再试。
