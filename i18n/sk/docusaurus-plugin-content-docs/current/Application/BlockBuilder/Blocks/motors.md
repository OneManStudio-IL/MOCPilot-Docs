---
id: Motors
title: Motory
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Motory

Bloky motorov sa používajú na spúšťanie, zastavovanie, polohovanie a nastavovanie motorov pripojených k portom hubu.

## Základné príkazové bloky motorov

### `Spusti motor` (Začiatočník) {#block_hubs_all_motors_port_start_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor.svg')} alt="block_hubs_all_motors_port_start_motor.svg" />
Spustí vybraný motor.

- Možnosti smeru: `v smere hodinových ručičiek` / `proti smeru hodinových ručičiek`

### `Zastav motor` (Začiatočník) {#block_hubs_all_motors_port_stop_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_stop_motor.svg')} alt="block_hubs_all_motors_port_stop_motor.svg" />
Zastaví vybraný motor.

### `Spusti na` (Pokročilý) {#block_hubs_all_motors_port_run_for}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for.svg')} alt="block_hubs_all_motors_port_run_for.svg" />
Spustí vybraný motor na zadaný čas/uhol/počet otáčok podľa nastavenia bloku.

- Možnosti smeru: `v smere hodinových ručičiek` / `proti smeru hodinových ručičiek`
- Možnosti jednotiek: `otáčky`, `stupne`, `sekundy`
- Poznámka: táto funkcia vyžaduje motor na vybranom porte, ktorý podporuje riadenie pomocou enkódera.

### `Spusti motor rýchlosťou` (Začiatočník) {#block_hubs_all_motors_port_start_motor_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="block_hubs_all_motors_port_start_motor_at_speed.svg" />
Spustí motor s explicitne zadanou rýchlosťou.

### `Spusti na rýchlosťou` (Pokročilý) {#block_hubs_all_motors_port_run_for_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for_at_speed.svg')} alt="block_hubs_all_motors_port_run_for_at_speed.svg" />
Spustí motor na cieľový čas/množstvo s nastavenou rýchlosťou.

- Možnosti jednotiek: `otáčky`, `stupne`, `sekundy`
- Poznámka: táto funkcia vyžaduje motor na vybranom porte, ktorý podporuje riadenie pomocou enkódera.

### `Nastav rýchlosť motora` (Pokročilý) {#block_hubs_all_motors_port_set_motor_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_speed.svg')} alt="block_hubs_all_motors_port_set_motor_speed.svg" />
Nastaví rýchlosť používanú príbuznými blokmi pre spúšťanie motora.

## Bloky polohy a pohybu

### `Prejdi na pozíciu` (Pokročilý) {#block_hubs_all_motors_port_go_to_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_position.svg')} alt="block_hubs_all_motors_port_go_to_position.svg" />
Presunie motor na cieľovú absolútnu pozíciu.

- Možnosti trajektórie: `najkratšia cesta`, `v smere hodinových ručičiek`, `proti smeru hodinových ručičiek`
- Poznámka: vyžaduje motor s podporou enkódera.

### `Prejdi na relatívnu pozíciu` (Začiatočník) {#block_hubs_all_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_relative_position.svg')} alt="block_hubs_all_motors_port_go_to_relative_position.svg" />
Presunie motor o relatívnu hodnotu.

- Poznámka: vyžaduje motor s podporou enkódera.

### `BuWizz 3 prejdi na relatívnu pozíciu` (Začiatočník) {#block_hubs_buwizz3_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_motors_port_go_to_relative_position.svg')} alt="block_hubs_buwizz3_motors_port_go_to_relative_position.svg" />
Variant pre BuWizz 3.

- Poznámka: vyžaduje motor s podporou enkódera.

### `Nastav relatívnu pozíciu` (Začiatočník) {#block_hubs_all_motors_port_set_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_relative_position.svg')} alt="block_hubs_all_motors_port_set_relative_position.svg" />
Nastaví referenčnú relatívnu pozíciu motora.

- Poznámka: vyžaduje motor s podporou enkódera.

### `Kalibruj riadiacu tyč` (Začiatočník) {#block_hubs_all_motors_port_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_calibrate_steering_rack.svg')} alt="block_hubs_all_motors_port_calibrate_steering_rack.svg" />
Kalibruje nulovú/referenčnú pozíciu riadiacej tyče.

