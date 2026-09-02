---
id: AboutApp
title: Über MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Bauen. Fahren. Alles steuern.

**MOCPilot** ist eine App zum Erstellen eigener Steuerungsprofile für LEGO® und kompatible Bluetooth-betriebene Modelle.

Sie bietet Baumeistern einen zentralen Ort, um Hubs zu verbinden, Motoren zu steuern, Sensoren auszulesen, Dashboards zu gestalten und visuelle Programme für Modelle, Mechanismen, Autos, Lkw, Züge, Roboter und eigene MOCs zu erstellen.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="MOCPilot app running on a phone" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Was MOCPilot bietet</h2>
    <ul>
      <li>Eigene Profile für Ihre Modelle.</li>
      <li>Fertige Profile für unterstützte offizielle Sets.</li>
      <li>Verbindung und Verwaltung von Bluetooth-Hubs.</li>
      <li>Visuelle Blockprogrammierung für Automatisierung und Logik.</li>
      <li>Dashboard-Steuerelemente zum Fahren und Bedienen von Modellen.</li>
      <li>Unterstützung für LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, Motoren, Sensoren und kompatible Bluetooth-Geräte.</li>
    </ul>
  </div>
</div>

## Die Idee

Die meisten motorisierten Modelle brauchen mehr als eine einfache Fernsteuerung. Ein Auto benötigt vielleicht Lenkung, Gas, Licht, Batterieüberwachung, eine Getriebesequenz oder eine spezielle Startroutine. Ein Roboter braucht möglicherweise Sensoren, Ereignisse, bedingte Logik und mehrere zusammenarbeitende Hubs.

MOCPilot ist für den Bereich zwischen einfacher Fernsteuerung und vollständiger Programmierumgebung gedacht. Sie können mit dem Fahren über ein Bildschirm-Dashboard beginnen und später Logik, Sensoren und Automatisierung hinzufügen.

## Profile

Ein **Profil** ist die Steuerzentrale für ein Modell.

In einem Profil wählen Sie die Hubs des Modells, erstellen das Programm, das das Modell ausführt, und gestalten das Dashboard zur Steuerung.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="MOCPilot profiles page" width="420" />

<details>
<summary>Vorgefertigte Profile</summary>

Vorgefertigte Profile sind einsatzbereite Beispiele für unterstützte offizielle Sets. Sie helfen beim schnellen Start oder beim Lernen, wie ein funktionierendes Profil aufgebaut ist.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="MOCPilot prebuilt profiles" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Prebuilt MOCPilot block program" width="1100" />

</details>

<details>
<summary>Eigene Profile</summary>

Eigene Profile sind für Ihre MOCs und Experimente gedacht. Sie können ein Profil erstellen, Hubs hinzufügen, Motoren und Sensoren verbinden, ein Programm bauen und ein passendes Steuer-Dashboard gestalten.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Create a custom MOCPilot profile" width="420" />

</details>

## Hubs und Geräte verbinden

MOCPilot kann unterstützte Bluetooth-Hubs und kompatible Geräte verbinden und sie in Ihrem Profil verfügbar machen.

Für ein einfaches Modell genügt ein Hub; für mehr Ports, getrennte Stromsysteme oder unabhängige Module können mehrere Hubs verbunden werden.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="My Bluetooth hubs page in MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Connected Bluetooth hubs in MOCPilot" width="1100" />

<details>
<summary>Beispiele unterstützter Hardware</summary>

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

Die vollständige Liste finden Sie auf der Seite [unterstützte Hubs, Motoren und Sensoren](/docs/Introducing/SupportedDevices/).

</details>

## Logik mit Blöcken bauen

MOCPilot enthält einen visuellen Block-Builder. Programme entstehen durch Verbinden von Blöcken statt durch Schreiben von Code.

Blöcke können auf Ereignisse reagieren, Motoren steuern, Sensoren lesen, mit Variablen arbeiten, Gamepad-Eingaben nutzen, Dashboard-Controller aktualisieren und mehrere Aktionen koordinieren.

MOCPilot unterstützt verbundene physische Gamepads vollständig. Gamepad-Blöcke lesen Tasten, Trigger, Steuerkreuz und Thumbsticks, sodass Sie einen echten Controller Ihrem Modell zuordnen können, wenn physische Bedienelemente besser passen als der Touchscreen.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="MOCPilot user program built with blocks" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="When program starts block" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Start motor at speed block" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Hub battery level block" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Steering wheel value block" />
</div>

