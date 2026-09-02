---
id: Sensors
title: Sensores
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Sensores

Los bloques de sensores leen el estado del hub/dispositivo y proporcionan datos para condiciones, eventos y lógica de control.

## Sensores del dispositivo y del hub

### `Nivel de batería del hub` (Principiante) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Devuelve el nivel actual de batería del hub.

### `Voltaje de batería del hub` (Avanzado) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Devuelve el voltaje de la batería del hub seleccionado en voltios.

- Tipo: bloque reportero numérico
- Disponible solo para hubs que informan voltaje de batería.
- Devuelve `NaN` cuando el hub seleccionado no está conectado.

### `Batería del dispositivo %` (Principiante) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Devuelve el nivel de batería del dispositivo (teléfono/tableta) en porcentaje.

### `Temperatura de la placa` (Avanzado) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Devuelve la temperatura de la placa del hub.

- Disponible solo en `BuWizz 2` y `BuWizz 3`.

### `Acelerómetro del hub` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Devuelve los datos sin procesar del acelerómetro reportados por el hub seleccionado.

- Ejes: `x`, `y`, `z`

### `Aceleración del hub` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Devuelve los datos de aceleración reportados por el hub seleccionado.

- Ejes: `x`, `y`, `z`

### `Botón presionado` (Principiante) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Comprueba si el botón seleccionado coincide con el estado elegido.

- Estados: `presionado`, `soltado`
- Opción típica: `centro`
- Nota: las opciones pueden variar según el hub.

### `Tipo de dispositivo` (Principiante) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Devuelve el tipo de dispositivo conectado al puerto.

- Tipo: bloque reportero
- Uso típico: detectar dispositivo antes de ejecutar lógica específica

### `Acelerómetro del dispositivo` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Devuelve valores del acelerómetro.

- Ejes: `x`, `y`, `z`

### `Aceleración del dispositivo` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Devuelve datos de aceleración.

- Ejes: `x`, `y`, `z`

## Sensores de orientación e inclinación

### `Inclinación del dispositivo` (Avanzado) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Devuelve los datos de inclinación del teléfono/tableta donde se ejecuta MOCPilot.

- Ejes: `pitch`, `roll`

### `Inclinación` (Principiante) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Devuelve el ángulo de inclinación.

- Ejes: `inclinación`, `balanceo`, `guiñada`
- Nota: `guiñada` depende del hub.

### `Obtener orientación` (Principiante) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Devuelve la orientación actual del hub.

- Formato: `texto`, `índice`
- Valores: `Delante`, `Superior`, `Derecha`, `Trasero`, `Fondo`, `Izquierda`

### `Orientación es arriba` (Principiante) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Comprueba si la orientación coincide.

### `Establecer orientación de inclinación` (Avanzado) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Configura la referencia de orientación.

## Temporizador y movimiento

### `Temporizador` (Avanzado) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Devuelve el tiempo en segundos.

### `Reiniciar temporizador` (Avanzado) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Reinicia el temporizador.

## Sensores de puerto

### `Sensor de distancia Technic` (Principiante) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Devuelve distancia.

- Unidades: `mm`, `cm`, `pulgadas`, `%`

### `Technic cuando distancia es` (Principiante) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Evalúa condición de distancia.

- Opciones: `más cerca que`, `más lejos que`, `exactamente en`

### `Technic establecer modo del sensor de color` (Avanzado) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Este bloque configura el sensor de color Technic en el modo seleccionado.

- Nota: Cambiar el modo del Sensor de color puede afectar tu programa de formas inesperadas. Por ejemplo, el sensor de color Technic no puede leer colores ni luz reflejada cuando está en modo `"ambiente"`.

### `Sensor de color Technic` (Principiante) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Devuelve color detectado.

- Salida: `valor`, `texto`

### `Technic cuando color es` (Principiante) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Evalúa coincidencia de color.

### `Luz reflejada Technic` (Principiante) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Devuelve luz reflejada.

### `Technic cuando luz reflejada es` (Principiante) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Evalúa condición de luz.

### `Luz ambiente Technic` (Principiante) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Devuelve luz ambiente.

### `Color bruto Technic` (Principiante) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Devuelve canales de color.

### `Sensor BOOST distancia` (Principiante) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Devuelve distancia BOOST.

### `Sensor BOOST color` (Principiante) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Devuelve color BOOST.

### `WeDo 2 distancia` (Principiante) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Devuelve distancia WeDo.

### `WeDo 2 cuando distancia es` (Principiante) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Activa/comprueba una condición de distancia para un sensor de distancia WeDo 2.

- Opciones de comparación: `closer than`, `farther than`, `exactly at`
- Unidades: `%`, `cm`, `inch`

### `Voltaje de salida BuWizz` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Devuelve el voltaje de salida actual reportado por un hub BuWizz.

- Disponible solo para hubs BuWizz compatibles.

### `Corriente del puerto BuWizz` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Devuelve el consumo de corriente reportado para el puerto seleccionado del hub BuWizz.

- Disponible solo para hubs y puertos BuWizz compatibles.

### `WeDo 2 inclinación` (Principiante) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Devuelve inclinación.