- Požiadavka: motor musí podporovať sledovanie uhla (enkóder)
- Mechanická požiadavka: pohyb musí byť fyzicky obmedzený
- Ako to funguje: blok vykoná meranie rozsahu a vypočíta kalibráciu
- Výstup: zapisuje výsledky do premenných (referenčné správanie)

## Bloky ladenia a bezpečnosti

### `Nastav správanie motora pri zastavení` (Guru) {#block_hubs_all_motors_port_set_motor_to_at_stop}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_to_at_stop.svg')} alt="block_hubs_all_motors_port_set_motor_to_at_stop.svg" />
Nastaví režim zastavenia motora.

- Možnosti: `brzda`, `držanie pozície`, `voľný chod`

### `Nastav detekciu zablokovania` (Guru) {#block_hubs_all_motors_port_set_motors_stall_detection}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motors_stall_detection.svg')} alt="block_hubs_all_motors_port_set_motors_stall_detection.svg" />
Zapne alebo vypne detekciu zablokovania.

- Dostupné iba pre `MINDSTORMS Robot Inventor`

### `Nastav zrýchlenie` (Guru) {#block_hubs_all_motors_port_set_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_acceleration.svg')} alt="block_hubs_all_motors_port_set_acceleration.svg" />
Nastaví profil zrýchlenia.

- Možnosti: `predvolené`, `rýchle`, `vyvážené`, `hladké`, `pomalé`, `veľmi pomalé`

### `Nastav spomalenie` (Guru) {#block_hubs_all_motors_port_set_deceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_deceleration.svg')} alt="block_hubs_all_motors_port_set_deceleration.svg" />
Nastaví profil spomalenia.

- Možnosti: `predvolené`, `rýchle`, `vyvážené`, `hladké`, `pomalé`, `veľmi pomalé`

## Reporter bloky motorov

### `Pozícia` (Začiatočník) {#block_hubs_all_motors_port_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_position.svg')} alt="block_hubs_all_motors_port_position.svg" />
Vracia aktuálnu pozíciu motora.

### `Relatívna pozícia` (Začiatočník) {#block_hubs_all_motors_port_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_relative_position.svg')} alt="block_hubs_all_motors_port_relative_position.svg" />
Vracia aktuálnu relatívnu pozíciu.

### `Rýchlosť` (Začiatočník) {#block_hubs_all_motors_port_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_speed.svg')} alt="block_hubs_all_motors_port_speed.svg" />
Vracia aktuálnu rýchlosť motora.

### `Výkon` (Pokročilý) {#block_hubs_all_motors_port_power}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_power.svg')} alt="block_hubs_all_motors_port_power.svg" />
Vracia aktuálnu hodnotu výkonu motora.

- Poznámka: dostupné iba pre `MINDSTORMS Robot Inventor`

## Technic Move bloky motorov

### `Spusti motory rýchlosťou` (Začiatočník) {#block_hubs_technicmove_motors_start_motors_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_start_motors_at_speed.svg')} alt="block_hubs_technicmove_motors_start_motors_at_speed.svg" />
Spustí pohonné motory Technic Move.

### `Napájací impulz` (Začiatočník) {#block_hubs_technicmove_motors_power_pulse}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="block_hubs_technicmove_motors_power_pulse.svg" />
Odošle príkaz napájacieho impulzu do vybraného Technic Move Hubu.

- Dostupné iba pre Technic Move Hub.
- Typické použitie: krátko zosilniť alebo prebudiť pohonný systém Technic Move pred pokračovaním ďalšími blokmi.

### `Zastav motory` (Začiatočník) {#block_hubs_technicmove_motors_stop_motors}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_stop_motors.svg')} alt="block_hubs_technicmove_motors_stop_motors.svg" />
Zastaví motory.

### `Brzda` (Začiatočník) {#block_hubs_technicmove_motors_brake}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_brake.svg')} alt="block_hubs_technicmove_motors_brake.svg" />
Aplikuje brzdenie.

- Možnosti: `vypnuté`, `povolené`

### `Nastav riadiacu tyč na` (Začiatočník) {#block_hubs_technicmove_motors_set_steering_rack_to}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_set_steering_rack_to.svg')} alt="block_hubs_technicmove_motors_set_steering_rack_to.svg" />
Nastaví cieľovú hodnotu riadenia.

### `Kalibruj riadiacu tyč` (Začiatočník) {#block_hubs_technicmove_motors_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_calibrate_steering_rack.svg')} alt="block_hubs_technicmove_motors_calibrate_steering_rack.svg" />
Kalibruje riadenie pomocou automatického rozsahu.
