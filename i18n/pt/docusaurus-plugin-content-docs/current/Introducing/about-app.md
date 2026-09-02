---
id: AboutApp
title: Sobre o MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Construa. Dirija. Controle tudo.

**MOCPilot** — um app para criar perfis de controle personalizados para LEGO® e criações compatíveis com Bluetooth.

Ele oferece aos construtores um só lugar para conectar hubs, controlar motores, ler sensores, criar painéis e montar programas visuais para modelos, mecanismos, carros, caminhões, trens, robôs e MOCs personalizados.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="App MOCPilot em um telefone" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>O que o MOCPilot oferece</h2>
    <ul>
      <li>Perfis personalizados para seus próprios modelos.</li>
      <li>Perfis prontos para conjuntos oficiais suportados.</li>
      <li>Conexão e gerenciamento de hubs Bluetooth.</li>
      <li>Programação visual com blocos para automação e lógica.</li>
      <li>Controles de painel para dirigir e operar modelos.</li>
      <li>Suporte para LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motores, sensores e dispositivos Bluetooth compatíveis.</li>
    </ul>
  </div>
</div>

## A ideia

A maioria das construções motorizadas precisa de mais do que um controle remoto simples. Um carro pode precisar de direção, aceleração, luzes, monitoramento de bateria, sequência de câmbio ou rotina especial de inicialização. Um robô pode precisar de sensores, eventos, lógica condicional e vários hubs trabalhando juntos.

O MOCPilot foi criado para o espaço entre um controle remoto básico e um ambiente completo de programação. Você pode começar dirigindo um modelo por um painel na tela e depois adicionar lógica, sensores e automação quando a construção ficar mais avançada.

## Perfis

Um **perfil** é o centro de controle de um modelo.

Dentro de um perfil, você escolhe quais hubs pertencem ao modelo, cria o programa que executa o modelo e projeta o painel usado para controlá-lo.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="Página de perfis do MOCPilot" width="420" />

<details>
<summary>Perfis prontos</summary>

Perfis prontos são exemplos já montados para conjuntos oficiais suportados. Eles são úteis para começar rapidamente ou estudar como um perfil funcional é montado.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Perfis prontos do MOCPilot" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Programa de blocos pronto do MOCPilot" width="1100" />

</details>

<details>
<summary>Perfis personalizados</summary>

Perfis personalizados são para seus próprios MOCs e experimentos. Você pode criar um perfil, adicionar hubs, conectar motores e sensores, montar um programa e criar um painel de controle que combine com o modelo exato.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Criar um perfil personalizado do MOCPilot" width="420" />

</details>

## Conectar hubs e dispositivos

O MOCPilot pode se conectar a hubs Bluetooth suportados e dispositivos compatíveis, deixando-os disponíveis dentro do seu perfil.

Você pode usar um perfil com um hub para uma construção simples ou conectar vários hubs quando o modelo precisa de mais portas, sistemas de energia separados ou módulos independentes.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Página Meus hubs Bluetooth no MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Hubs Bluetooth conectados no MOCPilot" width="1100" />

<details>
<summary>Exemplos de hardware suportado</summary>

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(140px, 1fr))', gap: '16px', alignItems: 'end', margin: '16px 0'}}>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_hub_p.webp')} alt="LEGO Technic Hub" style={{maxWidth: '130px'}} />
    <div><strong>Technic Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_move_hub_p.webp')} alt="LEGO Technic Move Hub" style={{maxWidth: '130px'}} />
    <div><strong>Technic Move Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/buwizz3_hub_p.webp')} alt="BuWizz 3.0 Pro Hub" style={{maxWidth: '130px'}} />
    <div><strong>BuWizz 3.0</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/sbrick_hub_p.webp')} alt="SBrick Hub" style={{maxWidth: '130px'}} />
    <div><strong>SBrick</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/mould_king_4_p.webp')} alt="Mould King Hub" style={{maxWidth: '130px'}} />
    <div><strong>Mould King</strong></div>
  </div>
</div>

Veja a página de [hubs, motores e sensores suportados](/docs/Introducing/SupportedDevices/) para a lista completa.

</details>

## Criar lógica com blocos

