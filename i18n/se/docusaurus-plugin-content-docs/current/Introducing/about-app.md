---
id: AboutApp
title: Om MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Bygg det. Kör det. Styr allt.

**MOCPilot** är en app för att skapa egna kontrollprofiler för LEGO® och kompatibla Bluetooth-drivna byggen.

Den ger byggare en plats för att ansluta hubbar, styra motorer, läsa sensorer, designa instrumentpaneler och skapa visuella program för modeller, mekanismer, bilar, lastbilar, tåg, robotar och egna MOC:er.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="MOCPilot-appen på en telefon" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Vad MOCPilot ger dig</h2>
    <ul>
      <li>Egna profiler för dina modeller.</li>
      <li>Färdiga profiler för officiella set som stöds.</li>
      <li>Anslutning och hantering av Bluetooth-hubbar.</li>
      <li>Visuell blockprogrammering för automatisering och logik.</li>
      <li>Instrumentpanelskontroller för att köra och använda modeller.</li>
      <li>Stöd för LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motorer, sensorer och kompatibla Bluetooth-enheter.</li>
    </ul>
  </div>
</div>

## Idén

De flesta motoriserade byggen behöver mer än en enkel fjärrkontroll. En bil kan behöva styrning, gas, ljus, batteriövervakning, växellådssekvens eller en särskild startrutin. En robot kan behöva sensorer, händelser, villkorslogik och flera hubbar som arbetar tillsammans.

MOCPilot är utformat för området mellan en enkel fjärrkontroll och en full programmeringsmiljö. Du kan börja med att köra en modell från en skärmpanel och sedan lägga till logik, sensorer och automatisering.

## Profiler

En **profil** är kontrollcentret för en modell.

I en profil kan du välja vilka hubbar som hör till modellen, skapa programmet som kör modellen och designa panelen som används för att styra den.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="MOCPilots profilsida" width="420" />

<details>
<summary>Förbyggda profiler</summary>

Förbyggda profiler är färdiga exempel för officiella set som stöds. De är användbara när du vill komma igång snabbt eller studera hur en fungerande profil är uppbyggd.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Förbyggda MOCPilot-profiler" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Förbyggt MOCPilot-blockprogram" width="1100" />

</details>

<details>
<summary>Egna profiler</summary>

Egna profiler är för dina MOC:er och experiment. Du kan skapa en profil, lägga till hubbar, ansluta motorer och sensorer, bygga ett program och designa en kontrollpanel som passar modellen.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Skapa en egen MOCPilot-profil" width="420" />

</details>

## Anslut hubbar och enheter

MOCPilot kan ansluta till Bluetooth-hubbar som stöds och kompatibla enheter och sedan göra dem tillgängliga i din profil.

Du kan använda en profil med en hubb för ett enkelt bygge eller ansluta flera hubbar när modellen behöver fler portar, separata strömsystem eller oberoende moduler.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Mina Bluetooth-hubbar-sidan i MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Anslutna Bluetooth-hubbar i MOCPilot" width="1100" />

<details>
<summary>Exempel på maskinvara som stöds</summary>

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

Se sidan [hubbar, motorer och sensorer som stöds](/docs/Introducing/SupportedDevices/) för hela listan.

</details>

## Bygg logik med block

MOCPilot innehåller en visuell blockbyggare. Du kan skapa program genom att koppla ihop block i stället för att skriva kod.

Block kan reagera på händelser, styra motorer, läsa sensorer, arbeta med variabler, använda gamepad-inmatning, uppdatera panelkontroller och samordna flera åtgärder.

MOCPilot har fullt stöd för anslutna fysiska gamepads. Gamepad-block kan läsa knappar, triggers, D-pad-riktningar och styrspakar, så att du kan mappa en riktig kontroll till modellen när fysisk styrning känns bättre än pekskärmen.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="MOCPilot-användarprogram byggt med block" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Block när programmet startar" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Block starta motor med hastighet" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Block för hubbens batterinivå" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Block för rattvärde" />
</div>

<details>
<summary>Vad du kan göra med blockprogram</summary>

- Starta, stoppa och styra motorer.
- Läsa batterinivå, spänning, lutning, orientering, temperatur och sensorvärden.
- Konfigurera fysisk gamepadstyrning för styrning, gas, triggers, åtgärder och lägesbyte.
- Reagera när knappar, sensorer, timers eller panelkontroller ändras.
- Skapa startkontroller innan modellen börjar röra sig.
- Lägga till egen logik för ljus, styrkalibrering, effektlägen och hubbkonfiguration.
- Använda variabler, listor, villkor, loopar, broadcasts och egna block för komplext beteende.

</details>

## Designa en körpanel

Instrumentpanelen är skärmen du använder när du styr modellen. Den kan innehålla rattar, joysticks, reglage, knappar, brytare, pedaler, monitorer och andra kontroller.

Du kan koppla panelkontroller och fysisk gamepad-inmatning till block och hubbåtgärder så att gränssnittet passar modellen.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="MOCPilot-panelkontroller" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="MOCPilot-kontrollskärm med ratt och pedaler" width="1100" />

<details>
<summary>Panelexempel</summary>

- Använd ratt och pedaler för bilar.
- Använd reglage för kranar, lyftar och linjära aktuatorer.
- Använd knappar för ljus, tuta, växling eller skriptade åtgärder.
- Använd monitorer för att visa batteri, hastighet, sensorvärden eller eget programtillstånd.
- Använd en ansluten gamepad om du föredrar fysiska knappar, spakar och triggers.

</details>

## Håll avancerade byggen hanterbara

När en modell växer kan profilen växa med den. MOCPilot stöder återanvändbar logik med **My Blocks**, profilspecifik hubbinställning, flera kontroller och programflöden som kombinerar manuell styrning med automatisering.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Exempel på användning av My Blocks i MOCPilot" width="1100" />

Det hjälper till att hålla stora program läsbara. En profil kan till exempel ha ett eget block för batteriuppdateringar, ett annat för styrkalibrering och ett tredje för ett särskilt körläge.

## Typiskt arbetsflöde

1. Skapa eller öppna en profil.
2. Lägg till Bluetooth-hubbar och enheter som modellen använder.
3. Bygg programmet med block.
4. Designa en panel för körning och interaktion.
5. Tryck på **Play**.
6. Testa, justera och förbättra profilen tills modellen beter sig som du vill.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Flöde för hubbanslutning i MOCPilot" width="1100" />

## Vem MOCPilot är till för

MOCPilot är användbart för byggare som vill ha:

- En bättre fjärrkontroll för motoriserade LEGO®-modeller.
- Ett sätt att styra kompatibla Bluetooth-hubbar från tredje part.
- En visuell programmeringsmiljö för mekanismer och robotar.
- Förbyggda profiler för officiella set som stöds.
- Egna paneler för bilar, lastbilar, tåg, crawlers, kranar och andra MOC:er.
- En enda app som kombinerar hubbar, motorer, sensorer, gamepads och skärmkontroller.

## Börja utforska

- Följ [snabbstartsguiden](/docs/Introducing/QuickStart/) för att bygga din första profil.
- Kontrollera [enheter som stöds](/docs/Introducing/SupportedDevices/) innan du väljer maskinvara.
- Utforska [BlockBuilder-dokumentationen](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/) när du är redo att lägga till logik.
- Läs om [uppdatering av hubb-firmware](/docs/Application/Hubs/FirmwareUpdating/) om en hubb kräver en stödd firmwareversion.
