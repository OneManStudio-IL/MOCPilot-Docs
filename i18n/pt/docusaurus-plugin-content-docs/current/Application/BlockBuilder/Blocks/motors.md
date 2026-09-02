---
id: Motors
title: Motores
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Motores

Os blocos de motor são usados para iniciar, parar, posicionar e ajustar motores conectados às portas do hub.

## Blocos principais de comando de motor

### `Iniciar motor` (Iniciante) {#block_hubs_all_motors_port_start_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor.svg')} alt="block_hubs_all_motors_port_start_motor.svg" />
Inicia o motor selecionado.

- Opções de direção: horário / anti-horário

### `Parar motor` (Iniciante) {#block_hubs_all_motors_port_stop_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_stop_motor.svg')} alt="block_hubs_all_motors_port_stop_motor.svg" />
Para o motor selecionado.

### `Executar por` (Avançado) {#block_hubs_all_motors_port_run_for}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for.svg')} alt="block_hubs_all_motors_port_run_for.svg" />
Executa o motor selecionado por um tempo/ângulo/rotação especificado com base nas configurações do bloco.

- Opções de direção: horário / anti-horário
- Opções de unidade: `rotações`, `graus`, `segundos`
- Nota: este recurso requer um motor com suporte a encoder na porta selecionada.

### `Iniciar motor com velocidade` (Iniciante) {#block_hubs_all_motors_port_start_motor_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="block_hubs_all_motors_port_start_motor_at_speed.svg" />
Inicia o motor com um valor de velocidade definido.

### `Executar por com velocidade` (Avançado) {#block_hubs_all_motors_port_run_for_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for_at_speed.svg')} alt="block_hubs_all_motors_port_run_for_at_speed.svg" />
Executa o motor por uma duração/quantidade alvo com velocidade definida.

- Opções de unidade: `rotações`, `graus`, `segundos`
- Nota: este recurso requer um motor com suporte a encoder na porta selecionada.

### `Definir velocidade do motor` (Avançado) {#block_hubs_all_motors_port_set_motor_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_speed.svg')} alt="block_hubs_all_motors_port_set_motor_speed.svg" />
Define a velocidade usada por outros blocos de execução do motor.

## Blocos de posição e movimento

### `Ir para posição` (Avançado) {#block_hubs_all_motors_port_go_to_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_position.svg')} alt="block_hubs_all_motors_port_go_to_position.svg" />
Move o motor para uma posição absoluta alvo.

- Opções de trajeto: `caminho mais curto`, `horário`, `anti-horário`
- Nota: requer motor com suporte a encoder.

### `Ir para posição relativa` (Iniciante) {#block_hubs_all_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_relative_position.svg')} alt="block_hubs_all_motors_port_go_to_relative_position.svg" />
Move o motor por um deslocamento relativo.

- Nota: requer motor com suporte a encoder.

### `BuWizz 3 ir para posição relativa` (Iniciante) {#block_hubs_buwizz3_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_motors_port_go_to_relative_position.svg')} alt="block_hubs_buwizz3_motors_port_go_to_relative_position.svg" />
Variante BuWizz 3 do bloco de posição relativa.

- Nota: requer motor com suporte a encoder.

### `Definir posição relativa` (Iniciante) {#block_hubs_all_motors_port_set_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_relative_position.svg')} alt="block_hubs_all_motors_port_set_relative_position.svg" />
Define a referência de posição relativa do motor.

- Nota: requer motor com suporte a encoder.

### `Calibrar direção` (Iniciante) {#block_hubs_all_motors_port_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_calibrate_steering_rack.svg')} alt="block_hubs_all_motors_port_calibrate_steering_rack.svg" />
Calibra a posição neutra/de referência da direção.

- Requisito: o motor deve suportar rastreamento de ângulo (encoder interno).
- Requisito mecânico: o movimento deve ser limitado fisicamente.
- Como funciona: mede o alcance de rotação e calcula dados de calibração.
- Comportamento de saída: escreve resultados nas variáveis passadas ao bloco.

## Blocos de ajuste e segurança do motor

