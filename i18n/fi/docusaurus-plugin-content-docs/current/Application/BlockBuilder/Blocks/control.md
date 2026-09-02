---
id: Control
title: Ohjaus
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Ohjaus

Ohjauslohkot hallitsevat suorituksen kulkua: odotukset, silmukat, ehdot ja skriptien pysäytys.

## Odotuslohkot

### `Odota` (Aloittelija) {#block_control_wait_for}

<img src={useBaseUrl('/img/blocks/block_control_wait_for.svg')} alt="block_control_wait_for.svg" />

Pysäyttää nykyisen skriptin määritellyksi ajaksi.

### `Odota kunnes` (Edistynyt) {#block_control_wait_until}

<img src={useBaseUrl('/img/blocks/block_control_wait_until.svg')} alt="block_control_wait_until.svg" />

Pysäyttää skriptin, kunnes ehto on tosi.

## Silmukkalohkot

### `Toista` (Edistynyt) {#block_control_repeat_for}

<img src={useBaseUrl('/img/blocks/block_control_repeat_for.svg')} alt="block_control_repeat_for.svg" />

Suorittaa sisäiset lohkot tietyn määrän kertoja.

### `Toista kunnes` (Edistynyt) {#block_control_repeat_until}

<img src={useBaseUrl('/img/blocks/block_control_repeat_until.svg')} alt="block_control_repeat_until.svg" />

Suorittaa lohkoja, kunnes ehto on tosi.

### `Ikuisesti` (Edistynyt) {#block_control_repeat_forever}

<img src={useBaseUrl('/img/blocks/block_control_repeat_forever.svg')} alt="block_control_repeat_forever.svg" />

Suorittaa lohkoja jatkuvasti, kunnes ohjelma tai skripti pysäytetään.

## Ehtolohkot

### `Jos` (Aloittelija) {#block_control_if}

<img src={useBaseUrl('/img/blocks/block_control_if.svg')} alt="block_control_if.svg" />

Suorittaa lohkot vain, jos ehto on tosi.

### `Jos / Muuten` (Edistynyt) {#block_control_if_else}

<img src={useBaseUrl('/img/blocks/block_control_if_else.svg')} alt="block_control_if_else.svg" />

Suorittaa toisen haaran, jos ehto on tosi, muuten toisen.

### `Tee tämä ja tämä` (Guru) {#block_control_do_this_and_this}

<img src={useBaseUrl('/img/blocks/block_control_do_this_and_this.svg')} alt="block_control_do_this_and_this.svg" />

Suorittaa kaksi lohkosarjaa peräkkäin yhtenä toimintona.

## Pysäytyslohkot

### `Pysäytä` (Aloittelija) {#block_control_stop}

<img src={useBaseUrl('/img/blocks/block_control_stop.svg')} alt="block_control_stop.svg" />

Pysäyttää skriptin suorittamisen (laajuus riippuu valinnasta).

- Vaihtoehdot: `kaikki`, `tämä pino`, `ja lopeta ohjelma`

### `Pysäytä muut pinot` (Guru) {#block_control_stop_other_stacks}

<img src={useBaseUrl('/img/blocks/block_control_stop_other_stacks.svg')} alt="block_control_stop_other_stacks.svg" />

Pysäyttää kaikki muut käynnissä olevat pinot, mutta jatkaa nykyistä.

## Hubin ohjauslohkot

### `Aseta yhteys` (Aloittelija) {#block_hubs_control_set_connect}

<img src={useBaseUrl('/img/blocks/block_hubs_control_set_connect.svg')} alt="block_hubs_control_set_connect.svg" />

Ohjaa hubin yhteystilaa.

- Vaihtoehdot: `yhdistä`, `katkaise`

### `Aseta hubin määritys` (Edistynyt) {#block_hubs_set_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="block_hubs_set_hub_config.svg" />
Asettaa valitun hubin yhteen sen tuetuista määritysprofiileista.

- Käytettävissä vain hubeilla, jotka tarjoavat hubin määritysasetuksia.
- Tyypillinen käyttö: vaihda määritettävä hubi, kuten Technic Move Hub, toiseen tallennettuun määritykseen ennen seuraavien lohkojen suorittamista.

### `Hubin määritys` (Edistynyt) {#block_hubs_all_control_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="block_hubs_all_control_hub_config.svg" />
Palauttaa valitun hubin nykyisen määrityksen.

- Tyyppi: raporttilohko
- Tulostusmuodon vaihtoehdot: `text`, `index`
- Käytettävissä vain hubeilla, jotka tarjoavat hubin määritysasetuksia.
- Palauttaa `NaN`, kun valittu hubi ei ole yhdistetty tai määritystä ei ole saatavilla.

### `Onko yhdistetty` (Aloittelija) {#block_hubs_all_sensors_is_connected}

<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_connected.svg')} alt="block_hubs_all_sensors_is_connected.svg" />

Palauttaa, onko hub yhdistetty.

- Tyyppi: boolean-arvo

### `BuWizz 2 aseta tehotila` (Aloittelija) {#block_hubs_buwizz_sensors_set_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_set_power_mode.svg')} alt="block_hubs_buwizz_sensors_set_power_mode.svg" />

Asettaa BuWizz 2 -hubin tehotilan.

- Tilat: `Slow`, `Normal`, `Fast`, `Ludicrous`

### `BuWizz 2 hae tehotila` (Guru) {#block_hubs_buwizz_sensors_get_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_power_mode.svg')} alt="block_hubs_buwizz_sensors_get_power_mode.svg" />

Palauttaa nykyisen tehotilan.

- Muoto: `teksti`, `indeksi`

### `MouldKing aseta ohjauskanava` (Edistynyt) {#block_hubs_mouldking_control_set_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_set_control_channel.svg')} alt="block_hubs_mouldking_control_set_control_channel.svg" />

Asettaa aktiivisen ohjauskanavan.

- Kanavat: `A`, `B`, `C`

### `MouldKing hae ohjauskanava` (Edistynyt) {#block_hubs_mouldking_control_get_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_get_control_channel.svg')} alt="block_hubs_mouldking_control_get_control_channel.svg" />

Palauttaa aktiivisen ohjauskanavan.

- Muoto: `teksti`, `indeksi`
