---
id: FirmwareUpdating
title: Firmware updating
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Firmware updating

MOCPilot can update firmware on supported LEGO Powered Up hubs when a newer compatible firmware version is available.

Firmware updates may be required before a hub can work correctly with MOCPilot. Newer firmware can improve compatibility, fix hub behavior, and make sure the app can use the features expected for that hub model.

## Supported hubs

Firmware updating is currently supported for these hubs:

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

## Before you start

Make sure the hub and the device running MOCPilot have enough battery power before starting the update.

Keep the hub powered on during the whole process. Keep your phone, tablet, or computer close to the hub so the Bluetooth connection stays stable. Do not close MOCPilot, turn off Bluetooth, or power off the hub while firmware is being uploaded.

:::warning Important
Interrupting a firmware update may leave the hub firmware in an incomplete state. If that happens, the hub may need firmware recovery before it can be used again.
:::

## Starting the update

When you connect a hub, MOCPilot checks the firmware version installed on the hub. If the app detects that a newer firmware version is required, it shows a firmware update dialog.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_1.png')} alt="Firmware update required dialog" />

Select **Update** to start the firmware update immediately.

If you do not want to update right away, select **Cancel**. You can start the update later from the hub context menu.

## Updating later from the hub menu

To start the firmware update manually:

1. Open **My Bluetooth Hubs**.
2. Find the hub that needs updating.
3. Open the hub context menu.
4. Select **Update firmware**.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_2.png')} alt="Update firmware action in the hub context menu" />

## During the firmware update

After the update starts, MOCPilot uploads the firmware to the hub and shows the update progress.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_3.png')} alt="Firmware update progress screen" />

Wait until the upload is complete. The hub may restart or temporarily disconnect while the new firmware is being applied.

After the firmware is uploaded, MOCPilot searches for the hub again. Keep the hub nearby and wait for the app to reconnect.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_4.png')} alt="Firmware uploaded and searching for hub" />

## Finishing the update

When the update finishes successfully, MOCPilot shows a confirmation dialog.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_5.png')} alt="Firmware update finished dialog" />

Select **OK**. The hub will reconnect, and the hub card will show the updated firmware version.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_6.png')} alt="Hub card showing updated firmware version" />

You can now continue using the hub with MOCPilot.

## If the update fails

If the update does not finish successfully, MOCPilot shows a firmware update failed message.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_7.png')} alt="Firmware update failed dialog" />

First, try to power-cycle the hub and run the firmware update again:

1. Turn the hub off.
2. Turn the hub on again.
3. Keep the hub close to your device.
4. Connect to the hub in MOCPilot.
5. Start the firmware update again.

If the hub does not respond normally, firmware recovery may be required. Follow the [Recovery hub firmware](/docs/Application/Hubs/RecoveryHubFirmware/) guide for detailed recovery instructions.
