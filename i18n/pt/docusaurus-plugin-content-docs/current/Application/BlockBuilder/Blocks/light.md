---
id: Light
title: Luz
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Luz

Esta página documenta os blocos da categoria Luz usados para controlar LEDs e saídas de luz em hubs compatíveis.

## Blocos de luz comuns

### `Definir cor do LED` (Iniciante) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Define a cor do LED do hub usando opções de cores predefinidas.

- Tipo: bloco de comando
- Uso típico: indicar estado (pronto, em execução, aviso, erro)

### `Definir intensidade da luz` (Iniciante) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Define a saída de luz selecionada para um valor/intensidade desejado.

- Tipo: bloco de comando
- Uso típico: brilho de faróis, intensidade de status

### `Desligar luz` (Iniciante) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Desliga a saída de luz selecionada.

- Tipo: bloco de comando
- Uso típico: sequência de desligamento, economia de bateria

### `Technic Move definir intensidade da luz` (Iniciante) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variante de `Definir intensidade da luz` para o hub/luz Technic Move.

- Tipo: bloco de comando
- Uso típico: definir nível de saída de luz do hub Move

## Blocos da matriz LED interna

### `Ligar matriz de luz` (Avançado) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Mostra a imagem selecionada na matriz LED interna do hub e continua imediatamente para o próximo bloco na pilha. A imagem permanece no display até que outro bloco altere a matriz LED interna ou o programa pare.

- Tipo: bloco de comando
- Nota: o hub selecionado deve ter uma matriz LED interna.

### `Escrever na matriz de luz` (Iniciante) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Mostra uma sequência de texto na matriz LED interna do hub rolando uma letra de cada vez.

- Tipo: bloco de comando
- Nota: o hub selecionado deve ter uma matriz LED interna.

### `Desligar pixels da matriz` (Iniciante) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Desliga todas as luzes da matriz LED interna do hub.

- Tipo: bloco de comando
- Nota: o hub selecionado deve ter uma matriz LED interna.

### `Definir pixel da matriz` (Avançado) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Define o brilho de um pixel na matriz LED interna do hub. Apenas o pixel selecionado é atualizado; o restante do display permanece inalterado. Os campos de posição do pixel usam valores de coluna e linha, com o pixel `1, 1` no canto superior esquerdo.

- Tipo: bloco de comando
- Nota: o hub selecionado deve ter uma matriz LED interna.

### `Girar orientação da matriz` (Avançado) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Gira a orientação do que é exibido na matriz LED interna do hub no sentido horário ou anti-horário. Cada rotação altera a orientação do display em 90 graus e afeta os blocos de Luz executados depois dela.

- Tipo: bloco de comando
- Nota: o hub selecionado deve ter uma matriz LED interna.

### `Definir orientação da matriz` (Avançado) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Define a orientação do que é exibido na matriz LED interna do hub. A orientação padrão é vertical, e a orientação selecionada afeta os blocos de Luz executados depois dela.

- Tipo: bloco de comando
- Opções de orientação: `vertical`, `esquerda`, `direita`, `de cabeça para baixo`
- Nota: o hub selecionado deve ter uma matriz LED interna.

## Blocos de luz do sensor de distância

### `Iluminar sensor de distância` (Iniciante) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Define as luzes no sensor de distância selecionado. O bloco pode ligar ou desligar luzes individuais do sensor e pode usar um bloco repórter de lista para controlar o brilho de cada luz.

- Tipo: bloco de comando
- Nota: disponível apenas para o hub MINDSTORMS Robot Inventor.

## Blocos de luz BuWizz 3

### `BuWizz 3 definir cor do LED` (Iniciante) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Define a cor do LED na porta selecionada do BuWizz 3 usando opções internas.

- Tipo: bloco de comando

### `BuWizz 3 definir cor do LED (texto)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Define a cor do LED do BuWizz 3 usando um valor de texto.

- Tipo: bloco de comando
- Uso típico: cores dinâmicas vindas de variáveis

### `BuWizz 3 definir cor do LED (RGB)` (Avançado) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Define a cor do LED do BuWizz 3 usando canais RGB explícitos.

- Tipo: bloco de comando
- Uso típico: controle completo de cores personalizadas e gradientes
