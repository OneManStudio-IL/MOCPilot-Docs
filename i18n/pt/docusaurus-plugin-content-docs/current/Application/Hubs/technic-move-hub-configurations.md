---
id: TechnicMoveHubConfigurations
title: Configurações do Technic Move Hub
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Configurações do Technic Move Hub

## Visão geral

Technic Move Hub introduziu um recurso único na família de hubs LEGO Powered Up: o hub pode mudar seu comportamento dependendo da configuração aplicada atualmente.

MOCPilot permite alterar a configuração do Technic Move Hub para que o comportamento do hub corresponda ao conjunto LEGO oficial que você deseja controlar.

## Configurações suportadas

No momento, estas configurações do Technic Move Hub são conhecidas:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Opções de configuração do Technic Move Hub" />

## Alterar a configuração em Meus hubs Bluetooth

Você pode alterar a configuração na página **Meus hubs Bluetooth**:

1. Abra **Meus hubs Bluetooth**.
2. Encontre o Technic Move Hub.
3. Abra o menu de contexto do hub.
4. Selecione **Selecionar configuração**.
5. Escolha a configuração necessária.
6. Confirme a caixa de diálogo de reconfiguração.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Menu de contexto do Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Submenu de configuração do Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Caixa de confirmação de reconfiguração do Technic Move Hub" />

:::warning Importante
Alterar a configuração do hub grava um subprograma no hub e é semelhante a um processo de atualização de firmware.

Mantenha o hub ligado durante todo o processo. Mantenha o telefone, tablet ou computador ligado e próximo do hub para que a conexão Bluetooth permaneça estável. Não feche o MOCPilot, não desligue o Bluetooth e não desligue o hub enquanto a configuração estiver sendo alterada.

Interromper a alteração da configuração pode danificar o firmware do hub. Se isso acontecer, pode ser necessário recuperar o firmware antes de usar o hub novamente. Siga o guia de [recuperação do firmware do hub](/docs/Application/Hubs/RecoveryHubFirmware/) se a recuperação for necessária.
:::

Durante a reconfiguração, o hub não responde a comandos normais. O LED pisca com uma indicação colorida em etapas até o processo terminar. Depois que a nova configuração é aplicada, o hub é reinicializado.

## Blocos de configuração

MOCPilot também inclui blocos para ler e alterar a configuração do Technic Move Hub durante um programa.

### Definir configuração do hub

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Bloco Definir configuração do hub" />

O bloco **Definir configuração do hub** altera o hub selecionado para um de seus perfis de configuração compatíveis.

- Seletor de hub: escolhe o hub a ser reconfigurado.
- Seletor de configuração: escolhe a configuração de destino.
- Configurações disponíveis para Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** e **Batmobile™ Tumbler**.

Consulte a [documentação do bloco Definir configuração do hub](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Configuração do hub

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Bloco Configuração do hub" />

O bloco **Configuração do hub** informa a configuração atual do hub selecionado.

- Seletor de hub: escolhe o hub a ser lido.
- Formato de saída: **texto** retorna o nome da configuração.
- Formato de saída: **índice** retorna o índice da configuração, útil para comparações em condições.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Opções de formato de saída do bloco Configuração do hub" />

Consulte a [documentação do bloco Configuração do hub](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Pulso de potência

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Bloco Pulso de potência" />

O bloco **Pulso de potência** envia um comando de pulso de potência ao Technic Move Hub selecionado. Este bloco funciona somente quando o Technic Move Hub está configurado como **Batmobile™ Tumbler**.

Quando executado, o hub liga os motores com a potência e velocidade máximas disponíveis por um curto período, geralmente cerca de 1-2 segundos.

Consulte a [documentação do bloco Pulso de potência](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Alterar a configuração durante a execução do programa

Também é possível alterar a configuração do Technic Move Hub enquanto um programa está em execução.

A abordagem comum é:

1. Leia a configuração atual do hub.
2. Compare-a com a configuração exigida pelo perfil.
3. Se a configuração for diferente, aplique a configuração exigida.
4. Leia a configuração novamente após a reconfiguração.
5. Continue somente quando o hub informar a configuração esperada.
6. Desconecte ou pare o programa se a configuração exigida não foi aplicada.

O perfil predefinido que usa este hub pode ser usado como referência para esta abordagem.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Exemplo de blocos mostrando a alteração da configuração do Technic Move Hub durante a execução" />
