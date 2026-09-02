---
id: Light
title: Світло
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Світло

Сторінка описує блоки категорії **Light** для керування LED та світловими виходами на підтримуваних хабах.

## Базові світлові блоки

### `Встановити колір LED` (Початківець) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Встановлює колір LED хаба із попередньо заданих варіантів.

- Тип: командний блок
- Типове використання: індикація стану (ready/running/warning/error)

### `Перемкнути світло на` (Початківець) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Встановлює вибраний світловий вихід у цільове значення яскравості/рівня.

- Тип: командний блок
- Типове використання: яскравість фар, індикація інтенсивності

### `Вимкнути світло` (Початківець) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Вимикає вибраний світловий вихід.

- Тип: командний блок
- Типове використання: вимкнення моделі, економія батареї

### `Technic Move: перемкнути світло на` (Початківець) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Варіант `Перемкнути світло на` для цілі Technic Move.

- Тип: командний блок

## Блоки внутрішньої LED-матриці

### `Увімкнути світлову матрицю` (Просунутий) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Показує вибране зображення на внутрішній LED-матриці хаба й одразу переходить до наступного блоку в стеку. Зображення залишається на дисплеї, доки інший блок не змінить внутрішню LED-матрицю або програма не зупиниться.

- Тип: командний блок
- Примітка: вибраний хаб повинен мати внутрішню LED-матрицю.

### `Написати на світловій матриці` (Початківець) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Показує текстовий рядок на внутрішній LED-матриці хаба, прокручуючи по одній літері за раз.

- Тип: командний блок
- Примітка: вибраний хаб повинен мати внутрішню LED-матрицю.

### `Вимкнути пікселі матриці` (Початківець) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Вимикає всі світла на внутрішній LED-матриці хаба.

- Тип: командний блок
- Примітка: вибраний хаб повинен мати внутрішню LED-матрицю.

### `Встановити піксель матриці` (Просунутий) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Встановлює яскравість одного пікселя на внутрішній LED-матриці хаба. Оновлюється лише вибраний піксель; решта дисплея залишається без змін. Поля позиції пікселя використовують значення стовпця та рядка, а піксель `1, 1` розташований у верхньому лівому куті.

- Тип: командний блок
- Примітка: вибраний хаб повинен мати внутрішню LED-матрицю.

### `Повернути орієнтацію матриці` (Просунутий) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Повертає орієнтацію того, що відображається на внутрішній LED-матриці хаба, за годинниковою стрілкою або проти неї. Кожен поворот змінює орієнтацію дисплея на 90 градусів і впливає на світлові блоки, що виконуються після нього.

- Тип: командний блок
- Примітка: вибраний хаб повинен мати внутрішню LED-матрицю.

### `Встановити орієнтацію матриці` (Просунутий) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Встановлює орієнтацію того, що відображається на внутрішній LED-матриці хаба. Типова орієнтація - вертикальна, а вибрана орієнтація впливає на світлові блоки, що виконуються після неї.

- Тип: командний блок
- Варіанти орієнтації: `вертикально`, `ліворуч`, `праворуч`, `догори дриґом`
- Примітка: вибраний хаб повинен мати внутрішню LED-матрицю.

## Світлові блоки датчика відстані

### `Підсвітити датчик відстані` (Початківець) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Налаштовує світла на вибраному датчику відстані. Блок може вмикати або вимикати окремі світла датчика й може використовувати блок-репортер списку для керування яскравістю кожного світла.

- Тип: командний блок
- Примітка: доступно лише для хаба MINDSTORMS Robot Inventor.

## Світлові блоки BuWizz 3

### `BuWizz 3: встановити колір LED` (Початківець) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Встановлює колір LED на вибраному порту BuWizz 3 з вбудованих варіантів.

- Тип: командний блок

### `BuWizz 3: встановити колір LED (рядок)` (Гуру) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Встановлює колір LED BuWizz 3 за текстовим значенням.

- Тип: командний блок

### `BuWizz 3: встановити колір LED (RGB)` (Просунутий) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Встановлює колір LED BuWizz 3 через канали RGB.

- Тип: командний блок
