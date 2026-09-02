---
id: Light
title: Svetlo
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Svetlo

Táto stránka dokumentuje bloky kategórie Svetlo, ktoré sa používajú na ovládanie LED diód a svetelných výstupov na podporovaných huboch.

## Základné bloky svetla

### `Nastav farbu LED` (Začiatočník) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Nastaví farbu LED na hube pomocou preddefinovaných farebných možností.

- Typ: príkazový blok  
- Typické použitie: zobrazenie stavu (pripravené, beží, upozornenie, chyba)  

### `Nastav svetlo na` (Začiatočník) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Nastaví vybraný svetelný výstup na cieľový jas/hodnotu.

- Typ: príkazový blok  
- Typické použitie: jas svetiel, intenzita indikácie  

### `Vypni svetlo` (Začiatočník) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Vypne vybraný svetelný výstup.

- Typ: príkazový blok  
- Typické použitie: vypínanie, úspora batérie  

### `Technic Move nastav svetlo na` (Začiatočník) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variant bloku `Nastav svetlo na` pre Technic Move hub/svetlo.

- Typ: príkazový blok  
- Typické použitie: nastavenie úrovne svetla na Move hube  

## Bloky internej LED matice

### `Zapnúť svetelnú maticu` (Pokročilý) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Zobrazí vybraný obrázok na internej LED matici hubu a okamžite pokračuje ďalším blokom v zásobníku. Obrázok zostane na displeji, kým iný blok nezmení internú LED maticu alebo kým sa program nezastaví.

- Typ: príkazový blok
- Poznámka: vybraný hub musí mať internú LED maticu.

### `Písať na svetelnú maticu` (Začiatočník) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Zobrazí textový reťazec na internej LED matici hubu posúvaním jedného písmena naraz.

- Typ: príkazový blok
- Poznámka: vybraný hub musí mať internú LED maticu.

### `Vypnúť pixely matice` (Začiatočník) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Vypne všetky svetlá na internej LED matici hubu.

- Typ: príkazový blok
- Poznámka: vybraný hub musí mať internú LED maticu.

### `Nastaviť pixel matice` (Pokročilý) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Nastaví jas jedného pixelu na internej LED matici hubu. Aktualizuje sa iba vybraný pixel; zvyšok displeja zostane nezmenený. Polia polohy pixelu používajú hodnoty stĺpca a riadka, pričom pixel `1, 1` je v ľavom hornom rohu.

- Typ: príkazový blok
- Poznámka: vybraný hub musí mať internú LED maticu.

### `Otočiť orientáciu matice` (Pokročilý) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Otočí orientáciu toho, čo sa zobrazuje na internej LED matici hubu, v smere alebo proti smeru hodinových ručičiek. Každé otočenie zmení orientáciu displeja o 90 stupňov a ovplyvní svetelné bloky spustené po ňom.

- Typ: príkazový blok
- Poznámka: vybraný hub musí mať internú LED maticu.

### `Nastaviť orientáciu matice` (Pokročilý) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Nastaví orientáciu toho, čo sa zobrazuje na internej LED matici hubu. Predvolená orientácia je vzpriamená a vybraná orientácia ovplyvní svetelné bloky spustené po nej.

- Typ: príkazový blok
- Možnosti orientácie: `vzpriamene`, `vľavo`, `vpravo`, `hore nohami`
- Poznámka: vybraný hub musí mať internú LED maticu.

## Bloky svetiel senzora vzdialenosti

### `Rozsvietiť senzor vzdialenosti` (Začiatočník) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Nastaví svetlá na vybranom senzore vzdialenosti. Blok môže zapnúť alebo vypnúť jednotlivé svetlá senzora a môže použiť reportovací blok zoznamu na ovládanie jasu každého svetla.

- Typ: príkazový blok
- Poznámka: dostupné iba pre hub MINDSTORMS Robot Inventor.

## Bloky svetla BuWizz 3

### `BuWizz 3 nastav farbu LED` (Začiatočník) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Nastaví farbu LED na vybranom porte BuWizz 3 pomocou vstavaných farebných možností.

- Typ: príkazový blok  

### `BuWizz 3 nastav farbu LED (text)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Nastaví farbu LED BuWizz 3 pomocou textovej hodnoty farby.

- Typ: príkazový blok  
- Typické použitie: dynamické názvy farieb z premenných  

### `BuWizz 3 nastav farbu LED (RGB)` (Pokročilý) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Nastaví farbu LED BuWizz 3 pomocou explicitných RGB kanálov.

- Typ: príkazový blok  
- Typické použitie: úplné prispôsobenie farieb a gradientov  
