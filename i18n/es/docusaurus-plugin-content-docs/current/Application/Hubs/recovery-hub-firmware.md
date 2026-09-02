---
id: RecoveryHubFirmware
title: Recuperación del firmware del hub
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Recuperación del firmware del hub

La recuperación del firmware del hub se usa cuando un hub no puede iniciar normalmente después de una actualización de firmware interrumpida o fallida.

Durante la recuperación, MOCPilot restaura la ruta de firmware del hub para que pueda actualizarse de nuevo a la última versión compatible. Use este proceso solo si el hub no responde normalmente, si MOCPilot indica que está en modo de recuperación o si una actualización anterior falló.

:::warning Importante
Mantenga el hub encendido y el dispositivo cerca del hub durante todo el proceso de recuperación. Desconectar Bluetooth, cerrar MOCPilot, retirar las pilas o apagar el hub mientras se carga el firmware puede hacer que la recuperación falle.
:::

## Cuándo se requiere recuperación

La recuperación de firmware puede ser necesaria si:

- Una actualización de firmware no terminó correctamente.
- El hub ya no se conecta como un hub normal.
- El hub aparece en MOCPilot como **LEGO Bootloader**.
- MOCPilot detecta que el hub está conectado en modo de recuperación de firmware.

Antes de iniciar la recuperación, asegúrese de que el hub tenga suficiente batería. Si es posible, asegúrese también de que el teléfono, la tablet o el ordenador con MOCPilot esté cargado y tenga Bluetooth activado.

## Hubs compatibles

La recuperación de firmware está disponible para los mismos hubs que la actualización de firmware:

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

## Poner Technic Hub, Boost Hub y City Hub en modo de recuperación

Technic Hub, Boost Hub y el pequeño City Hub usan el flujo de conexión mediante bootloader:

1. Apague el hub.
2. Mantenga pulsado el botón verde.
3. Siga manteniendo el botón hasta que el LED del hub empiece a parpadear en morado.
4. No suelte el botón mientras el LED parpadea en morado.
5. Sin soltar el botón, abra **Mis hubs Bluetooth** en MOCPilot y conéctese al hub.
6. Cuando el hub esté conectado en modo bootloader, puede soltar el botón.

En modo de recuperación, el hub puede aparecer como **LEGO Bootloader** en lugar de su nombre normal.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="LEGO Bootloader" />

## Poner Technic Move Hub en modo de recuperación

Technic Move Hub usa una secuencia de recuperación distinta a la de los demás hubs compatibles. No se conecta como **LEGO Bootloader**. En su lugar, esta secuencia carga el firmware de fábrica **1.2.3**, que no está pensado como firmware final para uso normal.

Para restaurar el firmware de Technic Move Hub:

1. Apague el hub.
2. Mantenga pulsado el botón verde.
3. Mantenga pulsado el botón verde durante aproximadamente un minuto.
4. Suelte el botón.
5. Espere hasta que el LED del hub empiece a parpadear en blanco.
6. Abra **Mis hubs Bluetooth** en MOCPilot y conéctese al hub.

Después de conectarse, MOCPilot detectará el firmware de fábrica y ofrecerá actualizar el hub a la última versión disponible. Inicie la actualización de firmware y espere a que termine.

## Iniciar la recuperación desde el diálogo

Cuando MOCPilot detecta un hub conectado en modo de recuperación de firmware, muestra un diálogo de recuperación.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_1.png')} alt="Recuperación del firmware del hub" />

Seleccione **Recuperar** para empezar a cargar el firmware en el hub.

Si no está preparado para iniciar la recuperación, seleccione **Cancelar**. Puede iniciar la recuperación más tarde desde el menú contextual del hub.

## Iniciar la recuperación desde el menú del hub

Para iniciar la recuperación manualmente:

1. Abra **Mis hubs Bluetooth**.
2. Busque el hub que aparece como **LEGO Bootloader**.
3. Abra el menú contextual del hub.
4. Seleccione **Recuperar firmware del hub**.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="Recuperar firmware del hub" />

## Durante la recuperación del firmware

Tras iniciar la recuperación, MOCPilot carga el firmware en el hub. La app muestra el progreso en pantalla.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_3.png')} alt="Recuperación del firmware del hub" />

Espere hasta que el proceso termine. No aleje el hub del dispositivo, no cierre la app, no desactive Bluetooth ni quite la alimentación del hub.

El hub puede reiniciarse o reconectarse varias veces durante el proceso. Es normal. Mantenga MOCPilot abierto y espere a que la recuperación termine.

## Finalizar la recuperación

Cuando la recuperación termina correctamente, MOCPilot muestra un diálogo de confirmación.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_4.png')} alt="Recuperación del firmware del hub" />

Seleccione **OK**. El hub debería reiniciarse y conectarse como un hub normal en lugar de **LEGO Bootloader**.

Cuando termine la recuperación, compruebe el hub en **Mis hubs Bluetooth**. Si MOCPilot sigue indicando que se requiere una actualización de firmware, ejecute el proceso normal de [Actualización de firmware](/docs/Application/Hubs/FirmwareUpdating/).

## Si la recuperación falla

Si la recuperación no termina correctamente:

1. Mantenga el hub cerca de su dispositivo.
2. Apague y encienda el hub.
3. Ponga el hub de nuevo en modo de recuperación.
4. Conéctese a **LEGO Bootloader** en MOCPilot.
5. Inicie **Recuperar firmware del hub** de nuevo.

Si vuelve a aparecer el mensaje de error de actualización, repita el procedimiento de recuperación desde el principio. Si el hub sigue sin poder recuperarse tras varios intentos, cambie o recargue las pilas e inténtelo de nuevo.
