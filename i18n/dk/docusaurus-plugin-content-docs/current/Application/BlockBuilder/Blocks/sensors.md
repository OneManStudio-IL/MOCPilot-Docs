---
id: Sensors
title: Sensorer
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Sensorer

Sensorblokke læser hub-/enhedstilstand og leverer data til betingelser, hændelser og kontrol-logik.

## Enheds- og hubsensorer

### `Hub-batteriniveau` (Begynder) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Returnerer hubbens aktuelle batteriniveau.

### `Hub-batterispænding` (Avanceret) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Returnerer den valgte hubs batterispænding i volt.

- Type: numerisk reporterblok
- Kun tilgængelig for hubs, der rapporterer batterispænding.
- Returnerer `NaN`, når den valgte hub ikke er tilsluttet.

### `Enhedsbatteri %` (Begynder) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Returnerer det aktuelle batteriniveau for telefon/tablet, der kører MOCPilot (i procent).

### `Board-temperatur` (Avanceret) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Returnerer hubbens board-temperatur.

- Kun tilgængelig for `BuWizz 2` og `BuWizz 3`.

### `Hub-accelerometer` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Returnerer rå accelerometerdata rapporteret af den valgte hub.

- Aksevalg: `x`, `y`, `z`

### `Hub-acceleration` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Returnerer accelerationsdata rapporteret af den valgte hub.

- Aksevalg: `x`, `y`, `z`

### `Knap trykket` (Begynder) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Tjekker om en valgt hub-knap matcher den valgte tilstand.

- Tilstandsmuligheder: `trykket`, `frigivet`
- Typisk knapmulighed: `center` (hub-afhængig)

- Bemærk: tilgængelige knapmuligheder kan variere efter hub-model (forskellige hubs kan have forskellige knapsæt).

### `Enhedstype` (Begynder) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Returnerer typen af tilsluttet enhed for den valgte port.

- Type: reporterblok
- Typisk brug: registrér hvilken enhed der er tilsluttet, før enhedsspecifik logik køres

### `Enheds-accelerometer` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Returnerer rå accelerometerværdier fra enhedens sensorer.

- Aksemuligheder: `x`, `y`, `z`

### `Enheds-acceleration` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Returnerer accelerationsdata fra enhedens sensorer.

- Aksemuligheder: `x`, `y`, `z`

## Orienterings- og tilt-sensorer

### `Enhedshældning` (Avanceret) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Returnerer hældningsdata fra telefonen/tabletten, der kører MOCPilot.

- Aksevalg: `pitch`, `roll`

### `Tilt` (Begynder) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Returnerer tilt-vinkel for den valgte akse.

- Aksemuligheder: `hældning`, `rulning`, `gyring`
- Bemærk: `yaw` er kun tilgængelig på hubs, der leverer yaw-data.

### `Hent orientering` (Begynder) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Returnerer hubbens aktuelle orienteringstilstand.

- Outputformat-muligheder: `text`, `index`
- Orienteringsværdier: `Foran`, `Top`, `Højre`, `Bagpå`, `Bund`, `Venstre`

### `Er orientering opad` (Begynder) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Tjekker om hubbens orientering matcher valgt "opad"-orientering.

- Orienteringsmuligheder: `Foran`, `Top`, `Højre`, `Bagpå`, `Bund`, `Venstre`

### `Sæt tilt-orientering` (Avanceret) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Konfigurerer orienteringsreference brugt af tilt-/orienteringsrelaterede blokke.

- Orienteringsmuligheder: `Foran`, `Top`, `Højre`, `Bagpå`, `Bund`, `Venstre`

## Timer og enhedsbevægelse

### `Timer` (Avanceret) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Returnerer timerværdi i sekunder.

### `Nulstil timer` (Avanceret) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Nulstiller timeren til nul.

## Port-sensorblokke

### `Technic afstandssensor` (Begynder) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Returnerer afstandsværdier fra en Technic-afstandssensor.

- Enhedsmuligheder: `mm`, `cm`, `tommer`, `%`

