---
id: Control
title: Kontroll
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Kontroll

Kontrollblock styr exekveringsflödet: väntan, loopar, förgreningar och att stoppa skript.

## Väntblock

### `Vänta` (Nybörjare) {#block_control_wait_for}

<img src={useBaseUrl('/img/blocks/block_control_wait_for.svg')} alt="block_control_wait_for.svg" />

Pausar det aktuella skriptet under en angiven tid.

### `Vänta tills` (Avancerad) {#block_control_wait_until}

<img src={useBaseUrl('/img/blocks/block_control_wait_until.svg')} alt="block_control_wait_until.svg" />

Pausar det aktuella skriptet tills ett villkor blir sant.

## Loopblock

### `Upprepa` (Avancerad) {#block_control_repeat_for}

<img src={useBaseUrl('/img/blocks/block_control_repeat_for.svg')} alt="block_control_repeat_for.svg" />

Kör nästlade block ett bestämt antal gånger.

### `Upprepa tills` (Avancerad) {#block_control_repeat_until}

<img src={useBaseUrl('/img/blocks/block_control_repeat_until.svg')} alt="block_control_repeat_until.svg" />

Kör nästlade block upprepade gånger tills ett villkor blir sant.

### `För alltid` (Avancerad) {#block_control_repeat_forever}

<img src={useBaseUrl('/img/blocks/block_control_repeat_forever.svg')} alt="block_control_repeat_forever.svg" />

Kör nästlade block kontinuerligt tills programmet eller skriptet stoppas.

## Förgreningsblock

### `Om` (Nybörjare) {#block_control_if}

<img src={useBaseUrl('/img/blocks/block_control_if.svg')} alt="block_control_if.svg" />

Kör nästlade block endast när villkoret är sant.

### `Om / Annars` (Avancerad) {#block_control_if_else}

<img src={useBaseUrl('/img/blocks/block_control_if_else.svg')} alt="block_control_if_else.svg" />

Kör en gren när villkoret är sant, annars körs den alternativa grenen.

### `Gör detta och detta` (Guru) {#block_control_do_this_and_this}

<img src={useBaseUrl('/img/blocks/block_control_do_this_and_this.svg')} alt="block_control_do_this_and_this.svg" />

Kör två blockstaplar i följd som en del av ett kontrollflöde.

## Stoppblock

### `Stoppa` (Nybörjare) {#block_control_stop}

<img src={useBaseUrl('/img/blocks/block_control_stop.svg')} alt="block_control_stop.svg" />

Stoppar skriptexekvering (omfattningen beror på valt stoppalternativ).

- Stoppalternativ: `alla`, `denna stapel`, `och avsluta programmet`

### `Stoppa andra staplar` (Guru) {#block_control_stop_other_stacks}

<img src={useBaseUrl('/img/blocks/block_control_stop_other_stacks.svg')} alt="block_control_stop_other_stacks.svg" />

Stoppar alla andra körande staplar medan den aktuella stapeln får fortsätta.

## Hubb-/kontrollverktygsblock

### `Anslut / koppla från` (Nybörjare) {#block_hubs_control_set_connect}

<img src={useBaseUrl('/img/blocks/block_hubs_control_set_connect.svg')} alt="block_hubs_control_set_connect.svg" />

Styr hubbens anslutningsstatus från kontrollflödeslogik.

- Åtgärdsalternativ: `anslut`, `koppla från`

### `Ställ in hubbkonfiguration` (Avancerad) {#block_hubs_set_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="block_hubs_set_hub_config.svg" />
Ställer in den valda hubben till en av dess konfigurationsprofiler som stöds.

- Endast tillgänglig för hubbar som erbjuder konfigurationsalternativ.
- Typisk användning: växla en konfigurerbar hubb, som Technic Move Hub, till en annan sparad konfiguration innan nästa block körs.

### `Hubbkonfiguration` (Avancerad) {#block_hubs_all_control_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="block_hubs_all_control_hub_config.svg" />
Returnerar den aktuella konfigurationen för den valda hubben.

- Typ: rapportblock
- Utdataformatsval: `text`, `index`
- Endast tillgänglig för hubbar som erbjuder konfigurationsalternativ.
- Returnerar `NaN` när den valda hubben inte är ansluten eller ingen konfiguration är tillgänglig.

### `Är ansluten` (Nybörjare) {#block_hubs_all_sensors_is_connected}

<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_connected.svg')} alt="block_hubs_all_sensors_is_connected.svg" />

Returnerar om hubben för närvarande är ansluten.

- Typ: booleskt reporterblock

### `BuWizz 2 ställ in effektläge` (Nybörjare) {#block_hubs_buwizz_sensors_set_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_set_power_mode.svg')} alt="block_hubs_buwizz_sensors_set_power_mode.svg" />

Ställer in effektläget för BuWizz 2-hubben.

- Lägesalternativ: `Slow`, `Normal`, `Fast`, `Ludicrous`

### `BuWizz 2 hämta effektläge` (Guru) {#block_hubs_buwizz_sensors_get_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_power_mode.svg')} alt="block_hubs_buwizz_sensors_get_power_mode.svg" />

Returnerar det aktuella effektläget för BuWizz 2.

- Alternativ för utdataformat: `text`, `index`

### `MouldKing ställ in kontrollkanal` (Avancerad) {#block_hubs_mouldking_control_set_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_set_control_channel.svg')} alt="block_hubs_mouldking_control_set_control_channel.svg" />

Ställer in aktiv kontrollkanal för stödd MouldKing-hubb/-kontroller.

- Kanalalternativ: `A`, `B`, `C`

### `MouldKing hämta kontrollkanal` (Avancerad) {#block_hubs_mouldking_control_get_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_get_control_channel.svg')} alt="block_hubs_mouldking_control_get_control_channel.svg" />

Returnerar aktuell aktiv kontrollkanal för stödd MouldKing-hubb/-kontroller.

- Alternativ för utdataformat: `text`, `index`
