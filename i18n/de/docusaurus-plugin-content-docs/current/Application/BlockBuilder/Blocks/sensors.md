---
id: Sensors
title: Sensoren
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Sensoren

Sensorblöcke lesen Hub-/Gerätezustände und liefern Daten für Bedingungen, Ereignisse und Steuerungslogik.

## Geräte- und Hub-Sensoren

### `Hub-Batteriestand` (Anfänger) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Gibt den aktuellen Hub-Batteriestand zurück.

### `Hub-Batteriespannung` (Fortgeschritten) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Gibt die Batteriespannung des ausgewählten Hubs in Volt zurück.

- Typ: numerischer Reporterblock
- Nur verfügbar für Hubs, die Batteriespannung melden.
- Gibt `NaN` zurück, wenn der ausgewählte Hub nicht verbunden ist.

### `Gerätebatterie %` (Anfänger) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Gibt den aktuellen Batteriestand des Smartphones/Tablets zurück, auf dem MOCPilot läuft.

### `Board-Temperatur` (Fortgeschritten) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Gibt die Temperatur der Hub-Platine zurück.

- Nur verfügbar für `BuWizz 2` und `BuWizz 3`.

### `Hub-Beschleunigungssensor` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Gibt rohe Beschleunigungssensordaten des ausgewählten Hubs zurück.

- Achsenoptionen: `x`, `y`, `z`

### `Hub-Beschleunigung` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Gibt Beschleunigungsdaten des ausgewählten Hubs zurück.

- Achsenoptionen: `x`, `y`, `z`

### `Taste gedrückt` (Anfänger) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Prüft, ob die ausgewählte Hub-Taste dem gewählten Zustand entspricht.

- Statusoptionen: `gedrückt`, `losgelassen`
- Typische Tastenoption: `mitte` (hubabhängig)

### `Gerätetyp` (Anfänger) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Gibt den Typ des verbundenen Geräts am ausgewählten Port zurück.

- Typ: Reporterblock

### `Geräte-Beschleunigungssensor` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Gibt rohe Beschleunigungssensorwerte des Geräts zurück.

- Achsenoptionen: `x`, `y`, `z`

### `Geräte-Beschleunigung` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Gibt Beschleunigungsdaten des Geräts zurück.

- Achsenoptionen: `x`, `y`, `z`

## Orientierungs- und Neigungssensoren

### `Geräteneigung` (Fortgeschritten) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Gibt Neigungsdaten des Smartphones/Tablets zurück, auf dem MOCPilot läuft.

- Achsenoptionen: `pitch`, `roll`

### `Neigung` (Anfänger) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Gibt den Neigungswinkel für die gewählte Achse zurück.

- Achsenoptionen: `pitch`, `roll`, `yaw`

### `Orientierung holen` (Anfänger) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Gibt den aktuellen Orientierungszustand des Hubs zurück.

- Ausgabeoptionen: `text`, `index`
- Orientierungswerte: `Vorne`, `Oben`, `Rechts`, `Hinten`, `Unten`, `Links`

### `Ist Orientierung oben` (Anfänger) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Prüft, ob die Hub-Orientierung der gewählten „oben“-Orientierung entspricht.

- Orientierungsoptionen: `Vorne`, `Oben`, `Rechts`, `Hinten`, `Unten`, `Links`

### `Neigungsorientierung setzen` (Fortgeschritten) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Konfiguriert die Orientierungsreferenz für Neigungs-/Orientierungsblöcke.

## Timer und Bewegung

### `Timer` (Fortgeschritten) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Gibt den Timerwert in Sekunden zurück.

### `Timer zurücksetzen` (Fortgeschritten) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Setzt den Timer auf Null zurück.

## Port-Sensorblöcke

### `Technic Distanzsensor` (Anfänger) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Gibt Distanzwerte eines Technic-Distanzsensors zurück.

- Einheitenoptionen: `mm`, `cm`, `zoll`, `%`

### `Technic wenn Distanz ist` (Anfänger) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Prüft/auslöst Distanzbedingungen für den Technic-Distanzsensor.

