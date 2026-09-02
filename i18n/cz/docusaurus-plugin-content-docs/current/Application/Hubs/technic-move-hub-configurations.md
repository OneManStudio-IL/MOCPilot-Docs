---
id: TechnicMoveHubConfigurations
title: Konfigurace Technic Move Hub
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Konfigurace Technic Move Hub

## Přehled

Technic Move Hub přinesl do rodiny LEGO Powered Up hubů jedinečnou funkci: hub může měnit své chování podle aktuálně použité konfigurace.

MOCPilot umožňuje změnit konfiguraci Technic Move Hubu tak, aby se chování hubu shodovalo s oficiální LEGO sadou, kterou chcete ovládat.

## Podporované konfigurace

V tuto chvíli jsou známy tyto konfigurace Technic Move Hubu:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Možnosti konfigurace Technic Move Hubu" />

## Změna konfigurace z Moje Bluetooth huby

Konfiguraci můžete změnit ze stránky **Moje Bluetooth huby**:

1. Otevřete **Moje Bluetooth huby**.
2. Najděte Technic Move Hub.
3. Otevřete kontextové menu hubu.
4. Vyberte **Vybrat konfiguraci**.
5. Zvolte požadovanou konfiguraci.
6. Potvrďte dialog rekonfigurace.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Kontextové menu Technic Move Hubu" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Podmenu konfigurace Technic Move Hubu" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Potvrzovací dialog rekonfigurace Technic Move Hubu" />

:::warning Důležité
Změna konfigurace hubu nahraje do hubu podprogram a podobá se procesu aktualizace firmwaru.

Během celého procesu nechte hub zapnutý. Telefon, tablet nebo počítač mějte nabitý a blízko hubu, aby bylo připojení Bluetooth stabilní. Během změny konfigurace nezavírejte MOCPilot, nevypínejte Bluetooth ani hub.

Přerušení změny konfigurace může poškodit firmware hubu. Pokud k tomu dojde, může být před dalším použitím nutná obnova firmwaru. V případě potřeby postupujte podle průvodce [obnovou firmwaru hubu](/docs/Application/Hubs/RecoveryHubFirmware/).
:::

Během rekonfigurace hub nereaguje na běžné příkazy. Jeho LED bliká stupňovanou barevnou indikací, dokud proces neskončí. Po použití nové konfigurace se hub znovu inicializuje.

## Konfigurační bloky

MOCPilot také obsahuje bloky pro čtení a změnu konfigurace Technic Move Hubu během programu.

### Nastavit konfiguraci hubu

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Blok Nastavit konfiguraci hubu" />

Blok **Nastavit konfiguraci hubu** změní vybraný hub na jeden z podporovaných konfiguračních profilů.

- Výběr hubu: zvolí hub k rekonfiguraci.
- Výběr konfigurace: zvolí cílovou konfiguraci.
- Dostupné konfigurace pro Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** a **Batmobile™ Tumbler**.

Viz [dokumentace bloku Nastavit konfiguraci hubu](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Konfigurace hubu

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Blok Konfigurace hubu" />

Blok **Konfigurace hubu** hlásí aktuální konfiguraci vybraného hubu.

- Výběr hubu: zvolí hub, který se má přečíst.
- Formát výstupu: **textová hodnota** vrátí název konfigurace.
- Formát výstupu: **index** vrátí pořadový index konfigurace, což je užitečné pro porovnávání v podmínkách.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Možnosti formátu výstupu bloku Konfigurace hubu" />

Viz [dokumentace bloku Konfigurace hubu](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Napájecí pulz

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Blok Napájecí pulz" />

Blok **Napájecí pulz** odešle vybranému Technic Move Hubu příkaz výkonového pulzu. Tento blok funguje pouze tehdy, když je Technic Move Hub nakonfigurován jako **Batmobile™ Tumbler**.

Při spuštění hub krátce roztočí motory s maximálním dostupným výkonem a rychlostí, obvykle asi na 1-2 sekundy.

Viz [dokumentace bloku Napájecí pulz](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Změna konfigurace za běhu programu

Konfiguraci Technic Move Hubu je možné změnit také během běhu programu.

Běžný postup je:

1. Přečtěte aktuální konfiguraci hubu.
2. Porovnejte ji s konfigurací požadovanou profilem.
3. Pokud je konfigurace jiná, nastavte požadovanou konfiguraci.
4. Po rekonfiguraci znovu přečtěte konfiguraci.
5. Pokračujte pouze tehdy, když hub hlásí očekávanou konfiguraci.
6. Pokud požadovaná konfigurace nebyla použita, odpojte hub nebo zastavte program.

Předpřipravený profil, který tento hub používá, může sloužit jako reference pro tento postup.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Příklad bloků pro změnu konfigurace Technic Move Hubu za běhu" />