### `Technic når afstand er` (Begynder) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Udløser/tjekker afstandsbetingelse for en Technic-afstandssensor.

- Sammenligningsmuligheder: `nærmere end`, `længere end`, `præcis ved`
- Enhedsmuligheder: `mm`, `cm`, `tommer`, `%`

### `Technic farvesensor sæt tilstand` (Avanceret) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Denne blok sætter Technic-farvesensoren til den valgte tilstand.

- Bemærk: Hvis du ændrer farvesensorens tilstand, kan det påvirke dit program på uventede måder. For eksempel kan Technic-farvesensoren ikke læse farver eller reflekteret lys, når den er i `"omgivelseslys"`-tilstand.

### `Technic farvesensorværdi` (Begynder) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Returnerer registreret farveværdi fra en Technic-afstandssensor.

- Outputmuligheder: `værdi`, `streng`

### `Technic når farve er` (Begynder) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Udløser/tjekker når registreret farve matcher valgt farve.

### `Technic reflekteret lys` (Begynder) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Returnerer intensitet af reflekteret lys.

### `Technic når reflekteret lys er` (Begynder) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Udløser/tjekker tærskelbetingelse for reflekteret lys.

- Sammenligningsmuligheder: `<`, `=`, `>`

### `Technic omgivelseslys` (Begynder) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Returnerer intensitet af omgivelseslys.

### `Technic når omgivelseslys er` (Begynder) {#block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg" />
Udløser/tjekker tærskelbetingelse for omgivelseslys.

- Sammenligningsmuligheder: `<`, `=`, `>`

### `Technic rå farve` (Begynder) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Returnerer rå farvekanalværdi fra Technic-sensor.

- Kanalmuligheder: `red`, `green`, `blue`

### `BOOST sensorafstand` (Begynder) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Returnerer afstand fra en BOOST-afstandssensor.

- Enhedsmuligheder: `%`, `cm`, `tommer`

### `BOOST når afstand er` (Begynder) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Udløser/tjekker afstandsbetingelse for BOOST-afstandssensor.

- Sammenligningsmuligheder: `nærmere end`, `længere end`, `præcis ved`
- Enhedsmuligheder: `%`, `cm`, `tommer`

### `BOOST sensorfarve` (Begynder) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Returnerer farve registreret af en BOOST-sensor.

- Outputmuligheder: `værdi`, `streng`

### `BOOST er farve` (Begynder) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Tjekker om BOOST-sensoren aktuelt registrerer valgt farve.

### `BOOST reflekteret lys` (Begynder) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Returnerer reflekteret lysværdi fra BOOST-sensor.

### `BOOST når reflekteret lys er` (Begynder) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Udløser/tjekker tærskelbetingelse for reflekteret lys for BOOST-sensor.

- Sammenligningsmuligheder: `<`, `=`, `>`

### `Technic Move sæt power mode` (Begynder) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Sætter Technic Move power mode.

- Tilstandsmuligheder: normal, boost

### `BuWizz-udgangsspænding` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Returnerer den aktuelle udgangsspænding rapporteret af en BuWizz-hub.

- Kun tilgængelig for understøttede BuWizz-hubs.

### `BuWizz-portstrøm` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Returnerer strømforbruget rapporteret for den valgte BuWizz-hubport.

- Kun tilgængelig for understøttede BuWizz-hubs og porte.

### `WeDo 2 afstand` (Begynder) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Returnerer afstand fra WeDo 2-afstandssensor.

- Enhedsmuligheder: `%`, `cm`, `tommer`

### `WeDo 2 når afstand er` (Begynder) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Udløser/kontrollerer en afstandsbetingelse for en WeDo 2-afstandssensor.

- Sammenligningsvalg: `closer than`, `farther than`, `exactly at`
- Enhedsvalg: `%`, `cm`, `inch`

### `WeDo 2 tilt` (Begynder) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Returnerer tilt-værdi fra WeDo 2-tiltsensor.

- Aksemuligheder: `hældning`, `rulning`