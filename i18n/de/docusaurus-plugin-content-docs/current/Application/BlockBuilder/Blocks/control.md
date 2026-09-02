---
id: Control
title: Steuerung
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Steuerung

Steuerungsblöcke verwalten den Ausführungsfluss: Warten, Schleifen, Verzweigung und Stoppen von Skripten.

## Warteblöcke

### `Warte` (Anfänger) {#block_control_wait_for}
<img src={useBaseUrl('/img/blocks/block_control_wait_for.svg')} alt="block_control_wait_for.svg" />
Pausiert das aktuelle Skript für eine angegebene Zeit.

### `Warte bis` (Fortgeschritten) {#block_control_wait_until}
<img src={useBaseUrl('/img/blocks/block_control_wait_until.svg')} alt="block_control_wait_until.svg" />
Pausiert das aktuelle Skript, bis eine Bedingung wahr wird.

## Schleifenblöcke

### `Wiederhole` (Fortgeschritten) {#block_control_repeat_for}
<img src={useBaseUrl('/img/blocks/block_control_repeat_for.svg')} alt="block_control_repeat_for.svg" />
Führt verschachtelte Blöcke eine feste Anzahl von Malen aus.

### `Wiederhole bis` (Fortgeschritten) {#block_control_repeat_until}
<img src={useBaseUrl('/img/blocks/block_control_repeat_until.svg')} alt="block_control_repeat_until.svg" />
Wiederholt verschachtelte Blöcke, bis eine Bedingung wahr ist.

### `Fortlaufend` (Fortgeschritten) {#block_control_repeat_forever}
<img src={useBaseUrl('/img/blocks/block_control_repeat_forever.svg')} alt="block_control_repeat_forever.svg" />
Führt verschachtelte Blöcke dauerhaft aus, bis Programm oder Skript gestoppt wird.

## Verzweigungsblöcke

### `Wenn` (Anfänger) {#block_control_if}
<img src={useBaseUrl('/img/blocks/block_control_if.svg')} alt="block_control_if.svg" />
Führt verschachtelte Blöcke nur bei wahrer Bedingung aus.

### `Wenn / Sonst` (Fortgeschritten) {#block_control_if_else}
<img src={useBaseUrl('/img/blocks/block_control_if_else.svg')} alt="block_control_if_else.svg" />
Führt einen Zweig aus, wenn die Bedingung wahr ist, sonst den alternativen Zweig.

### `Tu dies und dies` (Guru) {#block_control_do_this_and_this}
<img src={useBaseUrl('/img/blocks/block_control_do_this_and_this.svg')} alt="block_control_do_this_and_this.svg" />
Führt zwei Blockstapel nacheinander in einer Steuerungsoperation aus.

## Stoppblöcke

### `Stop` (Anfänger) {#block_control_stop}
<img src={useBaseUrl('/img/blocks/block_control_stop.svg')} alt="block_control_stop.svg" />
Stoppt die Skriptausführung (Bereich abhängig von der gewählten Stopp-Option).

- Stopp-Optionen: `alles`, `dieser Stapel`, `und Programm beenden`

### `Andere Stapel stoppen` (Guru) {#block_control_stop_other_stacks}
<img src={useBaseUrl('/img/blocks/block_control_stop_other_stacks.svg')} alt="block_control_stop_other_stacks.svg" />
Stoppt alle anderen laufenden Stapel, während der aktuelle Stapel weiterläuft.

## Hub-/Steuerungs-Utility-Blöcke

### `Verbindung setzen` (Anfänger) {#block_hubs_control_set_connect}
<img src={useBaseUrl('/img/blocks/block_hubs_control_set_connect.svg')} alt="block_hubs_control_set_connect.svg" />
Steuert den Verbindungsstatus des Hubs aus der Skriptlogik.

- Aktionsoptionen: `verbinden`, `trennen`

### `Hub-Konfiguration setzen` (Fortgeschritten) {#block_hubs_set_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="block_hubs_set_hub_config.svg" />
Setzt den ausgewählten Hub auf eines seiner unterstützten Konfigurationsprofile.

- Nur verfügbar für Hubs, die Hub-Konfigurationsoptionen bereitstellen.
- Typische Verwendung: einen konfigurierbaren Hub, zum Beispiel Technic Move Hub, vor den nächsten Blöcken auf eine andere gespeicherte Konfiguration umschalten.

### `Hub-Konfiguration` (Fortgeschritten) {#block_hubs_all_control_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="block_hubs_all_control_hub_config.svg" />
Gibt die aktuelle Konfiguration des ausgewählten Hubs zurück.

- Typ: Reporterblock
- Ausgabeformatoptionen: `text`, `index`
- Nur verfügbar für Hubs, die Hub-Konfigurationsoptionen bereitstellen.
- Gibt `NaN` zurück, wenn der ausgewählte Hub nicht verbunden ist oder keine Konfiguration verfügbar ist.

### `Ist verbunden` (Anfänger) {#block_hubs_all_sensors_is_connected}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_connected.svg')} alt="block_hubs_all_sensors_is_connected.svg" />
Gibt zurück, ob der Hub aktuell verbunden ist.

- Typ: boolescher Reporterblock

### `BuWizz 2 Leistungsmodus setzen` (Anfänger) {#block_hubs_buwizz_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_set_power_mode.svg')} alt="block_hubs_buwizz_sensors_set_power_mode.svg" />
Setzt den Leistungsmodus des BuWizz-2-Hubs.

- Modusoptionen: `Slow`, `Normal`, `Fast`, `Ludicrous`

### `BuWizz 2 Leistungsmodus abfragen` (Guru) {#block_hubs_buwizz_sensors_get_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_power_mode.svg')} alt="block_hubs_buwizz_sensors_get_power_mode.svg" />
Gibt den aktuell aktiven Leistungsmodus von BuWizz 2 zurück.

- Ausgabeoptionen: `text`, `index`

### `MouldKing Steuerkanal setzen` (Fortgeschritten) {#block_hubs_mouldking_control_set_control_channel}
<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_set_control_channel.svg')} alt="block_hubs_mouldking_control_set_control_channel.svg" />
Setzt den aktiven Steuerkanal für unterstützte MouldKing-Hubs/Controller.

- Kanaloptionen: `A`, `B`, `C`

### `MouldKing Steuerkanal abfragen` (Fortgeschritten) {#block_hubs_mouldking_control_get_control_channel}
<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_get_control_channel.svg')} alt="block_hubs_mouldking_control_get_control_channel.svg" />
Gibt den aktuell aktiven Steuerkanal für unterstützte MouldKing-Hubs/Controller zurück.

- Ausgabeoptionen: `text`, `index`