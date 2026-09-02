---
id: Light
title: Światło
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Światło

Ta strona opisuje bloki kategorii Światło używane do sterowania diodami LED i wyjściami świetlnymi w obsługiwanych hubach.

## Wspólne bloki światła

### `Ustaw kolor LED` (Początkujący) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Ustawia kolor diody LED huba przy użyciu predefiniowanych opcji kolorów.

- Typ: blok polecenia
- Typowe użycie: wskazywanie stanu (gotowy, w trakcie działania, ostrzeżenie, błąd)

### `Ustaw światło na` (Początkujący) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Ustawia wybrane wyjście światła na docelową jasność/wartość.

- Typ: blok polecenia
- Typowe użycie: jasność świateł, intensywność stanu

### `Wyłącz światło` (Początkujący) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Wyłącza wybrane wyjście światła.

- Typ: blok polecenia
- Typowe użycie: sekwencja wyłączania, oszczędzanie baterii

### `Technic Move ustaw światło na` (Początkujący) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Wariant bloku `Ustaw światło na` dla huba Technic Move.

- Typ: blok polecenia
- Typowe użycie: ustawienie poziomu światła w hubie Move

## Bloki wewnętrznej matrycy LED

### `Włącz matrycę świetlną` (Zaawansowany) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Wyświetla wybrany obraz na wewnętrznej matrycy LED huba i natychmiast przechodzi do następnego bloku w stosie. Obraz pozostaje na wyświetlaczu, dopóki inny blok nie zmieni wewnętrznej matrycy LED albo program się nie zatrzyma.

- Typ: blok polecenia
- Uwaga: wybrany hub musi mieć wewnętrzną matrycę LED.

### `Napisz na matrycy świetlnej` (Początkujący) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Wyświetla tekst na wewnętrznej matrycy LED huba, przewijając po jednej literze.

- Typ: blok polecenia
- Uwaga: wybrany hub musi mieć wewnętrzną matrycę LED.

### `Wyłącz piksele matrycy` (Początkujący) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Wyłącza wszystkie światła na wewnętrznej matrycy LED huba.

- Typ: blok polecenia
- Uwaga: wybrany hub musi mieć wewnętrzną matrycę LED.

### `Ustaw piksel matrycy` (Zaawansowany) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Ustawia jasność jednego piksela na wewnętrznej matrycy LED huba. Aktualizowany jest tylko wybrany piksel; reszta wyświetlacza pozostaje bez zmian. Pola pozycji piksela używają wartości kolumny i wiersza, a piksel `1, 1` znajduje się w lewym górnym rogu.

- Typ: blok polecenia
- Uwaga: wybrany hub musi mieć wewnętrzną matrycę LED.

### `Obróć orientację matrycy` (Zaawansowany) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Obraca orientację tego, co jest wyświetlane na wewnętrznej matrycy LED huba, zgodnie z ruchem wskazówek zegara lub przeciwnie do niego. Każdy obrót zmienia orientację wyświetlacza o 90 stopni i wpływa na bloki Światło uruchamiane później.

- Typ: blok polecenia
- Uwaga: wybrany hub musi mieć wewnętrzną matrycę LED.

### `Ustaw orientację matrycy` (Zaawansowany) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Ustawia orientację tego, co jest wyświetlane na wewnętrznej matrycy LED huba. Domyślna orientacja jest pionowa, a wybrana orientacja wpływa na bloki Światło uruchamiane później.

- Typ: blok polecenia
- Opcje orientacji: `pionowo`, `lewo`, `prawo`, `do góry nogami`
- Uwaga: wybrany hub musi mieć wewnętrzną matrycę LED.

## Bloki świateł czujnika odległości

### `Rozświetl czujnik odległości` (Początkujący) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Ustawia światła na wybranym czujniku odległości. Blok może włączać lub wyłączać pojedyncze światła czujnika i może użyć bloku raportującego listę, aby sterować jasnością każdego światła.

- Typ: blok polecenia
- Uwaga: dostępne tylko dla huba MINDSTORMS Robot Inventor.

## Bloki światła BuWizz 3

### `BuWizz 3 ustaw kolor LED` (Początkujący) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Ustawia kolor LED na wybranym porcie BuWizz 3 przy użyciu wbudowanych opcji kolorów.

- Typ: blok polecenia

### `BuWizz 3 ustaw kolor LED (tekst)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Ustawia kolor LED BuWizz 3 przy użyciu wartości tekstowej.

- Typ: blok polecenia
- Typowe użycie: dynamiczne nazwy kolorów z zmiennych

### `BuWizz 3 ustaw kolor LED (RGB)` (Zaawansowany) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Ustawia kolor LED BuWizz 3 przy użyciu wartości RGB.

- Typ: blok polecenia
- Typowe użycie: pełna kontrola kolorów i gradientów
