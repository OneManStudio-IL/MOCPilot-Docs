---
id: Light
title: Licht
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Licht

Diese Seite dokumentiert die Blöcke der Kategorie Licht zum Steuern von LEDs und Lichtausgängen auf unterstützten Hubs.

## Allgemeine Lichtblöcke

### `LED-Farbe setzen` (Anfänger) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Setzt die LED-Farbe des Hubs über vordefinierte Farboptionen.

- Typ: Befehlsblock
- Typische Verwendung: Status anzeigen (bereit, läuft, Warnung, Fehler)

### `Licht einschalten auf` (Anfänger) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Setzt den gewählten Lichtausgang auf einen Zielwert bzw. eine Helligkeit.

- Typ: Befehlsblock
- Typische Verwendung: Scheinwerferhelligkeit, Statusintensität

### `Licht ausschalten` (Anfänger) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Schaltet den gewählten Lichtausgang aus.

- Typ: Befehlsblock
- Typische Verwendung: Abschaltsequenz, Energiesparen

### `Technic Move Licht einschalten auf` (Anfänger) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variante von `Licht einschalten auf` für Technic Move Hub/Lichtziel.

- Typ: Befehlsblock
- Typische Verwendung: Lichtausgang des Move-Hubs setzen

## Interne LED-Matrix-Blöcke

### `Lichtmatrix einschalten` (Fortgeschritten) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Zeigt das ausgewählte Bild auf der internen LED-Matrix des Hubs an und fährt sofort mit dem nächsten Block im Stapel fort. Das Bild bleibt auf dem Display, bis ein anderer Block die interne LED-Matrix ändert oder das Programm stoppt.

- Typ: Befehlsblock
- Hinweis: Der ausgewählte Hub muss eine interne LED-Matrix haben.

### `Auf Lichtmatrix schreiben` (Anfänger) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Zeigt eine Textzeichenfolge auf der internen LED-Matrix des Hubs an, indem die Buchstaben nacheinander gescrollt werden.

- Typ: Befehlsblock
- Hinweis: Der ausgewählte Hub muss eine interne LED-Matrix haben.

### `Matrix-Pixel ausschalten` (Anfänger) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Schaltet alle Lichter auf der internen LED-Matrix des Hubs aus.

- Typ: Befehlsblock
- Hinweis: Der ausgewählte Hub muss eine interne LED-Matrix haben.

### `Matrix-Pixel setzen` (Fortgeschritten) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Setzt die Helligkeit eines einzelnen Pixels auf der internen LED-Matrix des Hubs. Nur das ausgewählte Pixel wird aktualisiert; der Rest des Displays bleibt unverändert. Die Pixelposition verwendet Spalten- und Zeilenwerte, wobei Pixel `1, 1` in der linken oberen Ecke liegt.

- Typ: Befehlsblock
- Hinweis: Der ausgewählte Hub muss eine interne LED-Matrix haben.

### `Matrixausrichtung drehen` (Fortgeschritten) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Dreht die Ausrichtung dessen, was auf der internen LED-Matrix des Hubs angezeigt wird, im oder gegen den Uhrzeigersinn. Jede Drehung ändert die Displayausrichtung um 90 Grad und wirkt sich auf danach ausgeführte Lichtblöcke aus.

- Typ: Befehlsblock
- Hinweis: Der ausgewählte Hub muss eine interne LED-Matrix haben.

### `Matrixausrichtung setzen` (Fortgeschritten) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Setzt die Ausrichtung dessen, was auf der internen LED-Matrix des Hubs angezeigt wird. Die Standardausrichtung ist aufrecht, und die ausgewählte Ausrichtung wirkt sich auf danach ausgeführte Lichtblöcke aus.

- Typ: Befehlsblock
- Ausrichtungsoptionen: `aufrecht`, `links`, `rechts`, `kopfüber`
- Hinweis: Der ausgewählte Hub muss eine interne LED-Matrix haben.

## Lichtblöcke für Entfernungssensoren

### `Entfernungssensor aufleuchten lassen` (Anfänger) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Setzt die Lichter am ausgewählten Entfernungssensor. Der Block kann einzelne Sensorlichter ein- oder ausschalten und einen Listen-Reporterblock verwenden, um die Helligkeit jedes Lichts zu steuern.

- Typ: Befehlsblock
- Hinweis: Nur für den MINDSTORMS Robot Inventor Hub verfügbar.

## BuWizz 3 Lichtblöcke

### `BuWizz 3 LED-Farbe setzen` (Anfänger) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Setzt die LED-Farbe am gewählten BuWizz-3-Port mit integrierten Farboptionen.

- Typ: Befehlsblock

### `BuWizz 3 LED-Farbe setzen (String)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Setzt die BuWizz-3-LED-Farbe über einen Textwert.

- Typ: Befehlsblock
- Typische Verwendung: Dynamische Farbnamen aus Variablen

### `BuWizz 3 LED-Farbe setzen (RGB)` (Fortgeschritten) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Setzt die BuWizz-3-LED-Farbe über explizite RGB-Kanäle.

- Typ: Befehlsblock
- Typische Verwendung: Volle benutzerdefinierte Farbkonteolle und Verläufe
