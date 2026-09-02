---
id: AboutApp
title: Over MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Bouw het. Bestuur het. Bedien alles.

**MOCPilot** — een app voor het maken van aangepaste besturingsprofielen voor LEGO® en compatibele Bluetooth-aangedreven creaties.

Het geeft bouwers één plek om hubs te verbinden, motoren te bedienen, sensoren uit te lezen, dashboards te ontwerpen en visuele programma’s te maken voor modellen, mechanismen, auto’s, vrachtwagens, treinen, robots en eigen MOC’s.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="MOCPilot-app op een telefoon" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Wat MOCPilot je geeft</h2>
    <ul>
      <li>Aangepaste profielen voor je eigen modellen.</li>
      <li>Kant-en-klare profielen voor ondersteunde officiële sets.</li>
      <li>Bluetooth-hubs verbinden en beheren.</li>
      <li>Visueel programmeren met blokken voor automatisering en logica.</li>
      <li>Dashboardbediening om modellen te rijden en te bedienen.</li>
      <li>Ondersteuning voor LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motoren, sensoren en compatibele Bluetooth-apparaten.</li>
    </ul>
  </div>
</div>

## Het idee

De meeste gemotoriseerde builds hebben meer nodig dan een eenvoudige afstandsbediening. Een auto kan besturing, gas, verlichting, batterijbewaking, een versnellingsbakreeks of een speciale startroutine nodig hebben. Een robot kan sensoren, gebeurtenissen, voorwaardelijke logica en meerdere samenwerkende hubs nodig hebben.

MOCPilot is ontworpen voor de ruimte tussen een eenvoudige afstandsbediening en een volledige programmeeromgeving. Je kunt beginnen door een model vanaf een schermdashboard te besturen en later logica, sensoren en automatisering toevoegen.

## Profielen

Een **profiel** is het controlecentrum voor één model.

Binnen een profiel kies je welke hubs bij het model horen, maak je het programma dat het model uitvoert en ontwerp je het dashboard waarmee je het bestuurt.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="Profielenpagina van MOCPilot" width="420" />

<details>
<summary>Vooraf gebouwde profielen</summary>

Vooraf gebouwde profielen zijn kant-en-klare voorbeelden voor ondersteunde officiële sets. Ze zijn handig om snel te starten of te bekijken hoe een werkend profiel is opgebouwd.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Vooraf gebouwde MOCPilot-profielen" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Vooraf gebouwd MOCPilot-blokprogramma" width="1100" />

</details>

<details>
<summary>Aangepaste profielen</summary>

Aangepaste profielen zijn voor je eigen MOC’s en experimenten. Je kunt een profiel maken, hubs toevoegen, motoren en sensoren verbinden, een programma bouwen en een dashboard ontwerpen dat precies bij het model past.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Een aangepast MOCPilot-profiel maken" width="420" />

</details>

## Hubs en apparaten verbinden

MOCPilot kan verbinding maken met ondersteunde Bluetooth-hubs en compatibele apparaten en ze daarna beschikbaar maken in je profiel.

Je kunt één hub gebruiken voor een eenvoudige build of meerdere hubs verbinden wanneer je model meer poorten, aparte voedingssystemen of onafhankelijke modules nodig heeft.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Mijn Bluetooth-hubs-pagina in MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Verbonden Bluetooth-hubs in MOCPilot" width="1100" />

<details>
<summary>Voorbeelden van ondersteunde hardware</summary>

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

Bekijk de pagina [ondersteunde hubs, motoren en sensoren](/docs/Introducing/SupportedDevices/) voor de volledige lijst.

</details>

## Logica bouwen met blokken

MOCPilot bevat een visuele block builder. Je kunt programma’s maken door blokken te verbinden in plaats van code te schrijven.

Blokken kunnen reageren op gebeurtenissen, motoren bedienen, sensoren uitlezen, met variabelen werken, gamepadinvoer gebruiken, dashboardcontrollers bijwerken en meerdere acties coördineren.

