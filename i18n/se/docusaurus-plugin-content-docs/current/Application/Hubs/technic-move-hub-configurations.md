---
id: TechnicMoveHubConfigurations
title: Technic Move Hub-konfigurationer
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Technic Move Hub-konfigurationer

## Översikt

Technic Move Hub introducerade en unik funktion i LEGO Powered Up-hubbfamiljen: hubben kan ändra sitt beteende beroende på den konfiguration som är aktiv.

MOCPilot låter dig ändra Technic Move Hub-konfigurationen så att hubbens beteende matchar det officiella LEGO-set du vill styra.

## Konfigurationer som stöds

För närvarande är dessa Technic Move Hub-konfigurationer kända:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Konfigurationsalternativ för Technic Move Hub" />

## Ändra konfiguration från Mina Bluetooth-hubbar

Du kan ändra konfigurationen från sidan **Mina Bluetooth-hubbar**:

1. Öppna **Mina Bluetooth-hubbar**.
2. Hitta Technic Move Hub.
3. Öppna hubbens snabbmeny.
4. Välj **Välj konfiguration**.
5. Välj den konfiguration som behövs.
6. Bekräfta dialogrutan för omkonfigurering.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Snabbmeny för Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Konfigurationsundermeny för Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Bekräftelsedialog för omkonfigurering av Technic Move Hub" />

:::warning Viktigt
När hubbkonfigurationen ändras flashas ett underprogram till hubben, och processen liknar en firmwareuppdatering.

Håll hubben påslagen under hela processen. Håll telefon, surfplatta eller dator påslagen och nära hubben så att Bluetooth-anslutningen förblir stabil. Stäng inte MOCPilot, stäng inte av Bluetooth och stäng inte av hubben medan konfigurationen ändras.

Om konfigurationsändringen avbryts kan hubbens firmware skadas. Då kan firmwareåterställning krävas innan hubben kan användas igen. Följ guiden för [återställning av hubbfirmware](/docs/Application/Hubs/RecoveryHubFirmware/) om återställning krävs.
:::

Under omkonfigureringen svarar hubben inte på normala kommandon. LED-lampan blinkar med en stegvis färgindikering tills processen är klar. När den nya konfigurationen har tillämpats initieras hubben om.

## Konfigurationsblock

MOCPilot innehåller också block för att läsa och ändra Technic Move Hub-konfigurationen under ett program.

### Ställ in hubbkonfiguration

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Blocket Ställ in hubbkonfiguration" />

Blocket **Ställ in hubbkonfiguration** ändrar den valda hubben till en av dess konfigurationsprofiler som stöds.

- Hubbväljare: väljer hubben som ska omkonfigureras.
- Konfigurationsväljare: väljer målkonfigurationen.
- Tillgängliga konfigurationer för Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** och **Batmobile™ Tumbler**.

Se [dokumentationen för blocket Ställ in hubbkonfiguration](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Hubbkonfiguration

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Blocket Hubbkonfiguration" />

Blocket **Hubbkonfiguration** rapporterar den aktuella konfigurationen för den valda hubben.

- Hubbväljare: väljer hubben som ska läsas.
- Utdataformat: **textvärde** returnerar konfigurationsnamnet.
- Utdataformat: **index** returnerar konfigurationens index, vilket är användbart för jämförelser i villkor.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Utdataformatalternativ för blocket Hubbkonfiguration" />

Se [dokumentationen för blocket Hubbkonfiguration](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Strömpuls

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Blocket Strömpuls" />

Blocket **Strömpuls** skickar ett effektpulskommando till den valda Technic Move Hub. Detta block fungerar endast när Technic Move Hub är konfigurerad som **Batmobile™ Tumbler**.

När det körs startar hubben motorerna med maximal tillgänglig effekt och hastighet under en kort stund, vanligtvis cirka 1-2 sekunder.

Se [dokumentationen för blocket Strömpuls](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Ändra konfiguration medan programmet körs

Det är också möjligt att ändra Technic Move Hub-konfigurationen medan ett program körs.

Det vanliga tillvägagångssättet är:

1. Läs den aktuella hubbkonfigurationen.
2. Jämför den med konfigurationen som profilen kräver.
3. Om konfigurationen skiljer sig, ange den krävda konfigurationen.
4. Läs konfigurationen igen efter omkonfigureringen.
5. Fortsätt bara när hubben rapporterar den förväntade konfigurationen.
6. Koppla från eller stoppa programmet om den krävda konfigurationen inte användes.

Den förbyggda profil som använder denna hubb kan användas som referens för detta tillvägagångssätt.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Blockexempel som visar ändring av Technic Move Hub-konfiguration medan programmet körs" />
