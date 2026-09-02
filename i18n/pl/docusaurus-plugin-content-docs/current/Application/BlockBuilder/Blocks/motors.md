---
id: Motors
title: Silniki
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Silniki

Bloki silników służą do uruchamiania, zatrzymywania, pozycjonowania oraz strojenia silników podłączonych do portów huba.

## Podstawowe bloki sterowania silnikiem

### `Uruchom silnik` (Początkujący) {#block_hubs_all_motors_port_start_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor.svg')} alt="block_hubs_all_motors_port_start_motor.svg" />
Uruchamia wybrany silnik.

- Opcje kierunku: zgodnie z ruchem wskazówek zegara / przeciwnie do ruchu wskazówek zegara

### `Zatrzymaj silnik` (Początkujący) {#block_hubs_all_motors_port_stop_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_stop_motor.svg')} alt="block_hubs_all_motors_port_stop_motor.svg" />
Zatrzymuje wybrany silnik.

### `Uruchom na` (Zaawansowany) {#block_hubs_all_motors_port_run_for}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for.svg')} alt="block_hubs_all_motors_port_run_for.svg" />
Uruchamia wybrany silnik na określony czas/kąt/obrót zgodnie z ustawieniami bloku.

- Opcje kierunku: zgodnie z ruchem wskazówek zegara / przeciwnie do ruchu wskazówek zegara
- Opcje jednostek: `obroty`, `stopnie`, `sekundy`
- Uwaga: wymaga silnika obsługującego enkoder.

### `Uruchom silnik z prędkością` (Początkujący) {#block_hubs_all_motors_port_start_motor_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="block_hubs_all_motors_port_start_motor_at_speed.svg" />
Uruchamia silnik z określoną prędkością.

### `Uruchom na z prędkością` (Zaawansowany) {#block_hubs_all_motors_port_run_for_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for_at_speed.svg')} alt="block_hubs_all_motors_port_run_for_at_speed.svg" />
Uruchamia silnik na określony czas/wartość z określoną prędkością.

- Opcje jednostek: `obroty`, `stopnie`, `sekundy`
- Uwaga: wymaga silnika obsługującego enkoder.

### `Ustaw prędkość silnika` (Zaawansowany) {#block_hubs_all_motors_port_set_motor_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_speed.svg')} alt="block_hubs_all_motors_port_set_motor_speed.svg" />
Ustawia prędkość używaną przez inne bloki sterujące silnikiem.

## Bloki pozycjonowania i ruchu

### `Przejdź do pozycji` (Zaawansowany) {#block_hubs_all_motors_port_go_to_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_position.svg')} alt="block_hubs_all_motors_port_go_to_position.svg" />
Przesuwa silnik do docelowej pozycji absolutnej.

- Opcje ścieżki: `najkrótsza droga`, `zgodnie z ruchem wskazówek zegara`, `przeciwnie do ruchu wskazówek zegara`
- Uwaga: wymaga silnika obsługującego enkoder.

### `Przejdź do pozycji względnej` (Początkujący) {#block_hubs_all_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_relative_position.svg')} alt="block_hubs_all_motors_port_go_to_relative_position.svg" />
Przesuwa silnik o względną wartość.

- Uwaga: wymaga silnika obsługującego enkoder.

### `BuWizz 3 przejdź do pozycji względnej` (Początkujący) {#block_hubs_buwizz3_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_motors_port_go_to_relative_position.svg')} alt="block_hubs_buwizz3_motors_port_go_to_relative_position.svg" />
Wariant dla BuWizz 3.

- Uwaga: wymaga silnika obsługującego enkoder.

### `Ustaw pozycję względną` (Początkujący) {#block_hubs_all_motors_port_set_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_relative_position.svg')} alt="block_hubs_all_motors_port_set_relative_position.svg" />
Ustawia odniesienie pozycji względnej silnika.

- Uwaga: wymaga silnika obsługującego enkoder.

### `Kalibruj przekładnię kierowniczą` (Początkujący) {#block_hubs_all_motors_port_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_calibrate_steering_rack.svg')} alt="block_hubs_all_motors_port_calibrate_steering_rack.svg" />
Kalibruje pozycję neutralną układu kierowniczego.

- Wymaganie: silnik musi obsługiwać enkoder.
- Wymaganie mechaniczne: zakres ruchu musi być fizycznie ograniczony.
- Działanie: blok wykonuje pomiar zakresu ruchu i oblicza dane kalibracyjne.
- Wyjście: wyniki zapisywane są do przekazanych zmiennych.