O MOCPilot inclui um construtor visual de blocos. Você pode criar programas conectando blocos em vez de escrever código.

Os blocos podem reagir a eventos, controlar motores, ler sensores, trabalhar com variáveis, usar entrada de gamepad, atualizar controles do painel e coordenar várias ações.

O MOCPilot oferece suporte completo a gamepads físicos conectados. Os blocos de gamepad permitem ler botões, gatilhos, direções do D-pad e analógicos, para mapear um controle real ao modelo quando controles físicos forem melhores que a tela sensível ao toque.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="Programa de usuário do MOCPilot criado com blocos" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Bloco quando o programa inicia" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Bloco iniciar motor em velocidade" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Bloco nível da bateria do hub" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Bloco valor do volante" />
</div>

<details>
<summary>O que você pode fazer com programas de blocos</summary>

- Iniciar, parar e direcionar motores.
- Ler nível da bateria, tensão, inclinação, orientação, temperatura e valores de sensores.
- Configurar controles de gamepad físico para direção, aceleração, gatilhos, ações e troca de modo.
- Reagir quando botões, sensores, temporizadores ou controles do painel mudam.
- Criar verificações de inicialização antes que o modelo comece a se mover.
- Adicionar lógica personalizada para luzes, calibração de direção, modos de potência e configuração de hub.
- Usar variáveis, listas, condições, loops, broadcasts e blocos personalizados para organizar comportamentos complexos.

</details>

## Criar um painel de condução

O painel é a tela usada ao controlar o modelo. Ele pode incluir volantes, joysticks, controles deslizantes, botões, interruptores, pedais, monitores e outros controladores.

Você pode conectar controles do painel e entradas de gamepad físico a blocos e ações do hub, para que a interface combine com o modelo.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="Controles de painel do MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="Tela de controle do MOCPilot com volante e pedais" width="1100" />

<details>
<summary>Exemplos de painel</summary>

- Use volante e pedais para carros.
- Use controles deslizantes para guindastes, elevadores e atuadores lineares.
- Use botões para luzes, buzina, trocas de marcha ou ações com script.
- Use monitores para mostrar bateria, velocidade, valores de sensores ou estado personalizado do programa.
- Use um gamepad conectado quando preferir botões, analógicos e gatilhos físicos aos controles de toque.

</details>

## Manter construções avançadas gerenciáveis

Conforme um modelo cresce, o perfil pode crescer com ele. O MOCPilot oferece lógica reutilizável com **My Blocks**, configuração de hubs específica do perfil, vários controladores e fluxos que combinam controle manual com automação.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Exemplo de uso de My Blocks no MOCPilot" width="1100" />

Isso ajuda a manter programas grandes legíveis. Por exemplo, um perfil pode ter um bloco personalizado para atualizar a bateria, outro para calibrar a direção e outro para um modo especial de condução.

## Fluxo típico

1. Crie ou abra um perfil.
2. Adicione os hubs Bluetooth e dispositivos usados pelo modelo.
3. Monte o programa com blocos.
4. Crie um painel para condução e interação.
5. Pressione **Play**.
6. Teste, ajuste e melhore o perfil até o modelo se comportar como você deseja.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Fluxo de conexão de hub no MOCPilot" width="1100" />

## Para quem é o MOCPilot

O MOCPilot é útil para construtores que querem:

- Um controle remoto melhor para modelos LEGO® motorizados.
- Uma forma de controlar hubs Bluetooth compatíveis de terceiros.
- Um ambiente de programação visual para mecanismos e robôs.
- Perfis prontos para conjuntos oficiais suportados.
- Painéis personalizados para carros, caminhões, trens, crawlers, guindastes e outros MOCs.
- Um único app que combina hubs, motores, sensores, gamepads e controles na tela.

## Comece a explorar

- Siga o [tutorial de início rápido](/docs/Introducing/QuickStart/) para criar seu primeiro perfil.
- Verifique os [dispositivos suportados](/docs/Introducing/SupportedDevices/) antes de escolher hardware.
- Explore a [documentação do BlockBuilder](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/) quando estiver pronto para adicionar lógica.
- Veja [atualização de firmware do hub](/docs/Application/Hubs/FirmwareUpdating/) se um hub exigir uma versão de firmware suportada.
