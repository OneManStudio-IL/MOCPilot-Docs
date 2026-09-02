---
id: Light
title: Valo
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Valo

Tällä sivulla kuvataan Valo-kategorian lohkot, joita käytetään LEDien ja valojen ohjaamiseen tuetuissa hubeissa.

## Yleiset valolohkot

### `Aseta LED-väri` (Aloittelija) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Asettaa hubin LEDin värin valmiista vaihtoehdoista.

- Tyyppi: komentolohko
- Tyypillinen käyttö: tilan näyttäminen (valmis, käynnissä, varoitus, virhe)

### `Aseta valo` (Aloittelija) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Asettaa valitun valon kirkkauden tai arvon.

- Tyyppi: komentolohko
- Tyypillinen käyttö: ajovalot, tilan kirkkaus

### `Sammuta valo` (Aloittelija) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Sammuttaa valitun valon.

- Tyyppi: komentolohko
- Tyypillinen käyttö: sammutus, virransäästö

### `Technic Move aseta valo` (Aloittelija) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

`Aseta valo` -lohkon versio Technic Move -hubille.

- Tyyppi: komentolohko
- Tyypillinen käyttö: Move-hubin valon säätö

## Sisäisen LED-matriisin lohkot

### `Kytke valomatriisi päälle` (Edistynyt) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Näyttää valitun kuvan hubin sisäisessä LED-matriisissa ja jatkaa heti pinon seuraavaan lohkoon. Kuva pysyy näytöllä, kunnes toinen lohko muuttaa sisäistä LED-matriisia tai ohjelma pysähtyy.

- Tyyppi: komentolohko
- Huomautus: valitussa hubissa on oltava sisäinen LED-matriisi.

### `Kirjoita valomatriisiin` (Aloittelija) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Näyttää tekstijonon hubin sisäisessä LED-matriisissa vierittämällä yhden kirjaimen kerrallaan.

- Tyyppi: komentolohko
- Huomautus: valitussa hubissa on oltava sisäinen LED-matriisi.

### `Sammuta matriisin pikselit` (Aloittelija) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Sammuttaa kaikki valot hubin sisäisestä LED-matriisista.

- Tyyppi: komentolohko
- Huomautus: valitussa hubissa on oltava sisäinen LED-matriisi.

### `Aseta matriisin pikseli` (Edistynyt) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Asettaa yhden pikselin kirkkauden hubin sisäisessä LED-matriisissa. Vain valittu pikseli päivitetään; muu näyttö säilyy ennallaan. Pikselin sijaintikentät käyttävät sarake- ja riviarvoja, ja pikseli `1, 1` on vasemmassa yläkulmassa.

- Tyyppi: komentolohko
- Huomautus: valitussa hubissa on oltava sisäinen LED-matriisi.

### `Kierrä matriisin suuntaa` (Edistynyt) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Kiertää hubin sisäisessä LED-matriisissa näkyvän sisällön suuntaa myötä- tai vastapäivään. Jokainen kierto muuttaa näytön suuntaa 90 astetta ja vaikuttaa sen jälkeen ajettaviin Valo-lohkoihin.

- Tyyppi: komentolohko
- Huomautus: valitussa hubissa on oltava sisäinen LED-matriisi.

### `Aseta matriisin suunta` (Edistynyt) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Asettaa hubin sisäisessä LED-matriisissa näkyvän sisällön suunnan. Oletussuunta on pystyssä, ja valittu suunta vaikuttaa sen jälkeen ajettaviin Valo-lohkoihin.

- Tyyppi: komentolohko
- Asentovaihtoehdot: `pystyssä`, `vasen`, `oikea`, `ylösalaisin`
- Huomautus: valitussa hubissa on oltava sisäinen LED-matriisi.

## Etäisyysanturin valolohkot

### `Sytytä etäisyysanturi` (Aloittelija) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Asettaa valot valitussa etäisyysanturissa. Lohko voi sytyttää tai sammuttaa yksittäisiä anturin valoja ja käyttää listaraportterilohkoa kunkin valon kirkkauden ohjaamiseen.

- Tyyppi: komentolohko
- Huomautus: saatavilla vain MINDSTORMS Robot Inventor -hubille.

## BuWizz 3 -valolohkot

### `BuWizz 3 aseta LED-väri` (Aloittelija) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Asettaa LED-värin valitussa BuWizz 3 -portissa.

- Tyyppi: komentolohko

### `BuWizz 3 aseta LED-väri (teksti)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Asettaa LED-värin tekstiarvon avulla.

- Tyyppi: komentolohko
- Tyypillinen käyttö: dynaamiset värit muuttujista

### `BuWizz 3 aseta LED-väri (RGB)` (Edistynyt) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Asettaa LED-värin RGB-arvoilla.

- Tyyppi: komentolohko
- Tyypillinen käyttö: tarkka väriohjaus ja gradientit
