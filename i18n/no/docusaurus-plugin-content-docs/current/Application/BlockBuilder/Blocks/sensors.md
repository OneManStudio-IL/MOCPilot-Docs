---
id: Sensors
title: Sensorer
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Sensorer

Sensorblokker leser hub-/enhetstilstand og gir data til betingelser, hendelser og kontrolllogikk.

## Enhets- og hub-sensorer

### `Hub batterinivå` (Nybegynner) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Returnerer gjeldende batterinivå for huben.

### `Hub-batterispenning` (Avansert) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Returnerer batterispenningen til den valgte huben i volt.

- Type: numerisk rapportblokk
- Bare tilgjengelig for huber som rapporterer batterispenning.
- Returnerer `NaN` når den valgte huben ikke er tilkoblet.

### `Enhet % batteri` (Nybegynner) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Returnerer batterinivået til telefonen/nettbrettet som kjører MOCPilot (i prosent).

### `Korttemperatur` (Avansert) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Returnerer temperatur på hubens kretskort.

- Tilgjengelig kun for `BuWizz 2` og `BuWizz 3`.

### `Hub-akselerometer` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Returnerer rå akselerometerdata rapportert av den valgte huben.

- Aksevalg: `x`, `y`, `z`

### `Hub-akselerasjon` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Returnerer akselerasjonsdata rapportert av den valgte huben.

- Aksevalg: `x`, `y`, `z`

### `Knapp trykket` (Nybegynner) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Sjekker om valgt hub-knapp matcher valgt tilstand.

- Tilstandsvalg: `trykket`, `sluppet`
- Typisk knapp: `senter`
- Merk: tilgjengelige knapper kan variere mellom huber.

### `Enhetstype` (Nybegynner) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Returnerer typen enhet koblet til valgt port.

- Type: rapportørblokk
- Typisk bruk: identifisere tilkoblet enhet før logikk kjøres

### `Enhet akselerometer` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Returnerer rå akselerometerverdier.

- Aksevalg: `x`, `y`, `z`

### `Enhet akselerasjon` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Returnerer akselerasjonsdata.

- Aksevalg: `x`, `y`, `z`

## Orientering og tilt

### `Enhetshelling` (Avansert) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Returnerer hellingsdata fra telefonen/nettbrettet som kjører MOCPilot.

- Aksevalg: `pitch`, `roll`

### `Tilt` (Nybegynner) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Returnerer tilt-vinkel.

- Aksevalg: `stigning`, `rulling`, `yaw`
- Merk: `yaw` støttes ikke av alle huber.

### `Hent orientering` (Nybegynner) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Returnerer gjeldende orientering.

- Output: `tekst`, `indeks`
- Verdier: `Foran`, `Topp`, `Høyre`, `Bak`, `Bunn`, `Venstre`

### `Er orientering opp` (Nybegynner) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Sjekker om orientering samsvarer med valgt "opp".

### `Sett tilt-orientering` (Avansert) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Setter referanse for tilt/orientering.

## Timer og bevegelse

### `Timer` (Avansert) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Returnerer tid i sekunder.

### `Nullstill timer` (Avansert) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Setter timer til null.

## Portsensorer

### `Technic avstandssensor` (Nybegynner) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Returnerer avstand.

### `Technic når avstand er` (Nybegynner) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Sjekker/utløser avstandsbetingelse.

### `Technic fargesensor sett modus` (Avansert) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Denne blokken setter Technic-fargesensoren til den valgte modusen.

- Merk: Endring av fargesensor-modus kan påvirke programmet ditt på uventede måter. For eksempel kan Technic-fargesensoren ikke lese farger eller reflektert lys når den er i `"omgivelseslys"`-modus.

### `Technic fargesensorverdi` (Nybegynner) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Returnerer fargeverdi.

### `Technic når farge er` (Nybegynner) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Sjekker/utløser farge.

### `Technic reflektert lys` (Nybegynner) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Returnerer reflektert lys.

### `Technic omgivelseslys` (Nybegynner) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Returnerer omgivelseslys.

### `Technic råfarge` (Nybegynner) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Returnerer rå RGB.

### `BOOST avstandssensor` (Nybegynner) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Returnerer avstand.

### `BOOST fargesensor` (Nybegynner) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Returnerer farge.

### `BOOST reflektert lys` (Nybegynner) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Returnerer reflektert lys.

### `Technic Move sett effektmodus` (Nybegynner) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Setter effektmodus.

### `BuWizz-utgangsspenning` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Returnerer gjeldende utgangsspenning rapportert av en BuWizz-hub.

- Bare tilgjengelig for støttede BuWizz-huber.

### `BuWizz-portstrøm` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Returnerer strømforbruket rapportert for den valgte BuWizz-hubporten.

- Bare tilgjengelig for støttede BuWizz-huber og porter.

### `WeDo 2 avstand` (Nybegynner) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Returnerer avstand.

### `WeDo 2 når avstand er` (Nybegynner) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Utløser/kontrollerer en avstandsbetingelse for en WeDo 2-avstandssensor.

- Sammenligningsvalg: `closer than`, `farther than`, `exactly at`
- Enhetsvalg: `%`, `cm`, `inch`

### `WeDo 2 tilt` (Nybegynner) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Returnerer tilt-verdi.