MOCPilot ondersteunt aangesloten fysieke gamepads volledig. Gamepadblokken lezen knoppen, triggers, D-pad-richtingen en thumbsticks, zodat je een echte controller aan je model kunt koppelen wanneer fysieke bediening beter voelt dan het touchscreen.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="MOCPilot-gebruikersprogramma gebouwd met blokken" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Blok wanneer programma start" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Blok motor starten op snelheid" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Blok batterijniveau van hub" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Blok stuurwielwaarde" />
</div>

<details>
<summary>Wat je met blokprogramma’s kunt doen</summary>

- Motoren starten, stoppen en sturen.
- Batterijniveau, spanning, kanteling, oriëntatie, temperatuur en sensorwaarden uitlezen.
- Fysieke gamepadbediening configureren voor sturen, gas, triggers, acties en moduswissels.
- Reageren wanneer knoppen, sensoren, timers of dashboardcontrollers veranderen.
- Startcontroles maken voordat het model begint te bewegen.
- Aangepaste logica toevoegen voor verlichting, stuurkalibratie, vermogensmodi en hubconfiguratie.
- Variabelen, lijsten, voorwaarden, lussen, broadcasts en aangepaste blokken gebruiken om complex gedrag te organiseren.

</details>

## Een rijdashboard ontwerpen

Het dashboard is het scherm dat je gebruikt terwijl je het model bestuurt. Het kan stuurwielen, joysticks, sliders, knoppen, schakelaars, pedalen, monitors en andere controllers bevatten.

Je kunt dashboardbediening en fysieke gamepadinvoer verbinden met blokken en hubacties, zodat de interface bij het model past.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="MOCPilot-dashboardcontrollers" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="MOCPilot-bedieningsscherm met stuur en pedalen" width="1100" />

<details>
<summary>Dashboardvoorbeelden</summary>

- Gebruik een stuurwiel en pedalen voor auto’s.
- Gebruik sliders voor kranen, liften en lineaire actuatoren.
- Gebruik knoppen voor verlichting, claxons, schakelen of gescripte acties.
- Gebruik monitors om batterij, snelheid, sensorwaarden of aangepaste programmastatus te tonen.
- Gebruik een aangesloten gamepad als je fysieke knoppen, sticks en triggers prettiger vindt dan touchscreenbediening.

</details>

## Geavanceerde builds beheersbaar houden

Naarmate een model groeit, kan het profiel meegroeien. MOCPilot ondersteunt herbruikbare logica met **My Blocks**, profielspecifieke hubinstellingen, meerdere controllers en programmaflows die handmatige bediening combineren met automatisering.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Voorbeeld van My Blocks-gebruik in MOCPilot" width="1100" />

Zo blijven grote programma’s leesbaar. Een profiel kan bijvoorbeeld één aangepast blok hebben voor batterij-updates, een ander voor stuurkalibratie en nog een voor een speciale rijmodus.

## Typische workflow

1. Maak of open een profiel.
2. Voeg de Bluetooth-hubs en apparaten toe die het model gebruikt.
3. Bouw het programma met blokken.
4. Ontwerp een dashboard voor rijden en interactie.
5. Druk op **Play**.
6. Test, stem af en verbeter het profiel totdat het model doet wat je wilt.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Hubverbindingsflow in MOCPilot" width="1100" />

## Voor wie MOCPilot is

MOCPilot is nuttig voor bouwers die willen:

- Een betere afstandsbediening voor gemotoriseerde LEGO®-modellen.
- Compatibele Bluetooth-hubs van derden bedienen.
- Een visuele programmeeromgeving voor mechanismen en robots.
- Vooraf gebouwde profielen voor ondersteunde officiële sets.
- Aangepaste dashboards voor auto’s, vrachtwagens, treinen, crawlers, kranen en andere MOC’s.
- Eén app die hubs, motoren, sensoren, gamepads en schermbediening combineert.

## Begin met verkennen

- Volg de [snelstarttutorial](/docs/Introducing/QuickStart/) om je eerste profiel te bouwen.
- Controleer [ondersteunde apparaten](/docs/Introducing/SupportedDevices/) voordat je hardware kiest.
- Verken de [BlockBuilder-documentatie](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/) wanneer je logica wilt toevoegen.
- Bekijk [hubfirmware bijwerken](/docs/Application/Hubs/FirmwareUpdating/) als een hub een ondersteunde firmwareversie vereist.