- Vergleichsoptionen: `näher als`, `weiter als`, `genau bei`
- Einheitenoptionen: `mm`, `cm`, `zoll`, `%`

### `Technic Sensor-Modus einstellen` (Fortgeschritten) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Dieser Block setzt den Technic-Farbsensor auf den ausgewählten Modus.

- Hinweis: Das Ändern des Farbsensor-Modus kann dein Programm auf unerwartete Weise beeinflussen. Zum Beispiel kann der Technic-Farbsensor keine Farben oder reflektiertes Licht lesen, wenn er sich im Modus `"Umgebungslicht"` befindet.

### `Technic Farbsensorwert` (Anfänger) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Gibt den erkannten Farbwert des Technic-Sensors zurück.

- Ausgabeoptionen: `wert`, `text`

### `Technic wenn Farbe ist` (Anfänger) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Prüft/auslöst, wenn die erkannte Farbe der gewählten Farbe entspricht.

### `Technic reflektiertes Licht` (Anfänger) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Gibt die Intensität des reflektierten Lichts zurück.

### `Technic wenn reflektiertes Licht ist` (Anfänger) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Prüft/auslöst für Schwellwert von reflektiertem Licht.

### `Technic Umgebungslicht` (Anfänger) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Gibt die Intensität des Umgebungslichts zurück.

### `Technic wenn Umgebungslicht ist` (Anfänger) {#block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg" />
Prüft/auslöst für Schwellwert von Umgebungslicht.

### `Technic Rohfarbe` (Anfänger) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Gibt Rohwerte der Farbkanäle des Technic-Sensors zurück.

- Kanaloptionen: `rot`, `grün`, `blau`

### `BOOST Distanzsensor` (Anfänger) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Gibt Distanzwerte des BOOST-Sensors zurück.

- Einheitenoptionen: `%`, `cm`, `zoll`

### `BOOST wenn Distanz ist` (Anfänger) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Prüft/auslöst Distanzbedingungen für BOOST.

- Vergleichsoptionen: `näher als`, `weiter als`, `genau bei`
- Einheitenoptionen: `%`, `cm`, `zoll`

### `BOOST Sensorfarbe` (Anfänger) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Gibt die vom BOOST-Sensor erkannte Farbe zurück.

- Ausgabeoptionen: `wert`, `text`

### `BOOST ist Farbe` (Anfänger) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Prüft, ob der BOOST-Sensor aktuell die gewählte Farbe erkennt.

### `BOOST reflektiertes Licht` (Anfänger) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Gibt den Wert des reflektierten Lichts vom BOOST-Sensor zurück.

### `BOOST wenn reflektiertes Licht ist` (Anfänger) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Prüft/auslöst für Schwellwert von reflektiertem Licht beim BOOST-Sensor.

### `Technic Move Leistungsmodus setzen` (Anfänger) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Setzt den Leistungsmodus von Technic Move.

- Modusoptionen: `normal`, `boost`

### `BuWizz-Ausgangsspannung` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Gibt die aktuelle Ausgangsspannung zurück, die ein BuWizz-Hub meldet.

- Nur verfügbar für unterstützte BuWizz-Hubs.

### `BuWizz-Portstrom` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Gibt die Stromaufnahme zurück, die für den ausgewählten BuWizz-Hub-Port gemeldet wird.

- Nur verfügbar für unterstützte BuWizz-Hubs und -Ports.

### `WeDo 2 Distanz` (Anfänger) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Gibt Distanzwerte des WeDo-2-Distanzsensors zurück.

- Einheitenoptionen: `%`, `cm`, `zoll`

### `WeDo 2 wenn Abstand ist` (Anfänger) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Löst eine Abstandsbedingung für einen WeDo-2-Abstandssensor aus oder prüft sie.

- Vergleichsoptionen: `closer than`, `farther than`, `exactly at`
- Einheitenoptionen: `%`, `cm`, `inch`

### `WeDo 2 Neigung` (Anfänger) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Gibt Neigungswerte des WeDo-2-Neigungssensors zurück.

- Achsenoptionen: `pitch`, `roll`