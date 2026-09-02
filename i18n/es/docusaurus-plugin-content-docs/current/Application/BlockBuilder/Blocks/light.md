---
id: Light
title: Luz
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Luz

Esta página documenta los bloques de la categoría Luz, utilizados para controlar LEDs y salidas de iluminación en hubs compatibles.

## Bloques de luz comunes

### `Establecer color del LED` (Principiante) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Establece el color del LED del hub usando opciones predefinidas.

- Tipo: bloque de comando
- Uso típico: mostrar estado (listo, en ejecución, advertencia, error)

### `Encender luz a` (Principiante) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Ajusta la luz seleccionada a un nivel de brillo o valor objetivo.

- Tipo: bloque de comando
- Uso típico: brillo de faros, intensidad de estado

### `Apagar luz` (Principiante) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Apaga la salida de luz seleccionada.

- Tipo: bloque de comando
- Uso típico: apagado del sistema, ahorro de batería

### `Technic Move encender luz a` (Principiante) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variante de `Encender luz a` para el hub Technic Move.

- Tipo: bloque de comando
- Uso típico: ajustar el nivel de luz del hub Move

## Bloques de matriz LED interna

### `Encender matriz de luces` (Avanzado) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Muestra la imagen seleccionada en la matriz LED interna del hub y continúa inmediatamente con el siguiente bloque de la pila. La imagen permanece en la pantalla hasta que otro bloque cambia la matriz LED interna o el programa se detiene.

- Tipo: bloque de comando
- Nota: el hub seleccionado debe tener una matriz LED interna.

### `Escribir en matriz de luces` (Principiante) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Muestra una cadena de texto en la matriz LED interna del hub desplazando una letra a la vez.

- Tipo: bloque de comando
- Nota: el hub seleccionado debe tener una matriz LED interna.

### `Apagar píxeles de la matriz` (Principiante) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Apaga todas las luces de la matriz LED interna del hub.

- Tipo: bloque de comando
- Nota: el hub seleccionado debe tener una matriz LED interna.

### `Establecer píxel de matriz` (Avanzado) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Establece el brillo de un píxel en la matriz LED interna del hub. Solo se actualiza el píxel seleccionado; el resto de la pantalla permanece sin cambios. Los campos de posición del píxel usan valores de columna y fila, con el píxel `1, 1` en la esquina superior izquierda.

- Tipo: bloque de comando
- Nota: el hub seleccionado debe tener una matriz LED interna.

### `Rotar orientación de matriz` (Avanzado) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Rota la orientación de lo que se muestra en la matriz LED interna del hub en sentido horario o antihorario. Cada rotación cambia la orientación de la pantalla 90 grados y afecta a los bloques de Luz que se ejecutan después.

- Tipo: bloque de comando
- Nota: el hub seleccionado debe tener una matriz LED interna.

### `Establecer orientación de matriz` (Avanzado) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Establece la orientación de lo que se muestra en la matriz LED interna del hub. La orientación predeterminada es vertical, y la orientación seleccionada afecta a los bloques de Luz que se ejecutan después.

- Tipo: bloque de comando
- Opciones de orientación: `vertical`, `izquierda`, `derecha`, `boca abajo`
- Nota: el hub seleccionado debe tener una matriz LED interna.

## Bloques de luces del sensor de distancia

### `Iluminar sensor de distancia` (Principiante) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Establece las luces del sensor de distancia seleccionado. El bloque puede encender o apagar luces individuales del sensor y puede usar un bloque reportero de lista para controlar el brillo de cada luz.

- Tipo: bloque de comando
- Nota: disponible solo en el hub MINDSTORMS Robot Inventor.

## Bloques de luz BuWizz 3

### `BuWizz 3 establecer color LED` (Principiante) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Establece el color del LED en el puerto seleccionado del BuWizz 3.

- Tipo: bloque de comando

### `BuWizz 3 establecer color LED (texto)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Establece el color del LED usando un valor de texto.

- Tipo: bloque de comando
- Uso típico: colores dinámicos desde variables

### `BuWizz 3 establecer color LED (RGB)` (Avanzado) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Establece el color del LED usando valores RGB.

- Tipo: bloque de comando
- Uso típico: control completo de color y gradientes