### `Definir comportamento do motor ao parar` (Guru) {#block_hubs_all_motors_port_set_motor_to_at_stop}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_to_at_stop.svg')} alt="block_hubs_all_motors_port_set_motor_to_at_stop.svg" />
Define o modo de parada do motor.

- Opções: `freio`, `manter posição`, `livre`
- Nota: requer motor com suporte a encoder.

### `Definir detecção de travamento` (Guru) {#block_hubs_all_motors_port_set_motors_stall_detection}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motors_stall_detection.svg')} alt="block_hubs_all_motors_port_set_motors_stall_detection.svg" />
Ativa ou desativa a detecção de travamento.

- Nota: disponível apenas para MINDSTORMS Robot Inventor.

### `Definir aceleração` (Guru) {#block_hubs_all_motors_port_set_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_acceleration.svg')} alt="block_hubs_all_motors_port_set_acceleration.svg" />
Define o perfil/taxa de aceleração do motor.

- Opções: `padrão`, `rápido`, `equilibrado`, `suave`, `lento`, `muito lento`
- Nota: requer motor com suporte a encoder.

### `Definir desaceleração` (Guru) {#block_hubs_all_motors_port_set_deceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_deceleration.svg')} alt="block_hubs_all_motors_port_set_deceleration.svg" />
Define o perfil/taxa de desaceleração do motor.

- Opções: `padrão`, `rápido`, `equilibrado`, `suave`, `lento`, `muito lento`
- Nota: requer motor com suporte a encoder.

## Blocos repórter de motor

### `Posição` (Iniciante) {#block_hubs_all_motors_port_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_position.svg')} alt="block_hubs_all_motors_port_position.svg" />
Retorna a posição atual do motor.

### `Posição relativa` (Iniciante) {#block_hubs_all_motors_port_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_relative_position.svg')} alt="block_hubs_all_motors_port_relative_position.svg" />
Retorna o valor atual da posição relativa.

### `Velocidade` (Iniciante) {#block_hubs_all_motors_port_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_speed.svg')} alt="block_hubs_all_motors_port_speed.svg" />
Retorna a velocidade atual do motor.

### `Potência` (Avançado) {#block_hubs_all_motors_port_power}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_power.svg')} alt="block_hubs_all_motors_port_power.svg" />
Retorna o valor atual de potência do motor.

- Nota: disponível apenas para MINDSTORMS Robot Inventor.

## Blocos de motor Technic Move

### `Iniciar motores com velocidade` (Iniciante) {#block_hubs_technicmove_motors_start_motors_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_start_motors_at_speed.svg')} alt="block_hubs_technicmove_motors_start_motors_at_speed.svg" />
Inicia os motores de tração Technic Move com a velocidade selecionada.

### `Pulso de potência` (Iniciante) {#block_hubs_technicmove_motors_power_pulse}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="block_hubs_technicmove_motors_power_pulse.svg" />
Envia um comando de pulso de potência para o Technic Move Hub selecionado.

- Disponível apenas para Technic Move Hub.
- Uso típico: reforçar brevemente ou acordar o sistema de tração Technic Move antes de continuar com os próximos blocos.

### `Parar motores` (Iniciante) {#block_hubs_technicmove_motors_stop_motors}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_stop_motors.svg')} alt="block_hubs_technicmove_motors_stop_motors.svg" />
Para os motores de tração Technic Move.

### `Frear` (Iniciante) {#block_hubs_technicmove_motors_brake}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_brake.svg')} alt="block_hubs_technicmove_motors_brake.svg" />
Aplica comportamento de freio aos motores.

- Opções: `desligado`, `ligado`

### `Definir direção para` (Iniciante) {#block_hubs_technicmove_motors_set_steering_rack_to}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_set_steering_rack_to.svg')} alt="block_hubs_technicmove_motors_set_steering_rack_to.svg" />
Define a posição/valor alvo da direção.

### `Calibrar direção` (Iniciante) {#block_hubs_technicmove_motors_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_calibrate_steering_rack.svg')} alt="block_hubs_technicmove_motors_calibrate_steering_rack.svg" />
Calibra a direção usando algoritmo interno do hub e detecção automática do alcance.

- Nota: o eixo do motor deve ser limitado mecanicamente.
