---
id: TechnicMoveHubConfigurations
title: Technic Move Hub-configuraties
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Technic Move Hub-configuraties

## Overzicht

Technic Move Hub introduceerde een unieke functie binnen de LEGO Powered Up-hubfamilie: de hub kan zijn gedrag aanpassen op basis van de configuratie die op dat moment is toegepast.

Met MOCPilot kun je de configuratie van Technic Move Hub wijzigen, zodat het gedrag van de hub overeenkomt met de officiële LEGO-set die je wilt bedienen.

## Ondersteunde configuraties

Op dit moment zijn deze Technic Move Hub-configuraties bekend:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Configuratieopties van Technic Move Hub" />

## Configuratie wijzigen vanuit Mijn Bluetooth-hubs

Je kunt de configuratie wijzigen vanaf de pagina **Mijn Bluetooth-hubs**:

1. Open **Mijn Bluetooth-hubs**.
2. Zoek de Technic Move Hub.
3. Open het contextmenu van de hub.
4. Selecteer **Configuratie selecteren**.
5. Kies de vereiste configuratie.
6. Bevestig het dialoogvenster voor herconfiguratie.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Contextmenu van Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Configuratiesubmenu van Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Bevestigingsvenster voor herconfiguratie van Technic Move Hub" />

:::warning Belangrijk
Bij het wijzigen van de hubconfiguratie wordt een subprogramma naar de hub geflasht; dit lijkt op een firmware-update.

Houd de hub tijdens het hele proces ingeschakeld. Houd je telefoon, tablet of computer ingeschakeld en dicht bij de hub, zodat de Bluetooth-verbinding stabiel blijft. Sluit MOCPilot niet, schakel Bluetooth niet uit en zet de hub niet uit terwijl de configuratie wordt gewijzigd.

Het onderbreken van de configuratiewijziging kan de firmware van de hub beschadigen. Als dat gebeurt, kan firmwareherstel nodig zijn voordat de hub weer kan worden gebruikt. Volg indien nodig de gids voor [hubfirmware herstellen](/docs/Application/Hubs/RecoveryHubFirmware/).
:::

Tijdens de herconfiguratie reageert de hub niet op normale commando’s. De LED knippert met een stapsgewijze kleurindicatie totdat het proces klaar is. Nadat de nieuwe configuratie is toegepast, wordt de hub opnieuw geïnitialiseerd.

## Configuratieblokken

MOCPilot bevat ook blokken om de configuratie van Technic Move Hub tijdens een programma te lezen en te wijzigen.

### Hubconfiguratie instellen

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Blok Hubconfiguratie instellen" />

Het blok **Hubconfiguratie instellen** wijzigt de geselecteerde hub naar een van de ondersteunde configuratieprofielen.

- Hubselector: kiest de hub die opnieuw wordt geconfigureerd.
- Configuratieselector: kiest de doelconfiguratie.
- Beschikbare configuraties voor Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** en **Batmobile™ Tumbler**.

Zie de [documentatie van het blok Hubconfiguratie instellen](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Hubconfiguratie

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Blok Hubconfiguratie" />

Het blok **Hubconfiguratie** meldt de huidige configuratie van de geselecteerde hub.

- Hubselector: kiest de hub die wordt gelezen.
- Uitvoerformaat: **tekst** geeft de configuratienaam terug.
- Uitvoerformaat: **index** geeft de configuratie-index terug, handig voor vergelijkingen in voorwaarden.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Uitvoerformaatopties van het blok Hubconfiguratie" />

Zie de [documentatie van het blok Hubconfiguratie](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Vermogenspuls

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Blok Vermogenspuls" />

Het blok **Vermogenspuls** stuurt een power-pulse-commando naar de geselecteerde Technic Move Hub. Dit blok werkt alleen wanneer de Technic Move Hub is geconfigureerd als **Batmobile™ Tumbler**.

Wanneer het wordt uitgevoerd, start de hub de motoren korte tijd met maximaal beschikbare kracht en snelheid, meestal ongeveer 1-2 seconden.

Zie de [documentatie van het blok Vermogenspuls](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Configuratie wijzigen tijdens programmauitvoering

Het is ook mogelijk om de configuratie van Technic Move Hub te wijzigen terwijl een programma draait.

De gebruikelijke aanpak is:

1. Lees de huidige hubconfiguratie.
2. Vergelijk deze met de configuratie die het profiel vereist.
3. Als de configuratie anders is, stel dan de vereiste configuratie in.
4. Lees de configuratie opnieuw na de herconfiguratie.
5. Ga alleen verder wanneer de hub de verwachte configuratie meldt.
6. Koppel los of stop het programma als de vereiste configuratie niet is toegepast.

Het vooraf gebouwde profiel dat deze hub gebruikt, kan als referentie voor deze aanpak dienen.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Blokvoorbeeld voor het wijzigen van de Technic Move Hub-configuratie tijdens uitvoering" />
