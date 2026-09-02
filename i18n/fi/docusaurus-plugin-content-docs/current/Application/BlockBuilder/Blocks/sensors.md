---
id: Sensors
title: Sensorit
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Sensorit

Sensorilohkot lukevat hubin/laitteen tilaa ja tuottavat dataa ehdoille, tapahtumille ja ohjauslogiikalle.

## Laitteen ja hubin sensorit

### `Hubin akun taso` (Aloittelija) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Palauttaa hubin nykyisen akun tason.

### `Hubin akkujännite` (Edistynyt) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Palauttaa valitun hubin akkujännitteen voltteina.

- Tyyppi: numeerinen raporttilohko
- Käytettävissä vain hubeilla, jotka raportoivat akkujännitteen.
- Palauttaa `NaN`, kun valittu hubi ei ole yhdistetty.

### `Laitteen akun %` (Aloittelija) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Palauttaa laitteen (puhelin/tabletti) akun tason prosentteina.

### `Piirilevyn lämpötila` (Edistynyt) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Palauttaa hubin lämpötilan.

- Saatavilla vain: `BuWizz 2` ja `BuWizz 3`.

### `Hubin kiihtyvyysanturi` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Palauttaa valitun hubin raportoimat raakakiihtyvyysanturitiedot.

- Akselivaihtoehdot: `x`, `y`, `z`

### `Hubin kiihtyvyys` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Palauttaa valitun hubin raportoimat kiihtyvyystiedot.

- Akselivaihtoehdot: `x`, `y`, `z`

### `Painike painettu` (Aloittelija) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Tarkistaa, vastaako valittu painike tilaa.

- Tilat: `painettu`, `vapautettu`
- Tyypillinen painike: `center`

- Huom: painikkeet voivat vaihdella hubin mukaan.

### `Laitetyyppi` (Aloittelija) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Palauttaa porttiin liitetyn laitteen tyypin.

- Tyyppi: reporter-lohko
- Tyypillinen käyttö: tunnistaa laite ennen ohjausta

### `Laitteen kiihtyvyysanturi` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Palauttaa kiihtyvyysanturin arvot.

- Akselit: `x`, `y`, `z`

### `Laitteen kiihtyvyys` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Palauttaa kiihtyvyysdatan.

- Akselit: `x`, `y`, `z`

## Suunta ja kallistus

### `Laitteen kallistus` (Edistynyt) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Palauttaa kallistustiedot puhelimesta/tabletista, jossa MOCPilot on käynnissä.

- Akselivaihtoehdot: `pitch`, `roll`

### `Kallistus` (Aloittelija) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Palauttaa kallistuskulman.

- Akselit: `kallistus`, `kallistus`, `kallistus`

### `Hae suunta` (Aloittelija) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Palauttaa hubin suunnan.

- Muoto: `teksti`, `indeksi`
- Arvot: `Etuosa`, `Yläosa`, `Oikea`, `Takana`, `Pohja`, `Vasen`

### `Onko suunta ylös` (Aloittelija) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Tarkistaa suunnan.

### `Aseta kallistuksen suunta` (Edistynyt) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Asettaa viitesuunnan.

## Ajastin

### `Ajastin` (Edistynyt) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Palauttaa ajan sekunteina.

### `Nollaa ajastin` (Edistynyt) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Nollaa ajastimen.

## Porttisensorit

### `Technic-etäisyysanturi` (Aloittelija) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Palauttaa etäisyyden.

- Yksiköt: `mm`, `cm`, `tuuma`, `%`

### `Technic kun etäisyys on` (Aloittelija) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Tarkistaa etäisyyden ehdon.

- Vaihtoehdot: `lähempänä kuin`, `kauempana kuin`, `täsmälleen kohdalla`

### `Technic-värisensorin tilan asetus` (Edistynyt) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Tämä lohko asettaa Technic-värisensorin valittuun tilaan.

- Huomautus: Värisensorin tilan muuttaminen voi vaikuttaa ohjelmaasi odottamattomilla tavoilla. Esimerkiksi Technic-värisensori ei voi lukea värejä tai heijastunutta valoa, kun se on tilassa `"ympäristövalo"`.

### `Technic-värianturi arvo` (Aloittelija) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Palauttaa värin.

### `Technic kun väri on` (Aloittelija) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Tarkistaa värin.

### `Technic heijastettu valo` (Aloittelija) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Palauttaa heijastetun valon.

### `Technic kun heijastettu valo on` (Aloittelija) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Tarkistaa valon ehdon.

### `Technic ympäristövalo` (Aloittelija) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Palauttaa ympäristön valon.

### `Technic raakaväri` (Aloittelija) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Palauttaa värikanavat.

### `BOOST-etäisyysanturi` (Aloittelija) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Palauttaa etäisyyden.

### `BOOST kun etäisyys on` (Aloittelija) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Tarkistaa etäisyyden.

### `BOOST-värianturi` (Aloittelija) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Palauttaa värin.

### `BOOST on väri` (Aloittelija) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Tarkistaa värin.

### `BOOST heijastettu valo` (Aloittelija) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Palauttaa valon.

### `BOOST kun heijastettu valo on` (Aloittelija) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Tarkistaa valon.

### `Technic Move aseta tehotila` (Aloittelija) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Asettaa tehotilan.

### `BuWizz-lähtöjännite` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Palauttaa BuWizz-hubin raportoiman nykyisen lähtöjännitteen.

- Käytettävissä vain tuetuilla BuWizz-hubeilla.

### `BuWizz-portin virta` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Palauttaa valitun BuWizz-hubin portin raportoiman virrankulutuksen.

- Käytettävissä vain tuetuilla BuWizz-hubeilla ja porteilla.

### `WeDo 2 etäisyys` (Aloittelija) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Palauttaa etäisyyden.

### `WeDo 2 kun etäisyys on` (Aloittelija) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Käynnistää/tarkistaa etäisyysehdon WeDo 2 -etäisyysanturille.

- Vertailuvaihtoehdot: `closer than`, `farther than`, `exactly at`
- Yksikkövaihtoehdot: `%`, `cm`, `inch`

### `WeDo 2 kallistus` (Aloittelija) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Palauttaa kallistuksen.
