---
id: Light
title: Licht
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Licht

Deze pagina beschrijft blokken uit de categorie Licht die worden gebruikt om LED’s en lichtuitgangen op ondersteunde hubs te bedienen.

## Algemene lichtblokken

### `Stel LED-kleur in` (Beginner) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Stelt de LED-kleur van de hub in met vooraf gedefinieerde kleuropties.

- Type: opdrachtblok
- Typisch gebruik: status weergeven (gereed, actief, waarschuwing, fout)

### `Licht instellen op` (Beginner) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Stelt de geselecteerde lichtuitgang in op een doelhelderheid/waarde.

- Type: opdrachtblok
- Typisch gebruik: koplamphelderheid, statusintensiteit

### `Licht uitschakelen` (Beginner) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Schakelt de geselecteerde lichtuitgang uit.

- Type: opdrachtblok
- Typisch gebruik: uitschakelprocedure, energiebesparend gedrag

### `Technic Move licht instellen op` (Beginner) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variant van `Licht instellen op` voor Technic Move hub/lichtdoel.

- Type: opdrachtblok
- Typisch gebruik: instellen van het lichtniveau van de Move hub

## Interne LED-matrixblokken

### `Lichtmatrix inschakelen` (Gevorderd) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Geeft de geselecteerde afbeelding weer op de interne LED-matrix van de hub en gaat direct verder met het volgende blok in de stapel. De afbeelding blijft op het display staan totdat een ander blok de interne LED-matrix wijzigt of het programma stopt.

- Type: opdrachtblok
- Opmerking: de geselecteerde hub moet een interne LED-matrix hebben.

### `Op lichtmatrix schrijven` (Beginner) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Geeft een tekststring weer op de interne LED-matrix van de hub door één letter tegelijk te scrollen.

- Type: opdrachtblok
- Opmerking: de geselecteerde hub moet een interne LED-matrix hebben.

### `Matrixpixels uitschakelen` (Beginner) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Schakelt alle lichten op de interne LED-matrix van de hub uit.

- Type: opdrachtblok
- Opmerking: de geselecteerde hub moet een interne LED-matrix hebben.

### `Matrixpixel instellen` (Gevorderd) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Stelt de helderheid van één pixel op de interne LED-matrix van de hub in. Alleen de geselecteerde pixel wordt bijgewerkt; de rest van het display blijft ongewijzigd. De pixelpositievakken gebruiken kolom- en rijwaarden, met pixel `1, 1` in de linkerbovenhoek.

- Type: opdrachtblok
- Opmerking: de geselecteerde hub moet een interne LED-matrix hebben.

### `Matrixrichting draaien` (Gevorderd) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Draait de richting van wat op de interne LED-matrix van de hub wordt weergegeven met de klok mee of tegen de klok in. Elke draaiing verandert de displayrichting met 90 graden en beïnvloedt de Licht-blokken die daarna worden uitgevoerd.

- Type: opdrachtblok
- Opmerking: de geselecteerde hub moet een interne LED-matrix hebben.

### `Matrixrichting instellen` (Gevorderd) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Stelt de richting in van wat op de interne LED-matrix van de hub wordt weergegeven. De standaardrichting is rechtop, en de geselecteerde richting beïnvloedt de Licht-blokken die daarna worden uitgevoerd.

- Type: opdrachtblok
- Orientatieopties: `rechtop`, `links`, `rechts`, `ondersteboven`
- Opmerking: de geselecteerde hub moet een interne LED-matrix hebben.

## Lichtblokken voor afstandssensor

### `Afstandssensor laten oplichten` (Beginner) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Stelt de lichten op de geselecteerde afstandssensor in. Het blok kan afzonderlijke sensorlichten in- of uitschakelen en kan een lijstrapportageblok gebruiken om de helderheid van elk licht te regelen.

- Type: opdrachtblok
- Opmerking: alleen beschikbaar voor de MINDSTORMS Robot Inventor hub.

## BuWizz 3 lichtblokken

### `BuWizz 3 stel LED-kleur in` (Beginner) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Stelt de LED-kleur in op de geselecteerde BuWizz 3-poort met ingebouwde kleuropties.

- Type: opdrachtblok

### `BuWizz 3 stel LED-kleur in (tekst)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Stelt de LED-kleur van BuWizz 3 in met een tekstwaarde.

- Type: opdrachtblok
- Typisch gebruik: dynamische kleurnamen vanuit variabelen

### `BuWizz 3 stel LED-kleur in (RGB)` (Gevorderd) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Stelt de LED-kleur van BuWizz 3 in met expliciete RGB-kanalen.

- Type: opdrachtblok
- Typisch gebruik: volledige aangepaste kleurcontrole en verlopen