<details>
<summary>Was Blockprogramme können</summary>

- Motoren starten, stoppen und lenken.
- Batteriestand, Spannung, Neigung, Ausrichtung, Temperatur und Sensorwerte lesen.
- Physische Gamepad-Steuerung für Lenkung, Gas, Trigger, Aktionen und Moduswechsel konfigurieren.
- Auf Änderungen von Tasten, Sensoren, Timern oder Dashboard-Controllern reagieren.
- Startprüfungen erstellen, bevor das Modell losfährt.
- Eigene Logik für Licht, Lenkkalibrierung, Leistungsmodi und Hub-Konfiguration hinzufügen.
- Variablen, Listen, Bedingungen, Schleifen, Broadcasts und eigene Blöcke verwenden, um komplexes Verhalten zu organisieren.

</details>

## Ein Fahr-Dashboard gestalten

Das Dashboard ist der Bildschirm, den Sie beim Steuern des Modells verwenden. Es kann Lenkräder, Joysticks, Slider, Tasten, Schalter, Pedale, Monitore und andere Controller enthalten.

Dashboard-Controller und physische Gamepad-Eingaben können mit Blöcken und Hub-Aktionen verbunden werden, damit die Oberfläche zum Modell passt.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="MOCPilot dashboard controllers" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="MOCPilot control screen with steering and pedals" width="1100" />

<details>
<summary>Dashboard-Beispiele</summary>

- Lenkrad und Pedale für Autos verwenden.
- Slider für Kräne, Hebevorrichtungen und Linearantriebe verwenden.
- Tasten für Licht, Hupe, Gangwechsel oder geskriptete Aktionen verwenden.
- Monitore für Batterie, Geschwindigkeit, Sensorwerte oder eigenen Programmstatus verwenden.
- Ein verbundenes Gamepad verwenden, wenn Sie physische Tasten, Sticks und Trigger bevorzugen.

</details>

## Fortgeschrittene Modelle übersichtlich halten

Wenn ein Modell wächst, kann das Profil mitwachsen. MOCPilot unterstützt wiederverwendbare Logik mit **My Blocks**, profilspezifische Hub-Einstellungen, mehrere Controller und Programmabläufe, die manuelle Steuerung mit Automatisierung kombinieren.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="MOCPilot My Blocks usage example" width="1100" />

So bleiben große Programme lesbar. Ein Profil kann zum Beispiel einen eigenen Block für Batterieupdates, einen für Lenkkalibrierung und einen für einen speziellen Fahrmodus enthalten.

## Typischer Ablauf

1. Profil erstellen oder öffnen.
2. Bluetooth-Hubs und Geräte des Modells hinzufügen.
3. Programm mit Blöcken bauen.
4. Dashboard zum Fahren und Interagieren gestalten.
5. **Play** drücken.
6. Profil testen, abstimmen und verbessern, bis das Modell wie gewünscht reagiert.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Connect hub flow in MOCPilot" width="1100" />

## Für wen MOCPilot gedacht ist

MOCPilot ist hilfreich für Baumeister, die Folgendes möchten:

- Eine bessere Fernsteuerung für motorisierte LEGO® Modelle.
- Kompatible Bluetooth-Hubs von Drittanbietern steuern.
- Eine visuelle Programmierumgebung für Mechanismen und Roboter.
- Vorgefertigte Profile für unterstützte offizielle Sets.
- Eigene Dashboards für Autos, Lkw, Züge, Crawler, Kräne und andere MOCs.
- Eine einzige App, die Hubs, Motoren, Sensoren, Gamepads und Bildschirmsteuerungen kombiniert.

## Loslegen

- Folgen Sie dem [Schnellstart-Tutorial](/docs/Introducing/QuickStart/), um Ihr erstes Profil zu erstellen.
- Prüfen Sie [unterstützte Geräte](/docs/Introducing/SupportedDevices/), bevor Sie Hardware auswählen.
- Öffnen Sie die [BlockBuilder-Dokumentation](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/), wenn Sie Logik hinzufügen möchten.
- Lesen Sie [Hub-Firmware aktualisieren](/docs/Application/Hubs/FirmwareUpdating/), wenn ein Hub eine unterstützte Firmware-Version benötigt.
