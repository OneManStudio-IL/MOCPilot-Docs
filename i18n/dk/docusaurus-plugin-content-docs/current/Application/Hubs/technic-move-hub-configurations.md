---
id: TechnicMoveHubConfigurations
title: Technic Move Hub-konfigurationer
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Technic Move Hub-konfigurationer

## Oversigt

Technic Move Hub introducerede en unik funktion i LEGO Powered Up hub-familien: hubben kan ændre adfærd afhængigt af den konfiguration, der aktuelt er anvendt.

MOCPilot lader dig ændre Technic Move Hub-konfigurationen, så hubbens adfærd matcher det officielle LEGO-sæt, du vil styre.

## Understøttede konfigurationer

I øjeblikket kendes disse Technic Move Hub-konfigurationer:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Konfigurationsmuligheder for Technic Move Hub" />

## Skift konfiguration fra Mine Bluetooth-hubs

Du kan ændre konfigurationen fra siden **Mine Bluetooth-hubs**:

1. Åbn **Mine Bluetooth-hubs**.
2. Find Technic Move Hub.
3. Åbn hubbens kontekstmenu.
4. Vælg **Vælg konfiguration**.
5. Vælg den nødvendige konfiguration.
6. Bekræft dialogen for rekonfiguration.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Kontekstmenu for Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Konfigurationsundermenu for Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Bekræftelsesdialog for rekonfiguration af Technic Move Hub" />

:::warning Vigtigt
Når hubkonfigurationen ændres, flashes et underprogram til hubben, og processen minder om en firmwareopdatering.

Hold hubben tændt under hele processen. Hold telefon, tablet eller computer tændt og tæt på hubben, så Bluetooth-forbindelsen forbliver stabil. Luk ikke MOCPilot, slå ikke Bluetooth fra, og sluk ikke hubben, mens konfigurationen ændres.

Hvis konfigurationsændringen afbrydes, kan hubbens firmware blive beskadiget. I så fald kan firmwaregendannelse være nødvendig, før hubben kan bruges igen. Følg guiden til [gendannelse af hubfirmware](/docs/Application/Hubs/RecoveryHubFirmware/), hvis gendannelse er nødvendig.
:::

Under rekonfigurationen reagerer hubben ikke på normale kommandoer. LED’en blinker med en trinvis farveindikation, indtil processen er færdig. Når den nye konfiguration er anvendt, initialiseres hubben igen.

## Konfigurationsblokke

MOCPilot indeholder også blokke til at læse og ændre Technic Move Hub-konfigurationen under et program.

### Indstil hub-konfiguration

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Blokken Indstil hub-konfiguration" />

Blokken **Indstil hub-konfiguration** ændrer den valgte hub til en af dens understøttede konfigurationsprofiler.

- Hubvælger: vælger den hub, der skal rekonfigureres.
- Konfigurationsvælger: vælger målkonfigurationen.
- Tilgængelige konfigurationer for Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** og **Batmobile™ Tumbler**.

Se [dokumentationen for blokken Indstil hub-konfiguration](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Hub-konfiguration

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Blokken Hub-konfiguration" />

Blokken **Hub-konfiguration** rapporterer den aktuelle konfiguration for den valgte hub.

- Hubvælger: vælger den hub, der skal læses.
- Outputformat: **tekst** returnerer konfigurationsnavnet.
- Outputformat: **indeks** returnerer konfigurationsindekset, hvilket er nyttigt til sammenligninger i betingelser.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Outputformatmuligheder for blokken Hub-konfiguration" />

Se [dokumentationen for blokken Hub-konfiguration](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Strømpuls

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Blokken Strømpuls" />

Blokken **Strømpuls** sender en effektpuls-kommando til den valgte Technic Move Hub. Denne blok virker kun, når Technic Move Hub er konfigureret som **Batmobile™ Tumbler**.

Når den kører, starter hubben motorerne med maksimal tilgængelig effekt og hastighed i kort tid, normalt omkring 1-2 sekunder.

Se [dokumentationen for blokken Strømpuls](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Skift konfiguration mens programmet kører

Det er også muligt at ændre Technic Move Hub-konfigurationen, mens et program kører.

Den almindelige fremgangsmåde er:

1. Læs den aktuelle hubkonfiguration.
2. Sammenlign den med den konfiguration, profilen kræver.
3. Hvis konfigurationen er anderledes, skal du indstille den krævede konfiguration.
4. Læs konfigurationen igen efter rekonfigurationen.
5. Fortsæt kun, når hubben rapporterer den forventede konfiguration.
6. Afbryd forbindelsen eller stop programmet, hvis den krævede konfiguration ikke blev anvendt.

Den forudbyggede profil, der bruger denne hub, kan bruges som reference for denne tilgang.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Blokeksempel på ændring af Technic Move Hub-konfiguration under kørsel" />
