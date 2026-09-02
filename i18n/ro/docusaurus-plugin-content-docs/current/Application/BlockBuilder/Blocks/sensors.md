---
id: Sensors
title: Senzori
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Senzori

Blocurile de senzori citesc starea hub-ului/dispozitivului și furnizează date pentru condiții, evenimente și logică de control.

## Senzori dispozitiv și hub

### `Nivel baterie hub` (Începător) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Returnează nivelul curent al bateriei hub-ului.

### `Tensiunea bateriei hubului` (Avansat) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Returnează tensiunea bateriei hubului selectat în volți.

- Tip: bloc raportor numeric
- Disponibil doar pentru huburi care raportează tensiunea bateriei.
- Returnează `NaN` când hubul selectat nu este conectat.

### `Baterie dispozitiv %` (Începător) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Returnează nivelul bateriei dispozitivului (telefon/tabletă) în procente.

### `Temperatura plăcii` (Avansat) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Returnează temperatura plăcii hub-ului.

- Disponibil doar pentru `BuWizz 2` și `BuWizz 3`.

### `Accelerometrul hubului` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Returnează date brute de accelerometru raportate de hubul selectat.

- Opțiuni axă: `x`, `y`, `z`

### `Accelerația hubului` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Returnează date de accelerație raportate de hubul selectat.

- Opțiuni axă: `x`, `y`, `z`

### `Buton apăsat` (Începător) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Verifică dacă un buton selectat al hub-ului corespunde stării selectate.

- Opțiuni stare: `apăsat`, `eliberat`
- Opțiune tipică: `centru`
- Notă: opțiunile pot diferi în funcție de modelul hub-ului

### `Tip dispozitiv` (Începător) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Returnează tipul dispozitivului conectat la portul selectat.

- Tip: bloc reporter
- Utilizare tipică: detectarea dispozitivului înainte de logică specifică

### `Accelerometru dispozitiv` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Returnează valorile brute ale accelerometrului.

- Opțiuni axă: `x`, `y`, `z`

### `Accelerație dispozitiv` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Returnează datele de accelerație.

- Opțiuni axă: `x`, `y`, `z`

## Senzori de orientare și înclinare

### `Înclinarea dispozitivului` (Avansat) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Returnează date de înclinare de la telefonul/tableta pe care rulează MOCPilot.

- Opțiuni axă: `pitch`, `roll`

### `Înclinare` (Începător) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Returnează unghiul de înclinare.

- Opțiuni axă: `înclinare`, `rotire`, `derapaj`
- Notă: `derapaj` este disponibil doar pe anumite hub-uri

### `Obține orientarea` (Începător) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Returnează orientarea curentă a hub-ului.

- Opțiuni output: `text`, `index`
- Valori: `Față`, `Sus`, `Dreapta`, `Spate`, `Jos`, `Stânga`

### `Este orientarea sus` (Începător) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Verifică dacă orientarea corespunde direcției „sus”.

- Opțiuni: `Față`, `Sus`, `Dreapta`, `Spate`, `Jos`, `Stânga`

### `Setează orientarea înclinării` (Avansat) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Configurează referința de orientare.

- Opțiuni: `Față`, `Sus`, `Dreapta`, `Spate`, `Jos`, `Stânga`

## Timer și senzori de mișcare

### `Timer` (Avansat) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Returnează valoarea timerului în secunde.

### `Resetează timerul` (Avansat) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Resetează timerul la zero.

## Blocuri senzori port

### `Senzor distanță Technic` (Începător) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Returnează distanța măsurată.

- Unități: `mm`, `cm`, `inci`, `%`

### `Technic când distanța este` (Începător) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Verifică/declanșează condiția de distanță.

- Opțiuni: `mai aproape decât`, `mai departe decât`, `exact la`
- Unități: `mm`, `cm`, `inci`, `%`

### `Technic setează modul senzorului de culoare` (Avansat) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Acest bloc setează senzorul de culoare Technic pe modul selectat.

- Notă: Schimbarea modului senzorului de culoare poate afecta programul în moduri neașteptate. De exemplu, senzorul de culoare Technic nu poate citi culori sau lumină reflectată când este în modul `"ambiental"`.

### `Valoare culoare Technic` (Începător) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Returnează culoarea detectată.

- Output: `valoare`, `șir`

### `Technic când culoarea este` (Începător) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Declanșează când culoarea corespunde.

### `Lumină reflectată Technic` (Începător) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Returnează intensitatea luminii reflectate.

### `Technic când lumina reflectată este` (Începător) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Verifică pragul luminii reflectate.

- Opțiuni: `<`, `=`, `>`

### `Lumină ambientală Technic` (Începător) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Returnează lumina ambientală.

### `Technic când lumina ambientală este` (Începător) {#block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg" />
Verifică pragul luminii ambientale.

- Opțiuni: `<`, `=`, `>`

### `Culoare brută Technic` (Începător) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Returnează valorile RGB brute.

- Canale: `roșu`, `verde`, `albastru`

### `Senzor distanță BOOST` (Începător) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Returnează distanța.

- Unități: `%`, `cm`, `inci`

### `BOOST când distanța este` (Începător) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Verifică condiția de distanță.

- Opțiuni: `mai aproape decât`, `mai departe decât`, `exact la`
- Unități: `%`, `cm`, `inci`

### `Culoare BOOST` (Începător) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Returnează culoarea detectată.

- Output: `valoare`, `șir`

### `BOOST este culoare` (Începător) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Verifică dacă senzorul detectează culoarea.

### `Lumină reflectată BOOST` (Începător) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Returnează lumina reflectată.

### `BOOST când lumina reflectată este` (Începător) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Verifică pragul luminii reflectate.

- Opțiuni: `<`, `=`, `>`

### `Technic Move setează modul de putere` (Începător) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Setează modul de putere.

- Opțiuni: `normal`, `impuls`

### `Tensiune de ieșire BuWizz` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Returnează tensiunea de ieșire curentă raportată de un hub BuWizz.

- Disponibil doar pentru huburi BuWizz acceptate.

### `Curent port BuWizz` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Returnează consumul de curent raportat pentru portul selectat al hubului BuWizz.

- Disponibil doar pentru huburi și porturi BuWizz acceptate.

### `Distanță WeDo 2` (Începător) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Returnează distanța.

### `WeDo 2 când distanța este` (Începător) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Declanșează/verifică o condiție de distanță pentru un senzor de distanță WeDo 2.

- Opțiuni comparație: `closer than`, `farther than`, `exactly at`
- Opțiuni unitate: `%`, `cm`, `inch`

### `Înclinare WeDo 2` (Începător) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Returnează înclinarea.

- Axe: `înclinare`, `rotire`
