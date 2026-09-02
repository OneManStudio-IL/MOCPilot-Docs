---
id: Sensors
title: Sensorer
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Sensorer

Sensorblock läser hubb-/enhetstillstånd och tillhandahåller data för villkor, händelser och kontrolllogik.

## Enhets- och hubbsensorer

### `Hubbens batterinivå` (Nybörjare) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Returnerar hubbens aktuella batterinivå.

### `Hubbens batterispänning` (Avancerad) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Returnerar den valda hubbens batterispänning i volt.

- Typ: numeriskt rapportblock
- Endast tillgänglig för hubbar som rapporterar batterispänning.
- Returnerar `NaN` när den valda hubben inte är ansluten.

### `Enhetens % batteri` (Nybörjare) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Returnerar den aktuella batterinivån för telefonen/surfplattan som kör MOCPilot (i procent).

### `Korttemperatur` (Avancerad) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Returnerar hubbens korttemperatur.

- Tillgänglig endast för `BuWizz 2` och `BuWizz 3`.

### `Hubbens accelerometer` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Returnerar rå accelerometerdata som rapporteras av den valda hubben.

- Axelval: `x`, `y`, `z`

### `Hubbens acceleration` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Returnerar accelerationsdata som rapporteras av den valda hubben.

- Axelval: `x`, `y`, `z`

### `Knapp nedtryckt` (Nybörjare) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Kontrollerar om en vald hubbknapp matchar det valda tillståndet.

- Tillståndsalternativ: `nedtryckt`, `släppt`
- Typiskt knappalternativ: `mitten` (hubberoende)

- Obs: tillgängliga knappalternativ kan skilja sig mellan olika hubbmodeller (olika hubbar kan exponera olika uppsättningar knappar).

### `Enhetstyp` (Nybörjare) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Returnerar ansluten enhetstyp för den valda porten.

- Typ: reporterblock
- Typisk användning: upptäcka vilken enhet som är ansluten innan enhetsspecifik logik körs

### `Enhetsaccelerometer` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Returnerar råa accelerometervärden från enhetssensorer.

- Axelalternativ: `x`, `y`, `z`

### `Enhetsacceleration` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Returnerar accelerationsdata från enhetssensorer.

- Axelalternativ: `x`, `y`, `z`

## Orienterings- och lutningssensorer

### `Enhetens lutning` (Avancerad) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Returnerar lutningsdata från telefonen/surfplattan som kör MOCPilot.

- Axelval: `pitch`, `roll`

### `Lutning` (Nybörjare) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Returnerar lutningsvinkeln för den valda axeln.

- Axelalternativ: `lutning`, `rullning`, `yaw`
- Obs: `yaw` är endast tillgängligt på hubbar som tillhandahåller yaw-data.

### `Hämta orientering` (Nybörjare) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Returnerar hubbens aktuella orienteringstillstånd.

- Alternativ för utdataformat: `text`, `index`
- Orienteringsvärden: `Fram`, `Topp`, `Höger`, `Bak`, `Botten`, `Vänster`

### `Är orientering uppåt` (Nybörjare) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Kontrollerar om hubbens orientering matchar den valda "uppåt"-orienteringen.

- Orienteringsalternativ: `Fram`, `Topp`, `Höger`, `Bak`, `Botten`, `Vänster`

### `Ställ in lutningsorientering` (Avancerad) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Konfigurerar den orienteringsreferens som används av lutnings-/orienteringsrelaterade block.

- Orienteringsalternativ: `Fram`, `Topp`, `Höger`, `Bak`, `Botten`, `Vänster`

## Timer- och enhetsrörelsesensorer

### `Timer` (Avancerad) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Returnerar timervärdet i sekunder.

### `Återställ timer` (Avancerad) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Återställer timern till noll.

## Portsensorblock

### `Technic avståndssensor` (Nybörjare) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Returnerar avståndsvärden från en Technic-avståndssensor.

- Enhetsalternativ: `mm`, `cm`, `tum`, `%`

