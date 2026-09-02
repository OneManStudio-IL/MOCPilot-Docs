---
id: Sensors
title: Sensoren
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Sensoren

Sensorblokken lezen de status van hub/apparaat en leveren gegevens voor voorwaarden, gebeurtenissen en besturingslogica.

## Apparaat- en hubsensoren

### `Hub batterijniveau` (Beginner) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Geeft het huidige batterijniveau van de hub terug.

### `Hub-batterijspanning` (Gevorderd) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Geeft de batterijspanning van de geselecteerde hub terug in volt.

- Type: numeriek reporterblok
- Alleen beschikbaar voor hubs die batterijspanning rapporteren.
- Geeft `NaN` terug wanneer de geselecteerde hub niet is verbonden.

### `Apparaat % batterij` (Beginner) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Geeft het huidige batterijniveau van de telefoon/tablet waarop MOCPilot draait terug (in procenten).

### `Bordtemperatuur` (Gevorderd) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Geeft de temperatuur van het hubbord terug.

- Alleen beschikbaar voor `BuWizz 2` en `BuWizz 3`.

### `Hub-versnellingsmeter` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Geeft ruwe versnellingsmetergegevens terug die door de geselecteerde hub worden gerapporteerd.

- Asopties: `x`, `y`, `z`

### `Hub-versnelling` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Geeft versnellingsgegevens terug die door de geselecteerde hub worden gerapporteerd.

- Asopties: `x`, `y`, `z`

### `Knop ingedrukt` (Beginner) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Controleert of een geselecteerde hubknop overeenkomt met de gekozen status.

- Statusopties: `ingedrukt`, `vrijgegeven`
- Typische knopoptie: `center` (afhankelijk van hub)

- Opmerking: beschikbare knopopties kunnen verschillen per hubmodel.

### `Apparaattype` (Beginner) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Geeft het type aangesloten apparaat terug voor de geselecteerde poort.

- Type: rapporteurblok
- Typisch gebruik: detecteren welk apparaat is aangesloten voordat apparaat-specifieke logica wordt uitgevoerd

### `Apparaat accelerometer` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Geeft ruwe accelerometerwaarden van apparaatsensoren terug.

- Asopties: `x`, `y`, `z`

### `Apparaat versnelling` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Geeft versnellingsgegevens van apparaatsensoren terug.

- Asopties: `x`, `y`, `z`

## Oriëntatie- en kantelsensoren

### `Apparaatkanteling` (Gevorderd) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Geeft kantelgegevens terug van de telefoon/tablet waarop MOCPilot draait.

- Asopties: `pitch`, `roll`

### `Kanteling` (Beginner) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Geeft de kantelhoek voor de geselecteerde as terug.

- Asopties: `helling`, `rol`, `gieren`
- Opmerking: `gieren` is alleen beschikbaar op hubs die gier-data ondersteunen.

### `Haal oriëntatie op` (Beginner) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Geeft de huidige oriëntatiestatus van de hub terug.

- Uitvoeropties: `tekst`, `index`
- Oriëntatiewaarden: `Front`, `Top`, `Right`, `Back`, `Bottom`, `Left`

### `Is oriëntatie omhoog` (Beginner) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Controleert of de oriëntatie van de hub overeenkomt met de geselecteerde "omhoog"-oriëntatie.

- Oriëntatieopties: `Front`, `Top`, `Right`, `Back`, `Bottom`, `Left`

### `Stel kanteloriëntatie in` (Gevorderd) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Stelt de referentieoriëntatie in die wordt gebruikt door kantel-/oriëntatieblokken.

- Oriëntatieopties: `Front`, `Top`, `Right`, `Back`, `Bottom`, `Left`

## Timer- en bewegingssensoren

### `Timer` (Gevorderd) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Geeft de timerwaarde in seconden terug.

### `Reset timer` (Gevorderd) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Reset de timer naar nul.

## Poortsensorblokken

### `Technic afstandssensor` (Beginner) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Geeft afstandswaarden van een Technic afstandssensor terug.

- Eenheidsopties: `mm`, `cm`, `duim`, `%`

### `Technic wanneer afstand is` (Beginner) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Activeert/controleert de afstandsvoorwaarde voor een Technic afstandssensor.

