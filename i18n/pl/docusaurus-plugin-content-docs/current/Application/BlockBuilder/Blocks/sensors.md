---
id: Sensors
title: Czujniki
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Czujniki

Bloki czujników odczytują stan huba/urządzenia i dostarczają dane do warunków, zdarzeń oraz logiki sterowania.

## Czujniki urządzenia i huba

### `Poziom baterii huba` (Początkujący) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Zwraca aktualny poziom baterii huba.

### `Napięcie baterii huba` (Zaawansowany) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Zwraca napięcie baterii wybranego huba w woltach.

- Typ: numeryczny blok raportujący
- Dostępne tylko dla hubów raportujących napięcie baterii.
- Zwraca `NaN`, gdy wybrany hub nie jest połączony.

### `Bateria urządzenia %` (Początkujący) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Zwraca aktualny poziom baterii telefonu/tabletu (w procentach).

### `Temperatura płytki` (Zaawansowany) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Zwraca temperaturę płytki huba.

- Dostępne tylko dla `BuWizz 2` i `BuWizz 3`.

### `Akcelerometr huba` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Zwraca surowe dane akcelerometru raportowane przez wybrany hub.

- Osie: `x`, `y`, `z`

### `Przyspieszenie huba` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Zwraca dane przyspieszenia raportowane przez wybrany hub.

- Osie: `x`, `y`, `z`

### `Przycisk wciśnięty` (Początkujący) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Sprawdza, czy wybrany przycisk huba odpowiada wybranemu stanowi.

- Opcje stanu: `naciśnięty`, `zwolniony`
- Typowa opcja przycisku: `środkowy`

- Uwaga: dostępne przyciski mogą się różnić w zależności od modelu huba.

### `Typ urządzenia` (Początkujący) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Zwraca typ urządzenia podłączonego do wybranego portu.

- Typ: blok raportujący
- Typowe użycie: wykrycie urządzenia przed uruchomieniem odpowiedniej logiki

### `Akcelerometr urządzenia` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Zwraca surowe dane akcelerometru.

- Opcje osi: `x`, `y`, `z`

### `Przyspieszenie urządzenia` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Zwraca dane przyspieszenia.

- Opcje osi: `x`, `y`, `z`

## Czujniki orientacji i nachylenia

### `Nachylenie urządzenia` (Zaawansowany) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Zwraca dane nachylenia telefonu/tabletu, na którym działa MOCPilot.

- Osie: `pitch`, `roll`

### `Nachylenie` (Początkujący) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Zwraca kąt nachylenia dla wybranej osi.

- Opcje osi: `pitch`, `roll`, `yaw`
- Uwaga: `yaw` dostępny tylko na wybranych hubach.

### `Pobierz orientację` (Początkujący) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Zwraca aktualną orientację huba.

- Opcje wyjścia: `tekst`, `indeks`
- Wartości: `Przód`, `Góra`, `Prawo`, `Tył`, `Dół`, `Lewo`

### `Czy orientacja jest w górę` (Początkujący) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Sprawdza, czy orientacja odpowiada wybranej pozycji „góra”.

- Opcje: `Przód`, `Góra`, `Prawo`, `Tył`, `Dół`, `Lewo`

### `Ustaw orientację nachylenia` (Zaawansowany) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Konfiguruje orientację odniesienia dla bloków nachylenia.

- Opcje: `Przód`, `Góra`, `Prawo`, `Tył`, `Dół`, `Lewo`

## Timer i ruch urządzenia

### `Timer` (Zaawansowany) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Zwraca wartość timera w sekundach.

### `Resetuj timer` (Zaawansowany) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Resetuje timer do zera.

## Bloki czujników portów

### `Czujnik odległości Technic` (Początkujący) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Zwraca odległość z czujnika Technic.

- Opcje jednostek: `mm`, `cm`, `cal`, `%`

### `Technic gdy odległość jest` (Początkujący) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Sprawdza warunek odległości.

- Opcje: `bliżej niż`, `dalej niż`, `dokładnie na`
- Jednostki: `mm`, `cm`, `cal`, `%`

### `Technic ustaw tryb czujnika koloru` (Zaawansowany) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Ten blok ustawia czujnik koloru Technic na wybrany tryb.

- Uwaga: Zmiana trybu czujnika koloru może wpłynąć na program w nieoczekiwany sposób. Na przykład czujnik koloru Technic nie może odczytywać kolorów ani światła odbitego, gdy jest w trybie `"otoczenia"`.

### `Wartość koloru Technic` (Początkujący) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Zwraca wykryty kolor.

- Opcje wyjścia: `wartość`, `ciąg`

### `Technic gdy kolor jest` (Początkujący) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Sprawdza, czy kolor odpowiada wybranemu.

### `Światło odbite Technic` (Początkujący) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Zwraca intensywność światła odbitego.

### `Technic gdy światło odbite jest` (Początkujący) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Sprawdza próg światła odbitego.

- Opcje: `<`, `=`, `>`

### `Światło otoczenia Technic` (Początkujący) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Zwraca natężenie światła otoczenia.

### `Technic gdy światło otoczenia jest` (Początkujący) {#block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg" />
Sprawdza próg światła otoczenia.

- Opcje: `<`, `=`, `>`

### `Surowy kolor Technic` (Początkujący) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Zwraca kanały RGB.

- Opcje: `czerwony`, `zielony`, `niebieski`

### `Czujnik odległości BOOST` (Początkujący) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Zwraca odległość z czujnika BOOST.

- Jednostki: `%`, `cm`, `cal`

### `BOOST gdy odległość jest` (Początkujący) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Sprawdza warunek odległości.

- Opcje: `bliżej niż`, `dalej niż`, `dokładnie na`
- Jednostki: `%`, `cm`, `cal`

### `Kolor BOOST` (Początkujący) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Zwraca kolor z czujnika BOOST.

- Opcje: `wartość`, `ciąg`

### `BOOST czy kolor` (Początkujący) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Sprawdza, czy kolor jest wykryty.

### `Światło odbite BOOST` (Początkujący) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Zwraca światło odbite.

### `BOOST gdy światło odbite jest` (Początkujący) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Sprawdza próg światła.

- Opcje: `<`, `=`, `>`

### `Technic Move ustaw tryb mocy` (Początkujący) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Ustawia tryb mocy.

- Opcje: `normal`, `boost`

### `Napięcie wyjściowe BuWizz` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Zwraca bieżące napięcie wyjściowe raportowane przez hub BuWizz.

- Dostępne tylko dla obsługiwanych hubów BuWizz.

### `Prąd portu BuWizz` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Zwraca pobór prądu raportowany dla wybranego portu huba BuWizz.

- Dostępne tylko dla obsługiwanych hubów i portów BuWizz.

### `WeDo 2 odległość` (Początkujący) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Zwraca odległość.

- Jednostki: `%`, `cm`, `cal`

### `WeDo 2 gdy odległość wynosi` (Początkujący) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Uruchamia/sprawdza warunek odległości dla czujnika odległości WeDo 2.

- Opcje porównania: `closer than`, `farther than`, `exactly at`
- Jednostki: `%`, `cm`, `inch`

### `WeDo 2 nachylenie` (Początkujący) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Zwraca nachylenie.

- Opcje: `pitch`, `roll`
