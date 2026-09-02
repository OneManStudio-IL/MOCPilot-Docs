---
id: Sensors
title: Sensores
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Sensores

Os blocos de sensores leem o estado do hub/dispositivo e fornecem dados para condições, eventos e lógica de controle.

## Sensores de dispositivo e hub

### `Nível de bateria do hub` (Iniciante) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Retorna o nível atual da bateria do hub.

### `Tensão da bateria do hub` (Avançado) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Retorna a tensão da bateria do hub selecionado em volts.

- Tipo: bloco repórter numérico
- Disponível apenas para hubs que informam tensão da bateria.
- Retorna `NaN` quando o hub selecionado não está conectado.

### `Bateria do dispositivo (%)` (Iniciante) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Retorna o nível atual de bateria do dispositivo (telefone/tablet) em porcentagem.

### `Temperatura da placa` (Avançado) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Retorna a temperatura da placa do hub.

- Disponível apenas para `BuWizz 2` e `BuWizz 3`.

### `Acelerômetro do hub` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Retorna dados brutos do acelerômetro relatados pelo hub selecionado.

- Opções de eixo: `x`, `y`, `z`

### `Aceleração do hub` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Retorna dados de aceleração relatados pelo hub selecionado.

- Opções de eixo: `x`, `y`, `z`

### `Botão pressionado` (Iniciante) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Verifica se o botão selecionado corresponde ao estado escolhido.

- Opções de estado: `pressionado`, `solto`
- Opção típica: `central`
- Nota: as opções podem variar conforme o hub.

### `Tipo de dispositivo` (Iniciante) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Retorna o tipo de dispositivo conectado à porta.

- Tipo: bloco repórter
- Uso típico: detectar o dispositivo antes de executar lógica específica

### `Acelerômetro do dispositivo` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Retorna valores brutos do acelerômetro.

- Eixos: `x`, `y`, `z`

### `Aceleração do dispositivo` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Retorna dados de aceleração.

- Eixos: `x`, `y`, `z`

## Sensores de orientação e inclinação

### `Inclinação do dispositivo` (Avançado) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Retorna dados de inclinação do telefone/tablet executando MOCPilot.

- Opções de eixo: `pitch`, `roll`

### `Inclinação` (Iniciante) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Retorna o ângulo de inclinação.

- Eixos: `inclinação`, `rotação`, `guinada`
- Nota: `guinada` depende do hub.

### `Obter orientação` (Iniciante) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Retorna o estado atual de orientação do hub.

- Formato: `texto`, `índice`
- Valores: `Frente`, `Topo`, `Direita`, `Traseira`, `Fundo`, `Esquerda`

### `Orientação é para cima` (Iniciante) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Verifica se a orientação corresponde à posição selecionada.

- Opções: `Frente`, `Topo`, `Direita`, `Traseira`, `Fundo`, `Esquerda`

### `Definir orientação de inclinação` (Avançado) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Define a referência de orientação.

- Opções: `Frente`, `Topo`, `Direita`, `Traseira`, `Fundo`, `Esquerda`

## Sensores de tempo e movimento

### `Temporizador` (Avançado) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Retorna o valor do tempo em segundos.

### `Resetar temporizador` (Avançado) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Reinicia o temporizador.

## Sensores de porta

### `Sensor de distância Technic` (Iniciante) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Retorna a distância medida.

- Unidades: `mm`, `cm`, `polegadas`, `%`

### `Technic quando distância é` (Iniciante) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Verifica condição de distância.

- Comparação: `mais perto que`, `mais longe que`, `exatamente em`
- Unidades: `mm`, `cm`, `polegadas`, `%`

### `Technic definir modo do sensor de cor` (Avançado) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Este bloco define o sensor de cor Technic para o modo selecionado.

- Nota: Alterar o modo do sensor de cor pode afetar seu programa de maneiras inesperadas. Por exemplo, o sensor de cor Technic não consegue ler cores ou luz refletida quando está no modo `"ambiente"`.

### `Valor do sensor de cor Technic` (Iniciante) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Retorna a cor detectada.

- Saída: `valor`, `cadeia`

### `Technic quando cor é` (Iniciante) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Verifica correspondência de cor.

### `Luz refletida Technic` (Iniciante) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Retorna intensidade da luz refletida.

### `Technic quando luz refletida é` (Iniciante) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Verifica condição de luz refletida.

- Comparação: `<`, `=`, `>`

### `Luz ambiente Technic` (Iniciante) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Retorna intensidade da luz ambiente.

### `Technic quando luz ambiente é` (Iniciante) {#block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg" />
Verifica condição de luz ambiente.

- Comparação: `<`, `=`, `>`

### `Cor bruta Technic` (Iniciante) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Retorna valor bruto de cor.

- Canais: `vermelho`, `verde`, `azul`

### `Sensor de distância BOOST` (Iniciante) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Retorna a distância do sensor BOOST.

### `BOOST quando distância é` (Iniciante) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Verifica condição de distância BOOST.

### `Sensor de cor BOOST` (Iniciante) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Retorna cor detectada.

### `BOOST é cor` (Iniciante) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Verifica se a cor corresponde.

### `Luz refletida BOOST` (Iniciante) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Retorna valor de luz refletida.

### `BOOST quando luz refletida é` (Iniciante) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Verifica condição de luz refletida.

### `Technic Move definir modo de potência` (Iniciante) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Define o modo de potência.

- Opções: `normal`, `impulso`

### `Tensão de saída BuWizz` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Retorna a tensão de saída atual relatada por um hub BuWizz.

- Disponível apenas para hubs BuWizz suportados.

### `Corrente da porta BuWizz` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Retorna o consumo de corrente relatado para a porta selecionada do hub BuWizz.

- Disponível apenas para hubs e portas BuWizz suportados.

### `WeDo 2 distância` (Iniciante) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Retorna a distância do sensor WeDo 2.

### `WeDo 2 quando distância é` (Iniciante) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Aciona/verifica uma condição de distância para um sensor de distância WeDo 2.

- Opções de comparação: `closer than`, `farther than`, `exactly at`
- Opções de unidade: `%`, `cm`, `inch`

### `WeDo 2 inclinação` (Iniciante) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Retorna o valor de inclinação.

- Eixos: `inclinação`, `rotação`
