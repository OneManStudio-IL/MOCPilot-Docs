---
id: Control
title: Ovládanie
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Ovládanie

Bloky ovládania riadia tok vykonávania: čakanie, cykly, vetvenie a zastavenie skriptov.

## Bloky čakania

### `Čakaj` (Začiatočník) {#block_control_wait_for}

<img src={useBaseUrl('/img/blocks/block_control_wait_for.svg')} alt="block_control_wait_for.svg" />

Pozastaví aktuálny skript na zadaný čas.

### `Čakaj, kým` (Pokročilý) {#block_control_wait_until}

<img src={useBaseUrl('/img/blocks/block_control_wait_until.svg')} alt="block_control_wait_until.svg" />

Pozastaví aktuálny skript, kým sa podmienka nestane pravdivou.

## Bloky cyklov

### `Opakuj` (Pokročilý) {#block_control_repeat_for}

<img src={useBaseUrl('/img/blocks/block_control_repeat_for.svg')} alt="block_control_repeat_for.svg" />

Spustí vnorené bloky pevne stanovený počet krát.

### `Opakuj, kým` (Pokročilý) {#block_control_repeat_until}

<img src={useBaseUrl('/img/blocks/block_control_repeat_until.svg')} alt="block_control_repeat_until.svg" />

Opakovane vykonáva bloky, kým sa podmienka nestane pravdivou.

### `Navždy` (Pokročilý) {#block_control_repeat_forever}

<img src={useBaseUrl('/img/blocks/block_control_repeat_forever.svg')} alt="block_control_repeat_forever.svg" />

Vykonáva bloky nepretržite, kým sa program alebo skript nezastaví.

## Bloky vetvenia

### `Ak` (Začiatočník) {#block_control_if}

<img src={useBaseUrl('/img/blocks/block_control_if.svg')} alt="block_control_if.svg" />

Spustí vnorené bloky iba vtedy, keď je podmienka pravdivá.

### `Ak / Inak` (Pokročilý) {#block_control_if_else}

<img src={useBaseUrl('/img/blocks/block_control_if_else.svg')} alt="block_control_if_else.svg" />

Spustí jednu vetvu, keď je podmienka pravdivá, inak spustí alternatívnu vetvu.

### `Urob toto a toto` (Guru) {#block_control_do_this_and_this}

<img src={useBaseUrl('/img/blocks/block_control_do_this_and_this.svg')} alt="block_control_do_this_and_this.svg" />

Spustí dve sekvencie blokov po sebe ako jednu operáciu riadenia toku.

## Bloky zastavenia

### `Zastav` (Začiatočník) {#block_control_stop}

<img src={useBaseUrl('/img/blocks/block_control_stop.svg')} alt="block_control_stop.svg" />

Zastaví vykonávanie skriptu (rozsah závisí od zvolenej možnosti).

- Možnosti zastavenia: `všetko`, `tento skript`, `a ukonči program`

### `Zastav ostatné skripty` (Guru) {#block_control_stop_other_stacks}

<img src={useBaseUrl('/img/blocks/block_control_stop_other_stacks.svg')} alt="block_control_stop_other_stacks.svg" />

Zastaví všetky ostatné bežiace skripty, pričom aktuálny skript pokračuje.

## Pomocné bloky hubu/ovládania

### `Nastav pripojenie` (Začiatočník) {#block_hubs_control_set_connect}

<img src={useBaseUrl('/img/blocks/block_hubs_control_set_connect.svg')} alt="block_hubs_control_set_connect.svg" />

Riadi stav pripojenia hubu z logiky programu.

- Možnosti akcie: `pripojiť`, `odpojiť`

### `Nastaviť konfiguráciu hubu` (Pokročilý) {#block_hubs_set_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="block_hubs_set_hub_config.svg" />
Nastaví vybraný hub na jeden z jeho podporovaných konfiguračných profilov.

- Dostupné iba pre huby, ktoré poskytujú možnosti konfigurácie.
- Typické použitie: prepnúť konfigurovateľný hub, napríklad Technic Move Hub, na inú uloženú konfiguráciu pred spustením ďalších blokov.

### `Konfigurácia hubu` (Pokročilý) {#block_hubs_all_control_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="block_hubs_all_control_hub_config.svg" />
Vráti aktuálnu konfiguráciu vybraného hubu.

- Typ: reportovací blok
- Možnosti výstupného formátu: `text`, `index`
- Dostupné iba pre huby, ktoré poskytujú možnosti konfigurácie.
- Vráti `NaN`, keď vybraný hub nie je pripojený alebo nie je dostupná žiadna konfigurácia.

### `Je pripojený` (Začiatočník) {#block_hubs_all_sensors_is_connected}

<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_connected.svg')} alt="block_hubs_all_sensors_is_connected.svg" />

Vracia, či je hub aktuálne pripojený.

- Typ: boolean reporter blok

### `BuWizz 2 nastav režim výkonu` (Začiatočník) {#block_hubs_buwizz_sensors_set_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_set_power_mode.svg')} alt="block_hubs_buwizz_sensors_set_power_mode.svg" />

Nastaví režim výkonu hubu BuWizz 2.

- Možnosti režimu: `Slow`, `Normal`, `Fast`, `Ludicrous`

### `BuWizz 2 zisti režim výkonu` (Guru) {#block_hubs_buwizz_sensors_get_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_power_mode.svg')} alt="block_hubs_buwizz_sensors_get_power_mode.svg" />

Vracia aktuálne aktívny režim výkonu BuWizz 2.

- Možnosti výstupu: `text`, `index`

### `MouldKing nastav riadiaci kanál` (Pokročilý) {#block_hubs_mouldking_control_set_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_set_control_channel.svg')} alt="block_hubs_mouldking_control_set_control_channel.svg" />

Nastaví aktívny riadiaci kanál pre podporovaný MouldKing hub/ovládač.

- Možnosti kanála: `A`, `B`, `C`

### `MouldKing zisti riadiaci kanál` (Pokročilý) {#block_hubs_mouldking_control_get_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_get_control_channel.svg')} alt="block_hubs_mouldking_control_get_control_channel.svg" />

Vracia aktuálne aktívny riadiaci kanál.

- Možnosti výstupu: `text`, `index`