- Vergelijkopties: `dichterbij dan`, `verder dan`, `precies op`
- Eenheidsopties: `mm`, `cm`, `duim`, `%`

### `Technic-kleursensor modus instellen` (Gevorderd) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Dit blok stelt de Technic-kleursensor in op de geselecteerde modus.

- Opmerking: Het wijzigen van de modus van de kleursensor kan je programma op onverwachte manieren beïnvloeden. De Technic-kleursensor kan bijvoorbeeld geen kleuren of gereflecteerd licht lezen wanneer hij in de modus `"omgevingslicht"` staat.

### `Technic kleursensor waarde` (Beginner) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Geeft de gedetecteerde kleurwaarde van een Technic sensor terug.

- Uitvoeropties: `waarde`, `tekst`

### `Technic wanneer kleur is` (Beginner) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Activeert/controleert wanneer de gedetecteerde kleur overeenkomt met de geselecteerde kleur.

### `Technic gereflecteerd licht` (Beginner) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Geeft de intensiteit van gereflecteerd licht terug.

### `Technic wanneer gereflecteerd licht is` (Beginner) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Activeert/controleert de drempelwaarde voor gereflecteerd licht.

- Vergelijkopties: `<`, `=`, `>`

### `Technic omgevingslicht` (Beginner) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Geeft de intensiteit van omgevingslicht terug.

### `Technic wanneer omgevingslicht is` (Beginner) {#block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg" />
Activeert/controleert de drempelwaarde voor omgevingslicht.

- Vergelijkopties: `<`, `=`, `>`

### `Technic ruwe kleur` (Beginner) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Geeft de ruwe kleurkanaalwaarde van de Technic sensor terug.

- Kanaalopties: `rood`, `groen`, `blauw`

### `BOOST afstandssensor` (Beginner) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Geeft de afstand van een BOOST afstandssensor terug.

- Eenheidsopties: `%`, `cm`, `duim`

### `BOOST wanneer afstand is` (Beginner) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Activeert/controleert de afstandsvoorwaarde voor de BOOST afstandssensor.

- Vergelijkopties: `dichterbij dan`, `verder dan`, `precies op`
- Eenheidsopties: `%`, `cm`, `duim`

### `BOOST kleursensor` (Beginner) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Geeft de kleur terug die door een BOOST sensor wordt gedetecteerd.

- Uitvoeropties: `waarde`, `tekst`

### `BOOST is kleur` (Beginner) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Controleert of de BOOST sensor momenteel de geselecteerde kleur detecteert.

### `BOOST gereflecteerd licht` (Beginner) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Geeft de waarde van gereflecteerd licht van de BOOST sensor terug.

### `BOOST wanneer gereflecteerd licht is` (Beginner) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Activeert/controleert de drempelwaarde voor gereflecteerd licht van de BOOST sensor.

- Vergelijkopties: `<`, `=`, `>`

### `Technic Move stel vermogensmodus in` (Beginner) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Stelt de vermogensmodus van Technic Move in.

- Modusopties: `normaal`, `boost`

### `BuWizz-uitgangsspanning` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Geeft de huidige uitgangsspanning terug die door een BuWizz-hub wordt gerapporteerd.

- Alleen beschikbaar voor ondersteunde BuWizz-hubs.

### `BuWizz-poortstroom` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Geeft het stroomverbruik terug dat voor de geselecteerde BuWizz-hubpoort wordt gerapporteerd.

- Alleen beschikbaar voor ondersteunde BuWizz-hubs en poorten.

### `WeDo 2 afstand` (Beginner) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Geeft de afstand van een WeDo 2 afstandssensor terug.

- Eenheidsopties: `%`, `cm`, `duim`

### `WeDo 2 wanneer afstand is` (Beginner) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Activeert/controleert een afstandsvoorwaarde voor een WeDo 2-afstandssensor.

- Vergelijkingsopties: `closer than`, `farther than`, `exactly at`
- Eenheidsopties: `%`, `cm`, `inch`

### `WeDo 2 kanteling` (Beginner) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Geeft de kantelwaarde van een WeDo 2 kantelsensor terug.

- Asopties: `helling`, `rol`
