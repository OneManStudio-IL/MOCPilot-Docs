---
id: Light
title: Lys
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Lys

Denne siden dokumenterer blokker i Lys-kategorien som brukes til å kontrollere LED-er og lysutganger på støttede huber.

## Vanlige lysblokker

### `Sett LED-farge` (Nybegynner) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Setter hubens LED-farge ved hjelp av forhåndsdefinerte fargevalg.

- Type: kommandoblokk
- Typisk bruk: vise tilstand (klar, kjører, advarsel, feil)

### `Sett lys til` (Nybegynner) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Setter valgt lysutgang til en målverdi/lysstyrke.

- Type: kommandoblokk
- Typisk bruk: frontlys, statusintensitet

### `Slå av lys` (Nybegynner) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Slår av valgt lysutgang.

- Type: kommandoblokk
- Typisk bruk: avslutningssekvens, batterisparing

### `Technic Move sett lys til` (Nybegynner) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variant av `Sett lys til` for Technic Move hub/lys.

- Type: kommandoblokk
- Typisk bruk: sette lysnivå på Move-hub

## Interne LED-matriseblokker

### `Slå på lysmatrise` (Avansert) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Viser det valgte bildet på hubens interne LED-matrise og går umiddelbart videre til neste blokk i stabelen. Bildet blir stående på displayet til en annen blokk endrer den interne LED-matrisen eller programmet stopper.

- Type: kommandoblokk
- Merk: den valgte huben må ha en intern LED-matrise.

### `Skriv på lysmatrise` (Nybegynner) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Viser en tekststreng på hubens interne LED-matrise ved å rulle én bokstav om gangen.

- Type: kommandoblokk
- Merk: den valgte huben må ha en intern LED-matrise.

### `Slå av matrisepiksler` (Nybegynner) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Slår av alle lysene på hubens interne LED-matrise.

- Type: kommandoblokk
- Merk: den valgte huben må ha en intern LED-matrise.

### `Sett matrisepiksel` (Avansert) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Setter lysstyrken for én piksel på hubens interne LED-matrise. Bare den valgte pikselen oppdateres; resten av displayet forblir uendret. Pikselposisjonsfeltene bruker kolonne- og radverdier, med piksel `1, 1` øverst til venstre.

- Type: kommandoblokk
- Merk: den valgte huben må ha en intern LED-matrise.

### `Roter matriseretning` (Avansert) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Roterer retningen på det som vises på hubens interne LED-matrise med eller mot klokken. Hver rotasjon endrer displayretningen med 90 grader og påvirker lysblokker som kjøres etter den.

- Type: kommandoblokk
- Merk: den valgte huben må ha en intern LED-matrise.

### `Sett matriseretning` (Avansert) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Setter retningen på det som vises på hubens interne LED-matrise. Standardretningen er oppreist, og den valgte retningen påvirker lysblokker som kjøres etter den.

- Type: kommandoblokk
- Orienteringsvalg: `oppreist`, `venstre`, `høyre`, `opp ned`
- Merk: den valgte huben må ha en intern LED-matrise.

## Lysblokker for avstandssensor

### `Avstandssensor lys opp` (Nybegynner) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Setter lysene på den valgte avstandssensoren. Blokken kan slå individuelle sensorlys på eller av, og kan bruke en listerapportørblokk til å styre lysstyrken for hvert lys.

- Type: kommandoblokk
- Merk: kun tilgjengelig for MINDSTORMS Robot Inventor-huben.

## BuWizz 3 lysblokker

### `BuWizz 3 sett LED-farge` (Nybegynner) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Setter LED-farge på valgt BuWizz 3-port med innebygde fargevalg.

- Type: kommandoblokk

### `BuWizz 3 sett LED-farge (tekst)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Setter BuWizz 3 LED-farge ved bruk av tekstverdi.

- Type: kommandoblokk
- Typisk bruk: dynamiske fargenavn fra variabler

### `BuWizz 3 sett LED-farge (RGB)` (Avansert) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Setter BuWizz 3 LED-farge ved bruk av eksplisitte RGB-kanaler.

- Type: kommandoblokk
- Typisk bruk: full tilpasset fargekontroll og gradienter