## Bloki strojenia i bezpieczeństwa

### `Ustaw zachowanie silnika przy zatrzymaniu` (Guru) {#block_hubs_all_motors_port_set_motor_to_at_stop}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_to_at_stop.svg')} alt="block_hubs_all_motors_port_set_motor_to_at_stop.svg" />
Ustawia tryb zatrzymania silnika.

- Opcje: `hamulec`, `utrzymaj pozycję`, `swobodny obrót`

### `Ustaw wykrywanie zablokowania` (Guru) {#block_hubs_all_motors_port_set_motors_stall_detection}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motors_stall_detection.svg')} alt="block_hubs_all_motors_port_set_motors_stall_detection.svg" />
Włącza lub wyłącza wykrywanie zablokowania.

- Uwaga: tylko dla MINDSTORMS Robot Inventor.

### `Ustaw przyspieszenie` (Guru) {#block_hubs_all_motors_port_set_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_acceleration.svg')} alt="block_hubs_all_motors_port_set_acceleration.svg" />
Ustawia profil przyspieszenia.

- Opcje: `domyślny`, `szybki`, `zrównoważony`, `płynny`, `wolny`, `bardzo wolny`

### `Ustaw hamowanie` (Guru) {#block_hubs_all_motors_port_set_deceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_deceleration.svg')} alt="block_hubs_all_motors_port_set_deceleration.svg" />
Ustawia profil zwalniania.

- Opcje: `domyślny`, `szybki`, `zrównoważony`, `płynny`, `wolny`, `bardzo wolny`

## Bloki raportujące silnika

### `Pozycja` (Początkujący) {#block_hubs_all_motors_port_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_position.svg')} alt="block_hubs_all_motors_port_position.svg" />
Zwraca aktualną pozycję silnika.

### `Pozycja względna` (Początkujący) {#block_hubs_all_motors_port_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_relative_position.svg')} alt="block_hubs_all_motors_port_relative_position.svg" />
Zwraca aktualną pozycję względną.

### `Prędkość` (Początkujący) {#block_hubs_all_motors_port_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_speed.svg')} alt="block_hubs_all_motors_port_speed.svg" />
Zwraca aktualną prędkość silnika.

### `Moc` (Zaawansowany) {#block_hubs_all_motors_port_power}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_power.svg')} alt="block_hubs_all_motors_port_power.svg" />
Zwraca aktualną moc silnika.

- Uwaga: tylko dla MINDSTORMS Robot Inventor.

## Bloki silników Technic Move

### `Uruchom silniki z prędkością` (Początkujący) {#block_hubs_technicmove_motors_start_motors_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_start_motors_at_speed.svg')} alt="block_hubs_technicmove_motors_start_motors_at_speed.svg" />
Uruchamia silniki napędowe Technic Move.

### `Impuls mocy` (Początkujący) {#block_hubs_technicmove_motors_power_pulse}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="block_hubs_technicmove_motors_power_pulse.svg" />
Wysyła polecenie impulsu mocy do wybranego Technic Move Hub.

- Dostępne tylko dla Technic Move Hub.
- Typowe użycie: krótkie wzmocnienie lub wybudzenie układu napędowego Technic Move przed kontynuowaniem kolejnych bloków.

### `Zatrzymaj silniki` (Początkujący) {#block_hubs_technicmove_motors_stop_motors}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_stop_motors.svg')} alt="block_hubs_technicmove_motors_stop_motors.svg" />
Zatrzymuje silniki napędowe.

### `Hamulec` (Początkujący) {#block_hubs_technicmove_motors_brake}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_brake.svg')} alt="block_hubs_technicmove_motors_brake.svg" />
Włącza/wyłącza hamowanie.

- Opcje: `wyłącz`, `włącz`

### `Ustaw przekładnię kierowniczą na` (Początkujący) {#block_hubs_technicmove_motors_set_steering_rack_to}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_set_steering_rack_to.svg')} alt="block_hubs_technicmove_motors_set_steering_rack_to.svg" />
Ustawia docelową pozycję układu kierowniczego.

### `Kalibruj przekładnię kierowniczą` (Początkujący) {#block_hubs_technicmove_motors_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_calibrate_steering_rack.svg')} alt="block_hubs_technicmove_motors_calibrate_steering_rack.svg" />
Kalibruje układ kierowniczy Technic Move.

- Uwaga: wymagane fizyczne ograniczenie zakresu ruchu.