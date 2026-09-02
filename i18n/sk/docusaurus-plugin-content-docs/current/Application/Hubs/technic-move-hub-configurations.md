---
id: TechnicMoveHubConfigurations
title: Konfigurácie Technic Move Hub
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Konfigurácie Technic Move Hub

## Prehľad

Technic Move Hub priniesol do rodiny hubov LEGO Powered Up jedinečnú funkciu: hub môže meniť svoje správanie podľa aktuálne použitej konfigurácie.

MOCPilot umožňuje zmeniť konfiguráciu Technic Move Hubu tak, aby správanie hubu zodpovedalo oficiálnej LEGO sade, ktorú chcete ovládať.

## Podporované konfigurácie

Momentálne sú známe tieto konfigurácie Technic Move Hubu:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Možnosti konfigurácie Technic Move Hubu" />

## Zmena konfigurácie z Moje Bluetooth huby

Konfiguráciu môžete zmeniť zo stránky **Moje Bluetooth huby**:

1. Otvorte **Moje Bluetooth huby**.
2. Nájdite Technic Move Hub.
3. Otvorte kontextové menu hubu.
4. Vyberte **Vybrať konfiguráciu**.
5. Vyberte požadovanú konfiguráciu.
6. Potvrďte dialóg rekonfigurácie.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Kontextové menu Technic Move Hubu" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Podmenu konfigurácie Technic Move Hubu" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Potvrdzovací dialóg rekonfigurácie Technic Move Hubu" />

:::warning Dôležité
Zmena konfigurácie hubu nahrá do hubu podprogram a podobá sa procesu aktualizácie firmvéru.

Počas celého procesu nechajte hub zapnutý. Telefón, tablet alebo počítač majte zapnutý a blízko hubu, aby bolo Bluetooth pripojenie stabilné. Počas zmeny konfigurácie nezatvárajte MOCPilot, nevypínajte Bluetooth ani hub.

Prerušenie zmeny konfigurácie môže poškodiť firmvér hubu. Ak sa to stane, pred ďalším použitím môže byť potrebná obnova firmvéru. Ak je obnova potrebná, postupujte podľa návodu na [obnovu firmvéru hubu](/docs/Application/Hubs/RecoveryHubFirmware/).
:::

Počas rekonfigurácie hub nereaguje na bežné príkazy. Jeho LED bliká stupňovanou farebnou indikáciou, kým sa proces nedokončí. Po použití novej konfigurácie sa hub znova inicializuje.

## Konfiguračné bloky

MOCPilot obsahuje aj bloky na čítanie a zmenu konfigurácie Technic Move Hubu počas programu.

### Nastaviť konfiguráciu hubu

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Blok Nastaviť konfiguráciu hubu" />

Blok **Nastaviť konfiguráciu hubu** zmení vybraný hub na jeden z podporovaných konfiguračných profilov.

- Výber hubu: vyberie hub na rekonfiguráciu.
- Výber konfigurácie: vyberie cieľovú konfiguráciu.
- Dostupné konfigurácie pre Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** a **Batmobile™ Tumbler**.

Pozrite si [dokumentáciu bloku Nastaviť konfiguráciu hubu](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Konfigurácia hubu

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Blok Konfigurácia hubu" />

Blok **Konfigurácia hubu** hlási aktuálnu konfiguráciu vybraného hubu.

- Výber hubu: vyberie hub, ktorý sa má čítať.
- Formát výstupu: **textová hodnota** vráti názov konfigurácie.
- Formát výstupu: **index** vráti poradový index konfigurácie, čo je užitočné na porovnania v podmienkach.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Možnosti formátu výstupu bloku Konfigurácia hubu" />

Pozrite si [dokumentáciu bloku Konfigurácia hubu](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Napájací impulz

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Blok Napájací impulz" />

Blok **Napájací impulz** odošle vybranému Technic Move Hubu príkaz výkonového impulzu. Tento blok funguje iba vtedy, keď je Technic Move Hub nakonfigurovaný ako **Batmobile™ Tumbler**.

Pri spustení hub na krátky čas spustí motory s maximálnym dostupným výkonom a rýchlosťou, zvyčajne približne na 1-2 sekundy.

Pozrite si [dokumentáciu bloku Napájací impulz](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Zmena konfigurácie počas behu programu

Konfiguráciu Technic Move Hubu je možné meniť aj počas behu programu.

Bežný postup je:

1. Prečítajte aktuálnu konfiguráciu hubu.
2. Porovnajte ju s konfiguráciou požadovanou profilom.
3. Ak je konfigurácia iná, nastavte požadovanú konfiguráciu.
4. Po rekonfigurácii znova prečítajte konfiguráciu.
5. Pokračujte iba vtedy, keď hub hlási očakávanú konfiguráciu.
6. Ak požadovaná konfigurácia nebola použitá, odpojte hub alebo zastavte program.

Predpripravený profil, ktorý používa tento hub, môže slúžiť ako referencia pre tento postup.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Príklad blokov zobrazujúci zmenu konfigurácie Technic Move Hubu počas behu" />
