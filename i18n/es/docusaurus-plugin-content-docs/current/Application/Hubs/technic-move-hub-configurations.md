---
id: TechnicMoveHubConfigurations
title: Configuraciones de Technic Move Hub
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Configuraciones de Technic Move Hub

## Descripción general

Technic Move Hub introdujo una función única en la familia de hubs LEGO Powered Up: el hub puede cambiar su comportamiento según la configuración aplicada actualmente.

MOCPilot permite cambiar la configuración de Technic Move Hub para que el comportamiento del hub coincida con el set oficial de LEGO que quieres controlar.

## Configuraciones compatibles

Actualmente se conocen estas configuraciones de Technic Move Hub:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Opciones de configuración de Technic Move Hub en el bloque Establecer configuración del hub" />

## Cambiar la configuración desde Mis hubs Bluetooth

Puedes cambiar la configuración desde la página **Mis hubs Bluetooth**:

1. Abre **Mis hubs Bluetooth**.
2. Busca el Technic Move Hub.
3. Abre el menú contextual del hub.
4. Selecciona **Seleccionar configuración**.
5. Elige la configuración necesaria.
6. Confirma el diálogo de reconfiguración.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Menú contextual de Technic Move Hub con la acción Seleccionar configuración" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Submenú de configuración de Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Diálogo de confirmación de reconfiguración de Technic Move Hub" />

:::warning Importante
Cambiar la configuración del hub graba un subprograma en el hub y es similar a una actualización de firmware.

Mantén el hub encendido durante todo el proceso. Mantén el teléfono, la tableta o el ordenador con batería y cerca del hub para que la conexión Bluetooth permanezca estable. No cierres MOCPilot, no apagues Bluetooth ni apagues el hub mientras se cambia la configuración.

Interrumpir el cambio de configuración puede dañar el firmware del hub. Si eso ocurre, puede ser necesaria la recuperación del firmware antes de volver a usarlo. Sigue la guía de [recuperación del firmware del hub](/docs/Application/Hubs/RecoveryHubFirmware/) si se requiere recuperación.
:::

Durante la reconfiguración, el hub no responde a comandos normales. Su LED parpadea con una indicación de colores por pasos hasta que termina el proceso. Después de aplicar la nueva configuración, el hub se reinicializa.

## Bloques de configuración

MOCPilot también incluye bloques para leer y cambiar la configuración de Technic Move Hub durante un programa.

### Establecer configuración del hub

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Bloque Establecer configuración del hub" />

El bloque **Establecer configuración del hub** cambia el hub seleccionado a uno de sus perfiles de configuración compatibles.

- Selector de hub: elige el hub que se va a reconfigurar.
- Selector de configuración: elige la configuración de destino.
- Configuraciones disponibles para Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** y **Batmobile™ Tumbler**.

Consulta la [documentación del bloque Establecer configuración del hub](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Configuración del hub

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Bloque informador Configuración del hub" />

El bloque **Configuración del hub** informa la configuración actual del hub seleccionado.

- Selector de hub: elige el hub que se va a leer.
- Formato de salida: **texto** devuelve el nombre de la configuración.
- Formato de salida: **índice** devuelve el índice de la configuración, útil para comparaciones en condiciones.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Opciones de formato de salida del bloque Configuración del hub" />

Consulta la [documentación del bloque Configuración del hub](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Pulso de potencia

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Bloque Pulso de potencia de Technic Move Hub" />

El bloque **Pulso de potencia** envía un comando de pulso de potencia al Technic Move Hub seleccionado. Este bloque solo funciona cuando el Technic Move Hub está configurado como **Batmobile™ Tumbler**.

Al ejecutarse, el hub pone en marcha los motores con la máxima potencia y velocidad disponibles durante poco tiempo, normalmente 1-2 segundos.

Consulta la [documentación del bloque Pulso de potencia](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Cambiar la configuración durante la ejecución del programa

También es posible cambiar la configuración de Technic Move Hub mientras se ejecuta un programa.

El enfoque habitual es:

1. Lee la configuración actual del hub.
2. Compárala con la configuración requerida por el perfil.
3. Si la configuración es diferente, aplica la configuración requerida.
4. Lee de nuevo la configuración después de la reconfiguración.
5. Continúa solo cuando el hub informe la configuración esperada.
6. Desconecta o detén el programa si no se aplicó la configuración requerida.

El perfil predefinido que usa este hub puede servir como referencia para este enfoque.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Ejemplo de bloques que muestra el cambio de configuración de Technic Move Hub durante la ejecución" />
