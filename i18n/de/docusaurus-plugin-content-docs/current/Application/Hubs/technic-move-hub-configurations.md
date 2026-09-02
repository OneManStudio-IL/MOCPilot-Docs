---
id: TechnicMoveHubConfigurations
title: Technic Move Hub-Konfigurationen
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Technic Move Hub-Konfigurationen

## Überblick

Technic Move Hub führte eine einzigartige Funktion in der LEGO Powered Up Hub-Familie ein: Der Hub kann sein Verhalten abhängig von der aktuell angewendeten Konfiguration ändern.

MOCPilot ermöglicht es, die Konfiguration des Technic Move Hub zu ändern, damit das Hub-Verhalten zum offiziellen LEGO Set passt, das Sie steuern möchten.

## Unterstützte Konfigurationen

Derzeit sind diese Technic Move Hub-Konfigurationen bekannt:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Konfigurationsoptionen des Technic Move Hub" />

## Konfiguration über Meine Bluetooth-Hubs ändern

Sie können die Konfiguration auf der Seite **Meine Bluetooth-Hubs** ändern:

1. Öffnen Sie **Meine Bluetooth-Hubs**.
2. Suchen Sie den Technic Move Hub.
3. Öffnen Sie das Kontextmenü des Hubs.
4. Wählen Sie **Konfiguration auswählen**.
5. Wählen Sie die erforderliche Konfiguration.
6. Bestätigen Sie den Dialog zur Neukonfiguration.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Kontextmenü des Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Konfigurationsuntermenü des Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Bestätigungsdialog zur Neukonfiguration des Technic Move Hub" />

:::warning Wichtig
Beim Ändern der Hub-Konfiguration wird ein Unterprogramm auf den Hub geflasht; der Vorgang ähnelt einem Firmware-Update.

Lassen Sie den Hub während des gesamten Vorgangs eingeschaltet. Halten Sie Telefon, Tablet oder Computer eingeschaltet und in der Nähe des Hubs, damit die Bluetooth-Verbindung stabil bleibt. Schließen Sie MOCPilot nicht, deaktivieren Sie Bluetooth nicht und schalten Sie den Hub während der Konfigurationsänderung nicht aus.

Eine Unterbrechung der Konfigurationsänderung kann die Hub-Firmware beschädigen. In diesem Fall kann eine Firmware-Wiederherstellung erforderlich sein. Folgen Sie bei Bedarf der Anleitung zur [Hub-Firmware-Wiederherstellung](/docs/Application/Hubs/RecoveryHubFirmware/).
:::

Während der Neukonfiguration reagiert der Hub nicht auf normale Befehle. Die LED blinkt mit einer abgestuften farbigen Anzeige, bis der Vorgang abgeschlossen ist. Danach wird der Hub neu initialisiert.

## Konfigurationsblöcke

MOCPilot enthält außerdem Blöcke zum Lesen und Ändern der Technic Move Hub-Konfiguration während eines Programms.

### Hub-Konfiguration setzen

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Block Hub-Konfiguration setzen" />

Der Block **Hub-Konfiguration setzen** ändert den ausgewählten Hub auf eines seiner unterstützten Konfigurationsprofile.

- Hub-Auswahl: wählt den neu zu konfigurierenden Hub.
- Konfigurationsauswahl: wählt die Zielkonfiguration.
- Verfügbare Konfigurationen für Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** und **Batmobile™ Tumbler**.

Siehe die [Dokumentation des Blocks Hub-Konfiguration setzen](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Hub-Konfiguration

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Block Hub-Konfiguration" />

Der Block **Hub-Konfiguration** meldet die aktuelle Konfiguration des ausgewählten Hubs.

- Hub-Auswahl: wählt den Hub, der gelesen werden soll.
- Ausgabeformat: **Text** gibt den Namen der Konfiguration zurück.
- Ausgabeformat: **Index** gibt den Konfigurationsindex zurück, was für Vergleiche in Bedingungen nützlich ist.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Ausgabeformatoptionen des Blocks Hub-Konfiguration" />

Siehe die [Dokumentation des Blocks Hub-Konfiguration](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Stromimpuls

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Block Stromimpuls" />

Der Block **Stromimpuls** sendet einen Leistungsimpuls an den ausgewählten Technic Move Hub. Dieser Block funktioniert nur, wenn der Technic Move Hub als **Batmobile™ Tumbler** konfiguriert ist.

Beim Ausführen startet der Hub die Motoren für kurze Zeit mit maximal verfügbarer Leistung und Geschwindigkeit, normalerweise etwa 1-2 Sekunden.

Siehe die [Dokumentation des Blocks Stromimpuls](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Konfiguration während der Programmausführung ändern

Die Technic Move Hub-Konfiguration kann auch während der Programmausführung geändert werden.

Der übliche Ablauf ist:

1. Lesen Sie die aktuelle Hub-Konfiguration.
2. Vergleichen Sie sie mit der vom Profil benötigten Konfiguration.
3. Wenn die Konfiguration abweicht, setzen Sie die erforderliche Konfiguration.
4. Lesen Sie die Konfiguration nach der Neukonfiguration erneut.
5. Fahren Sie nur fort, wenn der Hub die erwartete Konfiguration meldet.
6. Trennen Sie die Verbindung oder stoppen Sie das Programm, wenn die erforderliche Konfiguration nicht angewendet wurde.

Das vorgefertigte Profil, das diesen Hub verwendet, kann als Referenz für diesen Ablauf dienen.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Blockbeispiel zur Konfigurationsänderung des Technic Move Hub während der Laufzeit" />
