---
id: Light
title: Světla
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Světla

Tato stránka popisuje bloky kategorie Světla, které slouží k ovládání LED a světelných výstupů na podporovaných hubech.

## Běžné bloky světel

### `Nastavit barvu LED na` (Začátečník) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Nastaví barvu LED na hubu pomocí předdefinovaných barev.

- Typ: příkazový blok
- Typické použití: zobrazení stavu (připraveno, běží, varování, chyba)

### `Nastavit světlo na` (Začátečník) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Nastaví vybraný světelný výstup na cílový jas/hodnotu.

- Typ: příkazový blok
- Typické použití: jas předního světla, intenzita stavové signalizace

### `Vypnout světlo` (Začátečník) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Vypne vybraný světelný výstup.

- Typ: příkazový blok
- Typické použití: vypínací sekvence, úspora baterie

### `Technic Move nastavit světlo na` (Začátečník) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Varianta bloku `Nastavit světlo na` pro cíle hubu/světla Technic Move.

- Typ: příkazový blok
- Typické použití: nastavení úrovně světelného výstupu hubu Move

## Bloky interní LED matice

### `Zapnout světelnou matici` (Pokročilý) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Zobrazí vybraný obrázek na interní LED matici hubu a okamžitě pokračuje dalším blokem v zásobníku. Obrázek zůstane na displeji, dokud jiný blok nezmění interní LED matici nebo dokud se program nezastaví.

- Typ: příkazový blok
- Poznámka: vybraný hub musí mít interní LED matici.

### `Psát na světelnou matici` (Začátečník) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Zobrazí textový řetězec na interní LED matici hubu posouváním jednotlivých písmen.

- Typ: příkazový blok
- Poznámka: vybraný hub musí mít interní LED matici.

### `Vypnout pixely matice` (Začátečník) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Vypne všechna světla na interní LED matici hubu.

- Typ: příkazový blok
- Poznámka: vybraný hub musí mít interní LED matici.

### `Nastavit pixel matice` (Pokročilý) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Nastaví jas jednoho pixelu na interní LED matici hubu. Aktualizuje se pouze vybraný pixel; zbytek displeje zůstane beze změny. Pole polohy pixelu používají hodnoty sloupce a řádku, přičemž pixel `1, 1` je v levém horním rohu.

- Typ: příkazový blok
- Poznámka: vybraný hub musí mít interní LED matici.

### `Otočit orientaci matice` (Pokročilý) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Otočí orientaci obsahu zobrazeného na interní LED matici hubu po směru nebo proti směru hodinových ručiček. Každé otočení změní orientaci displeje o 90 stupňů a ovlivní světelné bloky spuštěné po něm.

- Typ: příkazový blok
- Poznámka: vybraný hub musí mít interní LED matici.

### `Nastavit orientaci matice` (Pokročilý) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Nastaví orientaci obsahu zobrazeného na interní LED matici hubu. Výchozí orientace je vzpřímená a vybraná orientace ovlivní světelné bloky spuštěné po ní.

- Typ: příkazový blok
- Možnosti orientace: `vzpřímeně`, `vlevo`, `vpravo`, `vzhůru nohama`
- Poznámka: vybraný hub musí mít interní LED matici.

## Bloky světel senzoru vzdálenosti

### `Rozsvítit senzor vzdálenosti` (Začátečník) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Nastaví světla na vybraném senzoru vzdálenosti. Blok může zapnout nebo vypnout jednotlivá světla senzoru a může použít reportovací blok seznamu k ovládání jasu každého světla.

- Typ: příkazový blok
- Poznámka: dostupné pouze pro hub MINDSTORMS Robot Inventor.

## Bloky světel BuWizz 3

### `BuWizz 3 nastavit barvu LED na` (Začátečník) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Nastaví barvu LED na vybraném portu BuWizz 3 pomocí vestavěných barevných možností.

- Typ: příkazový blok

### `BuWizz 3 nastavit barvu LED na (text)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Nastaví barvu LED BuWizz 3 pomocí textové hodnoty barvy.

- Typ: příkazový blok
- Typické použití: dynamické názvy barev z proměnných

### `BuWizz 3 nastavit barvu LED na (RGB)` (Pokročilý) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Nastaví barvu LED BuWizz 3 pomocí explicitních kanálů RGB.

- Typ: příkazový blok
- Typické použití: plně vlastní řízení barev a přechody
