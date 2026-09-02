---
id: FirmwareUpdating
title: Actualización de firmware
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Actualización de firmware

MOCPilot puede actualizar el firmware de los hubs LEGO Powered Up compatibles cuando hay una versión compatible más reciente disponible.

Las actualizaciones de firmware pueden ser necesarias para que un hub funcione correctamente con MOCPilot. Un firmware más reciente puede mejorar la compatibilidad, corregir el comportamiento del hub y permitir que la app use las funciones esperadas para ese modelo.

## Hubs compatibles

La actualización de firmware está disponible actualmente para estos hubs:

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

## Antes de empezar

Antes de iniciar la actualización, asegúrese de que el hub y el dispositivo que ejecuta MOCPilot tengan suficiente batería.

Mantenga el hub encendido durante todo el proceso. Mantenga el teléfono, la tablet o el ordenador cerca del hub para que la conexión Bluetooth permanezca estable. No cierre MOCPilot, no desactive Bluetooth ni apague el hub mientras se carga el firmware.

:::warning Importante
Interrumpir una actualización de firmware puede dejar el firmware del hub en un estado incompleto. Si ocurre, el hub puede necesitar recuperación de firmware antes de volver a usarse.
:::

## Iniciar la actualización

Al conectar un hub, MOCPilot comprueba la versión de firmware instalada. Si la app detecta que se necesita una versión más reciente, muestra un diálogo de actualización de firmware.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_1.png')} alt="Actualización de firmware" />

Seleccione **Actualizar** para iniciar la actualización de firmware inmediatamente.

Si no desea actualizar ahora, seleccione **Cancelar**. Puede iniciar la actualización más tarde desde el menú contextual del hub.

## Actualizar más tarde desde el menú del hub

Para iniciar la actualización de firmware manualmente:

1. Abra **Mis hubs Bluetooth**.
2. Busque el hub que necesita actualizarse.
3. Abra el menú contextual del hub.
4. Seleccione **Actualizar firmware**.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_2.png')} alt="Actualizar firmware" />

## Durante la actualización de firmware

Tras iniciar la actualización, MOCPilot carga el firmware en el hub y muestra el progreso.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_3.png')} alt="Actualización de firmware" />

Espere hasta que la carga termine. El hub puede reiniciarse o desconectarse temporalmente mientras se aplica el nuevo firmware.

Después de cargar el firmware, MOCPilot vuelve a buscar el hub. Mantenga el hub cerca y espere a que la app se reconecte.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_4.png')} alt="Actualización de firmware" />

## Finalizar la actualización

Cuando la actualización termina correctamente, MOCPilot muestra un diálogo de confirmación.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_5.png')} alt="Actualización de firmware" />

Seleccione **OK**. El hub se reconectará y la tarjeta del hub mostrará la versión de firmware actualizada.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_6.png')} alt="Actualización de firmware" />

Ahora puede seguir usando el hub con MOCPilot.

## Si la actualización falla

Si la actualización no termina correctamente, MOCPilot muestra un mensaje de error de actualización de firmware.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_7.png')} alt="Actualización de firmware" />

Primero, apague y encienda el hub y ejecute la actualización de nuevo:

1. Apague el hub.
2. Encienda el hub de nuevo.
3. Mantenga el hub cerca de su dispositivo.
4. Conecte el hub en MOCPilot.
5. Inicie de nuevo la actualización de firmware.

Si el hub no responde normalmente, puede ser necesaria la recuperación de firmware. Siga la guía [Recuperación del firmware del hub](/docs/Application/Hubs/RecoveryHubFirmware/) para obtener instrucciones detalladas.
