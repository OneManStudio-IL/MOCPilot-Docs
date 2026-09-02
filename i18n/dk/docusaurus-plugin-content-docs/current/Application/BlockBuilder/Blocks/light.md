---
id: Light
title: Lys
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Lys

Denne side dokumenterer blokke i kategorien Lys, som bruges til at styre LED'er og lysudgange på understøttede hubs.

## Almindelige lysblokke

### `Sæt LED-farve` (Begynder) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Sætter hubbens LED-farve ved hjælp af foruddefinerede farvevalg.

- Type: kommandoblok
- Typisk brug: vis status (klar, kører, advarsel, fejl)

### `Tænd lys til` (Begynder) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Sætter den valgte lysudgang til en mållysstyrke/-værdi.

- Type: kommandoblok
- Typisk brug: forlysstyrke, statusintensitet

### `Sluk lys` (Begynder) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Slukker den valgte lysudgang.

- Type: kommandoblok
- Typisk brug: nedlukningssekvens, batteribesparende adfærd

### `Technic Move tænd lys til` (Begynder) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variant af `Tænd lys til` for Technic Move hub/lysmål.

- Type: kommandoblok
- Typisk brug: indstil lysudgangsniveau for Move-hub

## Interne LED-matrixblokke

### `Tænd lysmatrix` (Avanceret) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Viser det valgte billede på hubbens interne LED-matrix og fortsætter straks til den næste blok i stakken. Billedet bliver på displayet, indtil en anden blok ændrer den interne LED-matrix, eller programmet stopper.

- Type: kommandoblok
- Bemærk: Den valgte hub skal have en intern LED-matrix.

### `Skriv på lysmatrix` (Begynder) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Viser en tekststreng på hubbens interne LED-matrix ved at rulle ét bogstav ad gangen.

- Type: kommandoblok
- Bemærk: Den valgte hub skal have en intern LED-matrix.

### `Sluk matrixpixels` (Begynder) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Slukker alle lys på hubbens interne LED-matrix.

- Type: kommandoblok
- Bemærk: Den valgte hub skal have en intern LED-matrix.

### `Indstil matrixpixel` (Avanceret) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Indstiller lysstyrken for én pixel på hubbens interne LED-matrix. Kun den valgte pixel opdateres; resten af displayet forbliver uændret. Pixelpositionsfelterne bruger kolonne- og rækkeværdier, hvor pixel `1, 1` er i øverste venstre hjørne.

- Type: kommandoblok
- Bemærk: Den valgte hub skal have en intern LED-matrix.

### `Roter matrixorientering` (Avanceret) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Roterer orienteringen af det, der vises på hubbens interne LED-matrix, med eller mod uret. Hver rotation ændrer displayorienteringen med 90 grader og påvirker de lysblokke, der køres efter den.

- Type: kommandoblok
- Bemærk: Den valgte hub skal have en intern LED-matrix.

### `Indstil matrixorientering` (Avanceret) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Indstiller orienteringen af det, der vises på hubbens interne LED-matrix. Standardorienteringen er opret, og den valgte orientering påvirker de lysblokke, der køres efter den.

- Type: kommandoblok
- Orienteringsmuligheder: `opret`, `venstre`, `højre`, `på hovedet`
- Bemærk: Den valgte hub skal have en intern LED-matrix.

## Lyseblokke til afstandssensor

### `Afstandssensor lys op` (Begynder) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Indstiller lysene på den valgte afstandssensor. Blokken kan tænde eller slukke individuelle sensorlys og kan bruge en listerapporterblok til at styre lysstyrken for hvert lys.

- Type: kommandoblok
- Bemærk: Kun tilgængelig for MINDSTORMS Robot Inventor-hubben.

## BuWizz 3-lysblokke

### `BuWizz 3 sæt LED-farve` (Begynder) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Sætter LED-farven på den valgte BuWizz 3-port med indbyggede farvevalg.

- Type: kommandoblok

### `BuWizz 3 sæt LED-farve (tekst)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Sætter BuWizz 3 LED-farven ved hjælp af en tekstbaseret farveværdi.

- Type: kommandoblok
- Typisk brug: dynamiske farvenavne fra variabler

### `BuWizz 3 sæt LED-farve (RGB)` (Avanceret) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Sætter BuWizz 3 LED-farven ved hjælp af eksplicitte RGB-kanaler.

- Type: kommandoblok
- Typisk brug: fuld brugerdefineret farvestyring og gradienter
