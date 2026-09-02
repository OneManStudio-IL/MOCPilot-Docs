---
id: Control
title: Controle
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Controle

Os blocos de controle gerenciam o fluxo de execução: espera, loops, ramificações e parada de scripts.

## Blocos de espera

### `Esperar` (Iniciante) {#block_control_wait_for}

<img src={useBaseUrl('/img/blocks/block_control_wait_for.svg')} alt="block_control_wait_for.svg" />

Pausa o script atual por um tempo especificado.

### `Esperar até` (Avançado) {#block_control_wait_until}

<img src={useBaseUrl('/img/blocks/block_control_wait_until.svg')} alt="block_control_wait_until.svg" />

Pausa o script atual até que uma condição se torne verdadeira.

## Blocos de loop

### `Repetir` (Avançado) {#block_control_repeat_for}

<img src={useBaseUrl('/img/blocks/block_control_repeat_for.svg')} alt="block_control_repeat_for.svg" />

Executa os blocos aninhados um número fixo de vezes.

### `Repetir até` (Avançado) {#block_control_repeat_until}

<img src={useBaseUrl('/img/blocks/block_control_repeat_until.svg')} alt="block_control_repeat_until.svg" />

Executa os blocos aninhados repetidamente até que uma condição se torne verdadeira.

### `Para sempre` (Avançado) {#block_control_repeat_forever}

<img src={useBaseUrl('/img/blocks/block_control_repeat_forever.svg')} alt="block_control_repeat_forever.svg" />

Executa os blocos aninhados continuamente até que o programa ou script seja interrompido.

## Blocos de ramificação

### `Se` (Iniciante) {#block_control_if}

<img src={useBaseUrl('/img/blocks/block_control_if.svg')} alt="block_control_if.svg" />

Executa os blocos aninhados apenas quando a condição for verdadeira.

### `Se / Senão` (Avançado) {#block_control_if_else}

<img src={useBaseUrl('/img/blocks/block_control_if_else.svg')} alt="block_control_if_else.svg" />

Executa um ramo quando a condição for verdadeira, caso contrário executa o ramo alternativo.

### `Fazer isto e isto` (Guru) {#block_control_do_this_and_this}

<img src={useBaseUrl('/img/blocks/block_control_do_this_and_this.svg')} alt="block_control_do_this_and_this.svg" />

Executa duas pilhas de blocos em sequência como parte de uma única operação de fluxo de controle.

## Blocos de parada

### `Parar` (Iniciante) {#block_control_stop}

<img src={useBaseUrl('/img/blocks/block_control_stop.svg')} alt="block_control_stop.svg" />

Interrompe a execução do script (o escopo depende da opção de parada selecionada).

- Opções de parada: `tudo`, `esta pilha`, `e sair do programa`

### `Parar outras pilhas` (Guru) {#block_control_stop_other_stacks}

<img src={useBaseUrl('/img/blocks/block_control_stop_other_stacks.svg')} alt="block_control_stop_other_stacks.svg" />

Interrompe todas as outras pilhas em execução, permitindo que a pilha atual continue.

## Blocos utilitários de hub/controle

### `Definir conexão` (Iniciante) {#block_hubs_control_set_connect}

<img src={useBaseUrl('/img/blocks/block_hubs_control_set_connect.svg')} alt="block_hubs_control_set_connect.svg" />

Controla o estado de conexão do hub a partir da lógica de fluxo de controle.

- Opções de ação: `conectar`, `desconectar`

### `Definir configuração do hub` (Avançado) {#block_hubs_set_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="block_hubs_set_hub_config.svg" />
Define o hub selecionado para um dos seus perfis de configuração suportados.

- Disponível apenas para hubs que expõem opções de configuração.
- Uso típico: alternar um hub configurável, como Technic Move Hub, para outra configuração salva antes de executar os próximos blocos.

### `Configuração do hub` (Avançado) {#block_hubs_all_control_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="block_hubs_all_control_hub_config.svg" />
Retorna a configuração atual do hub selecionado.

- Tipo: bloco repórter
- Opções de formato de saída: `text`, `index`
- Disponível apenas para hubs que expõem opções de configuração.
- Retorna `NaN` quando o hub selecionado não está conectado ou nenhuma configuração está disponível.

### `Está conectado` (Iniciante) {#block_hubs_all_sensors_is_connected}

<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_connected.svg')} alt="block_hubs_all_sensors_is_connected.svg" />

Retorna se o hub está atualmente conectado.

- Tipo: bloco repórter booleano

### `BuWizz 2 definir modo de potência` (Iniciante) {#block_hubs_buwizz_sensors_set_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_set_power_mode.svg')} alt="block_hubs_buwizz_sensors_set_power_mode.svg" />

Define o modo de potência do hub BuWizz 2.

- Opções de modo: `Slow`, `Normal`, `Fast`, `Ludicrous`

### `BuWizz 2 obter modo de potência` (Guru) {#block_hubs_buwizz_sensors_get_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_power_mode.svg')} alt="block_hubs_buwizz_sensors_get_power_mode.svg" />

Retorna o modo de potência atualmente ativo do BuWizz 2.

- Opções de formato de saída: `texto`, `índice`

### `MouldKing definir canal de controle` (Avançado) {#block_hubs_mouldking_control_set_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_set_control_channel.svg')} alt="block_hubs_mouldking_control_set_control_channel.svg" />

Define o canal de controle ativo para o hub/controlador MouldKing suportado.

- Opções de canal: `A`, `B`, `C`

### `MouldKing obter canal de controle` (Avançado) {#block_hubs_mouldking_control_get_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_get_control_channel.svg')} alt="block_hubs_mouldking_control_get_control_channel.svg" />

Retorna o canal de controle ativo atual para o hub/controlador MouldKing suportado.

- Opções de formato de saída: `texto`, `índice`