---
id: Light
title: Свет
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Свет

Световые блоки управляют LED-подсветкой на поддерживаемых хабах и устройствах.

## Общие световые блоки

### `Установить цвет LED` (Начинающий) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Устанавливает цвет LED хаба с помощью предустановленных цветов.

### `Переключить свет на` (Начинающий) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Переключает свет в выбранное состояние/цвет.

### `Выключить свет` (Начинающий) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Выключает свет.

### `Technic Move: переключить свет на` (Начинающий) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Устанавливает свет для Technic Move.

## Блоки внутренней LED-матрицы

### `Включить световую матрицу` (Продвинутый) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Показывает выбранное изображение на внутренней LED-матрице хаба и сразу переходит к следующему блоку в стеке. Изображение остается на дисплее, пока другой блок не изменит внутреннюю LED-матрицу или программа не остановится.

- Тип: командный блок
- Примечание: выбранный хаб должен иметь внутреннюю LED-матрицу.

### `Написать на световой матрице` (Начинающий) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Показывает текстовую строку на внутренней LED-матрице хаба, прокручивая по одной букве за раз.

- Тип: командный блок
- Примечание: выбранный хаб должен иметь внутреннюю LED-матрицу.

### `Выключить пиксели матрицы` (Начинающий) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Выключает все огни на внутренней LED-матрице хаба.

- Тип: командный блок
- Примечание: выбранный хаб должен иметь внутреннюю LED-матрицу.

### `Установить пиксель матрицы` (Продвинутый) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Устанавливает яркость одного пикселя на внутренней LED-матрице хаба. Обновляется только выбранный пиксель; остальная часть дисплея остается без изменений. Поля положения пикселя используют значения столбца и строки, а пиксель `1, 1` находится в левом верхнем углу.

- Тип: командный блок
- Примечание: выбранный хаб должен иметь внутреннюю LED-матрицу.

### `Повернуть ориентацию матрицы` (Продвинутый) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Поворачивает ориентацию того, что отображается на внутренней LED-матрице хаба, по часовой стрелке или против часовой стрелки. Каждый поворот меняет ориентацию дисплея на 90 градусов и влияет на блоки Свет, выполняемые после него.

- Тип: командный блок
- Примечание: выбранный хаб должен иметь внутреннюю LED-матрицу.

### `Установить ориентацию матрицы` (Продвинутый) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Устанавливает ориентацию того, что отображается на внутренней LED-матрице хаба. Ориентация по умолчанию - вертикальная, а выбранная ориентация влияет на блоки Свет, выполняемые после нее.

- Тип: командный блок
- Варианты ориентации: `вертикально`, `влево`, `вправо`, `вверх ногами`
- Примечание: выбранный хаб должен иметь внутреннюю LED-матрицу.

## Световые блоки датчика расстояния

### `Подсветить датчик расстояния` (Начинающий) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Настраивает огни на выбранном датчике расстояния. Блок может включать или выключать отдельные огни датчика и может использовать блок-репортер списка для управления яркостью каждого огня.

- Тип: командный блок
- Примечание: доступно только для хаба MINDSTORMS Robot Inventor.

## Световые блоки BuWizz 3

### `BuWizz 3: установить цвет LED` (Начинающий) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Устанавливает цвет LED порта BuWizz 3.

### `BuWizz 3: установить цвет LED (строка)` (Гуру) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Устанавливает цвет LED BuWizz 3 по строковому значению.

### `BuWizz 3: установить цвет LED (RGB)` (Продвинутый) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Устанавливает цвет LED BuWizz 3 через значения RGB.