### `Technic när avstånd är` (Nybörjare) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Utlöser/kontrollerar avståndsvillkor för en Technic-avståndssensor.

- Jämförelsealternativ: `närmare än`, `längre än`, `precis på`
- Enhetsalternativ: `mm`, `cm`, `tum`, `%`

### `Technic färgsensor ställ in läge` (Avancerad) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Det här blocket ställer in Technic-färgsensorn till det valda läget.

- Obs: Att ändra färgsensorns läge kan påverka ditt program på oväntade sätt. Till exempel kan Technic-färgsensorn inte läsa färger eller reflekterat ljus när den är i läget `"omgivningsljus"`.

### `Technic färgsensorvärde` (Nybörjare) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Returnerar detekterat färgvärde från en Technic-avståndssensor.

- Utdatalternativ: `värde`, `sträng`

### `Technic när färg är` (Nybörjare) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Utlöser/kontrollerar när den detekterade färgen matchar vald färg.

### `Technic reflekterat ljus` (Nybörjare) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Returnerar intensiteten för reflekterat ljus.

### `Technic när reflekterat ljus är` (Nybörjare) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Utlöser/kontrollerar tröskelvillkor för reflekterat ljus.

- Jämförelsealternativ: `<`, `=`, `>`

### `Technic omgivningsljus` (Nybörjare) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Returnerar intensiteten för omgivningsljus.

### `Technic när omgivningsljus är` (Nybörjare) {#block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg" />
Utlöser/kontrollerar tröskelvillkor för omgivningsljus.

- Jämförelsealternativ: `<`, `=`, `>`

### `Technic rå färg` (Nybörjare) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Returnerar rått färgkanalvärde från Technic-sensorn.

- Kanalalternativ: `röd`, `grön`, `blå`

### `BOOST avståndssensor` (Nybörjare) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Returnerar avstånd från en BOOST-avståndssensor.

- Enhetsalternativ: `%`, `cm`, `tum`

### `BOOST när avstånd är` (Nybörjare) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Utlöser/kontrollerar avståndsvillkor för BOOST-avståndssensorn.

- Jämförelsealternativ: `närmare än`, `längre än`, `precis på`
- Enhetsalternativ: `%`, `cm`, `tum`

### `BOOST färgsensor` (Nybörjare) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Returnerar färgen som detekteras av en BOOST-sensor.

- Utdatalternativ: `värde`, `sträng`

### `BOOST är färg` (Nybörjare) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Kontrollerar om BOOST-sensorn för närvarande detekterar vald färg.

### `BOOST reflekterat ljus` (Nybörjare) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Returnerar värdet för reflekterat ljus från BOOST-sensorn.

### `BOOST när reflekterat ljus är` (Nybörjare) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Utlöser/kontrollerar tröskelvillkor för reflekterat ljus för BOOST-sensorn.

- Jämförelsealternativ: `<`, `=`, `>`

### `Technic Move ställ in effektläge` (Nybörjare) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Ställer in effektläget för Technic Move.

- Lägesalternativ: `normal`, `boost`

### `BuWizz-utspänning` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Returnerar den aktuella utspänningen som rapporteras av en BuWizz-hubb.

- Endast tillgänglig för BuWizz-hubbar som stöds.

### `BuWizz-portström` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Returnerar strömförbrukningen som rapporteras för den valda BuWizz-hubbporten.

- Endast tillgänglig för BuWizz-hubbar och portar som stöds.

### `WeDo 2 avstånd` (Nybörjare) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Returnerar avstånd från WeDo 2-avståndssensorn.

- Enhetsalternativ: `%`, `cm`, `tum`

### `WeDo 2 när avstånd är` (Nybörjare) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Utlöser/kontrollerar ett avståndsvillkor för en WeDo 2-avståndssensor.

- Jämförelseval: `closer than`, `farther than`, `exactly at`
- Enhetsval: `%`, `cm`, `inch`

### `WeDo 2 lutning` (Nybörjare) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Returnerar lutningsvärde från WeDo 2-lutningssensorn.

- Axelalternativ: `lutning`, `rullning`
