---
id: TechnicMoveHubConfigurations
title: Technic Move Hub-konfigurasjoner
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Technic Move Hub-konfigurasjoner

## Oversikt

Technic Move Hub introduserte en unik funksjon i LEGO Powered Up-hubfamilien: huben kan endre oppførsel avhengig av konfigurasjonen som er brukt.

MOCPilot lar deg endre Technic Move Hub-konfigurasjonen slik at hubens oppførsel samsvarer med det offisielle LEGO-settet du vil styre.

## Støttede konfigurasjoner

For øyeblikket er disse Technic Move Hub-konfigurasjonene kjent:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Konfigurasjonsalternativer for Technic Move Hub" />

## Endre konfigurasjon fra Mine Bluetooth-huber

Du kan endre konfigurasjonen fra siden **Mine Bluetooth-huber**:

1. Åpne **Mine Bluetooth-huber**.
2. Finn Technic Move Hub.
3. Åpne kontekstmenyen for huben.
4. Velg **Velg konfigurasjon**.
5. Velg nødvendig konfigurasjon.
6. Bekreft dialogen for rekonfigurering.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Kontekstmeny for Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Konfigurasjonsundermeny for Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Bekreftelsesdialog for rekonfigurering av Technic Move Hub" />

:::warning Viktig
Når hubkonfigurasjonen endres, flashes et underprogram til huben, og prosessen ligner en fastvareoppdatering.

Hold huben slått på under hele prosessen. Hold telefonen, nettbrettet eller datamaskinen slått på og nær huben, slik at Bluetooth-tilkoblingen holder seg stabil. Ikke lukk MOCPilot, ikke slå av Bluetooth og ikke slå av huben mens konfigurasjonen endres.

Hvis konfigurasjonsendringen avbrytes, kan hubens fastvare bli skadet. Da kan fastvaregjenoppretting være nødvendig før huben kan brukes igjen. Følg veiledningen for [gjenoppretting av hubfastvare](/docs/Application/Hubs/RecoveryHubFirmware/) hvis gjenoppretting kreves.
:::

Under rekonfigurering svarer ikke huben på vanlige kommandoer. LED-en blinker med trinnvis fargeindikasjon til prosessen er ferdig. Etter at den nye konfigurasjonen er brukt, initialiseres huben på nytt.

## Konfigurasjonsblokker

MOCPilot inneholder også blokker for å lese og endre Technic Move Hub-konfigurasjonen under et program.

### Angi hub-konfigurasjon

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Blokken Angi hub-konfigurasjon" />

Blokken **Angi hub-konfigurasjon** endrer den valgte huben til en av de støttede konfigurasjonsprofilene.

- Hubvelger: velger huben som skal rekonfigureres.
- Konfigurasjonsvelger: velger målkonfigurasjonen.
- Tilgjengelige konfigurasjoner for Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** og **Batmobile™ Tumbler**.

Se [dokumentasjonen for blokken Angi hub-konfigurasjon](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Hub-konfigurasjon

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Blokken Hub-konfigurasjon" />

Blokken **Hub-konfigurasjon** rapporterer den gjeldende konfigurasjonen for den valgte huben.

- Hubvelger: velger huben som skal leses.
- Utdataformat: **tekst** returnerer konfigurasjonsnavnet.
- Utdataformat: **indeks** returnerer konfigurasjonsindeksen, som er nyttig for sammenligninger i betingelser.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Utdataformatvalg for blokken Hub-konfigurasjon" />

Se [dokumentasjonen for blokken Hub-konfigurasjon](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Strømpuls

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Blokken Strømpuls" />

Blokken **Strømpuls** sender en effektpuls-kommando til den valgte Technic Move Hub. Denne blokken fungerer bare når Technic Move Hub er konfigurert som **Batmobile™ Tumbler**.

Når den kjøres, starter huben motorene med maksimal tilgjengelig kraft og hastighet i kort tid, vanligvis rundt 1-2 sekunder.

Se [dokumentasjonen for blokken Strømpuls](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Endre konfigurasjon mens programmet kjører

Det er også mulig å endre Technic Move Hub-konfigurasjonen mens et program kjører.

Den vanlige fremgangsmåten er:

1. Les den gjeldende hubkonfigurasjonen.
2. Sammenlign den med konfigurasjonen profilen krever.
3. Hvis konfigurasjonen er annerledes, angir du den nødvendige konfigurasjonen.
4. Les konfigurasjonen på nytt etter rekonfigureringen.
5. Fortsett bare når huben rapporterer forventet konfigurasjon.
6. Koble fra eller stopp programmet hvis den nødvendige konfigurasjonen ikke ble brukt.

Den forhåndsbygde profilen som bruker denne huben kan brukes som referanse for denne fremgangsmåten.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Blokkeksempel som viser endring av Technic Move Hub-konfigurasjon under kjøring" />
