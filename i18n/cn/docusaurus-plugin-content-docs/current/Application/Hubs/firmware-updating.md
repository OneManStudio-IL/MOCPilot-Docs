---
id: FirmwareUpdating
title: 固件更新
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# 固件更新

当有新的兼容固件版本可用时，MOCPilot 可以更新受支持 LEGO Powered Up 集线器上的固件。

固件更新可能是让集线器正确配合 MOCPilot 工作的必要步骤。较新的固件可以提升兼容性、修正集线器行为，并启用该型号应有的功能。

## 受支持的集线器

目前支持为以下集线器更新固件：

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

## 开始之前

开始前，请确保集线器以及运行 MOCPilot 的手机、平板或电脑都有足够电量。

在整个过程中保持集线器开机，并让设备靠近集线器以保持 Bluetooth 连接稳定。固件上传期间请不要关闭 MOCPilot、关闭 Bluetooth 或切断集线器电源。

:::warning 重要
中断固件更新可能会让集线器固件处于不完整状态。如果发生这种情况，集线器可能需要先进行固件恢复才能再次使用。
:::

## 开始更新

连接集线器时，MOCPilot 会检查已安装的固件版本。如果需要较新的版本，应用会显示固件更新对话框。

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_1.png')} alt="固件更新" />

选择 **更新** 可立即开始固件更新。

如果不想立即更新，请选择 **取消**。之后可以从集线器上下文菜单启动更新。

## 稍后从集线器菜单更新

手动启动固件更新：

1. 打开 **我的蓝牙集线器**。
2. 找到需要更新的集线器。
3. 打开集线器上下文菜单。
4. 选择 **更新固件**。

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_2.png')} alt="更新固件" />

## 固件更新期间

更新开始后，MOCPilot 会将固件上传到集线器并显示进度。

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_3.png')} alt="固件更新" />

等待上传完成。应用新固件时，集线器可能会重启或暂时断开连接。

固件上传后，MOCPilot 会再次搜索集线器。请让集线器保持在附近，并等待应用重新连接。

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_4.png')} alt="固件更新" />

## 完成更新

更新成功完成后，MOCPilot 会显示确认对话框。

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_5.png')} alt="固件更新" />

选择 **OK**。集线器会重新连接，集线器卡片会显示更新后的固件版本。

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_6.png')} alt="固件更新" />

现在可以继续在 MOCPilot 中使用该集线器。

## 如果更新失败

如果更新未能成功完成，MOCPilot 会显示固件更新失败消息。

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_7.png')} alt="固件更新" />

首先尝试重启集线器电源，然后再次运行固件更新：

1. 关闭集线器。
2. 再次打开集线器。
3. 让集线器靠近你的设备。
4. 在 MOCPilot 中连接集线器。
5. 再次启动固件更新。

如果集线器无法正常响应，可能需要进行固件恢复。请按照[集线器固件恢复](/docs/Application/Hubs/RecoveryHubFirmware/)指南中的详细说明操作。
