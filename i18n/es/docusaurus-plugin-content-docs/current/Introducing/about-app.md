---
id: AboutApp
title: Acerca de MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Constrúyelo. Condúcelo. Contrólalo todo.

**MOCPilot** — una app para crear perfiles de control personalizados para LEGO® y creaciones compatibles con Bluetooth.

Ofrece a los constructores un único lugar para conectar hubs, controlar motores, leer sensores, diseñar paneles y crear programas visuales para modelos, mecanismos, coches, camiones, trenes, robots y MOCs personalizados.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="Aplicación MOCPilot en un teléfono" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Qué te ofrece MOCPilot</h2>
    <ul>
      <li>Perfiles personalizados para tus propios modelos.</li>
      <li>Perfiles listos para sets oficiales compatibles.</li>
      <li>Conexión y gestión de hubs Bluetooth.</li>
      <li>Programación visual con bloques para automatización y lógica.</li>
      <li>Controles de panel para conducir y operar modelos.</li>
      <li>Compatibilidad con LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motores, sensores y dispositivos Bluetooth compatibles.</li>
    </ul>
  </div>
</div>

## La idea

La mayoría de las construcciones motorizadas necesitan más que un mando simple. Un coche puede necesitar dirección, acelerador, luces, monitorización de batería, una secuencia de caja de cambios o una rutina especial de arranque. Un robot puede necesitar sensores, eventos, lógica condicional y varios hubs trabajando juntos.

MOCPilot está diseñado para ese espacio intermedio entre un mando básico y un entorno de programación completo. Puedes empezar conduciendo un modelo desde un panel en pantalla y después añadir lógica, sensores y automatización cuando la construcción se vuelve más avanzada.

## Perfiles

Un **perfil** es el centro de control de un modelo.

Dentro de un perfil puedes elegir qué hubs pertenecen al modelo, crear el programa que ejecuta el modelo y diseñar el panel usado para controlarlo.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="Página de perfiles de MOCPilot" width="420" />

<details>
<summary>Perfiles predefinidos</summary>

Los perfiles predefinidos son ejemplos listos para sets oficiales compatibles. Son útiles cuando quieres empezar rápido o estudiar cómo se monta un perfil funcional.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Perfiles predefinidos de MOCPilot" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Programa de bloques predefinido de MOCPilot" width="1100" />

</details>

<details>
<summary>Perfiles personalizados</summary>

Los perfiles personalizados son para tus propios MOCs y experimentos. Puedes crear un perfil, añadir hubs, conectar motores y sensores, construir un programa y diseñar un panel de control que coincida con el modelo exacto.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Crear un perfil personalizado de MOCPilot" width="420" />

</details>

## Conectar hubs y dispositivos

MOCPilot puede conectarse a hubs Bluetooth compatibles y dispositivos compatibles, y luego ponerlos a disposición dentro de tu perfil.

Puedes usar un perfil con un solo hub para una construcción simple, o conectar varios hubs cuando tu modelo necesita más puertos, sistemas de alimentación separados o módulos independientes.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Página Mis hubs Bluetooth en MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Hubs Bluetooth conectados en MOCPilot" width="1100" />

<details>
<summary>Ejemplos de hardware compatible</summary>

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

Consulta la página de [hubs, motores y sensores compatibles](/docs/Introducing/SupportedDevices/) para ver la lista completa.

</details>

## Construir lógica con bloques

MOCPilot incluye un constructor visual de bloques. Puedes crear programas conectando bloques en lugar de escribir código.

Los bloques pueden reaccionar a eventos, controlar motores, leer sensores, trabajar con variables, usar entrada de gamepad, actualizar controladores del panel y coordinar varias acciones.

MOCPilot ofrece soporte completo para gamepads físicos conectados. Los bloques de gamepad permiten leer botones, gatillos, direcciones del D-pad y sticks, para mapear un mando real a tu modelo cuando el control físico es preferible a la pantalla táctil.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="Programa de usuario de MOCPilot creado con bloques" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Bloque al iniciar el programa" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Bloque iniciar motor a velocidad" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Bloque nivel de batería del hub" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Bloque valor del volante" />
</div>

<details>
<summary>Qué puedes hacer con programas de bloques</summary>

- Arrancar, detener y dirigir motores.
- Leer nivel de batería, voltaje, inclinación, orientación, temperatura y valores de sensores.
- Configurar controles de gamepad físico para dirección, acelerador, gatillos, acciones y cambio de modo.
- Reaccionar cuando cambian botones, sensores, temporizadores o controles del panel.
- Crear comprobaciones de arranque antes de que el modelo empiece a moverse.
- Añadir lógica personalizada para luces, calibración de dirección, modos de potencia y configuración del hub.
- Usar variables, listas, condiciones, bucles, mensajes y bloques personalizados para organizar comportamientos complejos.

</details>

## Diseñar un panel de conducción

El panel es la pantalla que usas mientras controlas el modelo. Puede incluir volantes, joysticks, deslizadores, botones, interruptores, pedales, monitores y otros controladores.

Puedes conectar controles del panel y entradas de gamepad físico a bloques y acciones del hub para que la interfaz coincida con el modelo.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="Controladores del panel de MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="Pantalla de control de MOCPilot con volante y pedales" width="1100" />

<details>
<summary>Ejemplos de panel</summary>

- Usa volante y pedales para coches.
- Usa deslizadores para grúas, elevadores y actuadores lineales.
- Usa botones para luces, bocina, cambios de marcha o acciones con script.
- Usa monitores para mostrar batería, velocidad, valores de sensores o estado personalizado del programa.
- Usa un gamepad conectado si prefieres botones, sticks y gatillos físicos en lugar de controles táctiles.

</details>

## Mantener manejables los modelos avanzados

A medida que crece un modelo, el perfil puede crecer con él. MOCPilot admite lógica reutilizable con **My Blocks**, configuración de hubs específica del perfil, varios controladores y flujos de programa que combinan control manual con automatización.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Ejemplo de uso de My Blocks en MOCPilot" width="1100" />

Esto ayuda a mantener legibles los programas grandes. Por ejemplo, un perfil puede tener un bloque personalizado para actualizar la batería, otro para calibrar la dirección y otro para un modo de conducción especial.

## Flujo típico

1. Crea o abre un perfil.
2. Añade los hubs Bluetooth y dispositivos usados por el modelo.
3. Construye el programa con bloques.
4. Diseña un panel para conducción e interacción.
5. Pulsa **Play**.
6. Prueba, ajusta y mejora el perfil hasta que el modelo se comporte como quieres.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Flujo de conexión de hub en MOCPilot" width="1100" />

## Para quién es MOCPilot

MOCPilot es útil para constructores que quieren:

- Un mando mejor para modelos LEGO® motorizados.
- Una forma de controlar hubs Bluetooth compatibles de terceros.
- Un entorno de programación visual para mecanismos y robots.
- Perfiles predefinidos para sets oficiales compatibles.
- Paneles personalizados para coches, camiones, trenes, crawlers, grúas y otros MOCs.
- Una sola app que combine hubs, motores, sensores, gamepads y controles en pantalla.

## Empezar a explorar

- Sigue el [tutorial de inicio rápido](/docs/Introducing/QuickStart/) para crear tu primer perfil.
- Consulta los [dispositivos compatibles](/docs/Introducing/SupportedDevices/) antes de elegir hardware.
- Explora la [documentación de BlockBuilder](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/) cuando estés listo para añadir lógica.
- Revisa la [actualización de firmware del hub](/docs/Application/Hubs/FirmwareUpdating/) si un hub requiere una versión de firmware compatible.
