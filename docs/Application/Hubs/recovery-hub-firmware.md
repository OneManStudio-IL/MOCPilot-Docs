---
id: RecoveryHubFirmware
title: Recovery hub firmware
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Recovery hub firmware

Hub firmware recovery is used when a hub cannot start normally after an interrupted or failed firmware update.

During recovery, MOCPilot restores the hub firmware path so the hub can be updated to the latest supported firmware again. Use this process only when the hub is not responding normally, when MOCPilot shows that the hub is in recovery mode, or when a previous firmware update failed.

:::warning Important
Keep the hub powered on and keep your device close to the hub during the whole recovery process. Disconnecting Bluetooth, closing MOCPilot, removing batteries, or turning off the hub while firmware is being uploaded may cause the recovery to fail.
:::

## When recovery is required

Firmware recovery may be required if:

- A firmware update did not finish successfully.
- The hub no longer connects as a normal hub.
- The hub appears as **LEGO Bootloader** in MOCPilot.
- MOCPilot detects that the hub is connected in firmware recovery mode.

Before starting recovery, make sure the hub has enough battery power. If possible, also make sure the phone, tablet, or computer running MOCPilot is charged and Bluetooth is enabled.

## Supported hubs

Firmware recovery is supported for the same hubs as firmware updating:

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

## Put Technic Hub, Boost Hub, and City Hub into recovery mode

Technic Hub, Boost Hub, and the small City Hub use the bootloader connection flow:

1. Turn the hub off.
2. Press and hold the green button.
3. Keep holding the button until the hub LED starts blinking purple.
4. Do not release the button while the LED is blinking purple.
5. While still holding the button, open **My Bluetooth Hubs** in MOCPilot and connect to the hub.
6. After the hub is connected in bootloader mode, you can release the button.

When the hub is in recovery mode, it may appear as **LEGO Bootloader** instead of its normal hub name.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="LEGO Bootloader hub in the hub list with recover firmware action" />

## Put Technic Move Hub into recovery mode

Technic Move Hub uses a different recovery mode sequence than the other supported hubs. It does not connect as **LEGO Bootloader**. Instead, this recovery sequence loads the factory firmware version **1.2.3**, which is not intended as the final firmware for normal use.

To restore Technic Move Hub firmware:

1. Turn the hub off.
2. Press and hold the green button.
3. Keep holding the green button for about one minute.
4. Release the button.
5. Wait until the hub LED starts blinking white.
6. Open **My Bluetooth Hubs** in MOCPilot and connect to the hub.

After the hub connects, MOCPilot will detect the factory firmware and offer to update the hub to the latest available firmware version. Start the firmware update and wait until it finishes.

## Start recovery from the dialog

When MOCPilot detects a hub connected in firmware recovery mode, it shows a recovery dialog.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_1.png')} alt="Hub recovery mode detected dialog" />

Select **Recover** to start uploading firmware to the hub.

If you are not ready to start recovery, select **Cancel**. You can start recovery later from the hub context menu.

## Start recovery from the hub menu

To start recovery manually:

1. Open **My Bluetooth Hubs**.
2. Find the hub shown as **LEGO Bootloader**.
3. Open the hub context menu.
4. Select **Recover hub firmware**.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="Recover hub firmware action in the hub context menu" />

## During firmware recovery

After recovery starts, MOCPilot uploads firmware to the hub. The app shows the progress on screen.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_3.png')} alt="Firmware recovery progress screen" />

Wait until the process is complete. Do not move the hub far away from your device, close the app, disable Bluetooth, or remove power from the hub.

The hub may restart or reconnect several times during the process. This is expected. Keep MOCPilot open and wait for the recovery to finish.

## Finish recovery

When the recovery finishes successfully, MOCPilot shows a confirmation dialog.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_4.png')} alt="Firmware recovery finished dialog" />

Select **OK**. The hub should restart and reconnect as a normal hub instead of **LEGO Bootloader**.

After recovery is complete, check the hub in **My Bluetooth Hubs**. If MOCPilot still reports that a firmware update is required, run the normal [Firmware updating](/docs/Application/Hubs/FirmwareUpdating/) process.

## If recovery fails

If recovery does not finish successfully:

1. Keep the hub close to your device.
2. Power-cycle the hub.
3. Put the hub into recovery mode again.
4. Connect to **LEGO Bootloader** in MOCPilot.
5. Start **Recover hub firmware** again.

If the update failed message appears again, repeat the recovery procedure from the beginning. If the hub still cannot be recovered after several attempts, replace or recharge the batteries and try again.
