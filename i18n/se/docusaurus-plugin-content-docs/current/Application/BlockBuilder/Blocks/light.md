---
id: Light
title: Ljus
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Ljus

Den här sidan dokumenterar block i kategorin Ljus som används för att styra LED:er och ljusutgångar på stödda hubbar.

## Vanliga ljusblock

### `Ställ in LED-färg` (Nybörjare) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Ställer in hubbens LED-färg med fördefinierade färgalternativ.

- Typ: kommandoblock
- Typisk användning: visa tillstånd (redo, kör, varning, fel)

### `Ställ ljus till` (Nybörjare) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Ställer in vald ljusutgång till ett målvärde för ljusstyrka/värde.

- Typ: kommandoblock
- Typisk användning: strålkastarens ljusstyrka, statusintensitet

### `Stäng av ljus` (Nybörjare) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Stänger av vald ljusutgång.

- Typ: kommandoblock
- Typisk användning: avstängningssekvens, batteribesparande beteende

### `Technic Move ställ ljus till` (Nybörjare) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variant av `Ställ ljus till` för Technic Move-hubb/ljusmål.

- Typ: kommandoblock
- Typisk användning: ställa in ljusutgångsnivån för Move-hubben

## Block för intern LED-matris

### `Tänd ljusmatris` (Avancerad) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Visar den valda bilden på hubbens interna LED-matris och fortsätter direkt till nästa block i blockföljden. Bilden stannar på displayen tills ett annat block ändrar den interna LED-matrisen eller programmet stoppas.

- Typ: kommandoblock
- Obs: den valda hubben måste ha en intern LED-matris.

### `Skriv på ljusmatris` (Nybörjare) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Visar en textsträng på hubbens interna LED-matris genom att rulla en bokstav i taget.

- Typ: kommandoblock
- Obs: den valda hubben måste ha en intern LED-matris.

### `Släck matrispixlar` (Nybörjare) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Släcker alla lampor på hubbens interna LED-matris.

- Typ: kommandoblock
- Obs: den valda hubben måste ha en intern LED-matris.

### `Ställ in matrispixel` (Avancerad) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Ställer in ljusstyrkan för en pixel på hubbens interna LED-matris. Endast den valda pixeln uppdateras; resten av displayen förblir oförändrad. Pixelpositionsfälten använder kolumn- och radvärden, med pixel `1, 1` i det övre vänstra hörnet.

- Typ: kommandoblock
- Obs: den valda hubben måste ha en intern LED-matris.

### `Rotera matrisorientering` (Avancerad) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Roterar orienteringen för det som visas på hubbens interna LED-matris medurs eller moturs. Varje rotation ändrar displayens orientering med 90 grader och påverkar ljusblock som körs efter den.

- Typ: kommandoblock
- Obs: den valda hubben måste ha en intern LED-matris.

### `Ställ in matrisorientering` (Avancerad) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Ställer in orienteringen för det som visas på hubbens interna LED-matris. Standardorienteringen är upprätt, och den valda orienteringen påverkar ljusblock som körs efter den.

- Typ: kommandoblock
- Orienteringsalternativ: `upprätt`, `vänster`, `höger`, `upp och ned`
- Obs: den valda hubben måste ha en intern LED-matris.

## Ljusblock för avståndssensor

### `Avståndssensor lys upp` (Nybörjare) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Ställer in lamporna på den valda avståndssensorn. Blocket kan tända eller släcka enskilda sensorlampor och kan använda ett listreporterblock för att styra ljusstyrkan för varje lampa.

- Typ: kommandoblock
- Obs: endast tillgängligt för MINDSTORMS Robot Inventor-hubben.

## BuWizz 3-ljusblock

### `BuWizz 3 ställ in LED-färg` (Nybörjare) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Ställer in LED-färg på vald BuWizz 3-port med inbyggda färgalternativ.

- Typ: kommandoblock

### `BuWizz 3 ställ in LED-färg (sträng)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Ställer in BuWizz 3-LED-färg med ett textbaserat färgvärde.

- Typ: kommandoblock
- Typisk användning: dynamiska färgnamn från variabler

### `BuWizz 3 ställ in LED-färg (RGB)` (Avancerad) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Ställer in BuWizz 3-LED-färg med explicita RGB-kanaler.

- Typ: kommandoblock
- Typisk användning: fullständig anpassad färgstyrning och gradienter
