---
id: Motors
title: Motoren
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Motoren

Motorblokken worden gebruikt om motoren die op hubpoorten zijn aangesloten te starten, stoppen, positioneren en af te stellen.

## Basis motoropdrachtblokken

### `Start motor` (Beginner) {#block_hubs_all_motors_port_start_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor.svg')} alt="block_hubs_all_motors_port_start_motor.svg" />
Start de geselecteerde motor.

- Richtingsopties: rechtsom / linksom

### `Stop motor` (Beginner) {#block_hubs_all_motors_port_stop_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_stop_motor.svg')} alt="block_hubs_all_motors_port_stop_motor.svg" />
Stopt de geselecteerde motor.

### `Draaien voor` (Gevorderd) {#block_hubs_all_motors_port_run_for}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for.svg')} alt="block_hubs_all_motors_port_run_for.svg" />
Laat de geselecteerde motor draaien voor een opgegeven tijd/hoek/rotatie op basis van de blokinstellingen.

- Richtingsopties: rechtsom / linksom
- Eenheidsopties: `rotaties`, `graden`, `seconden`
- Opmerking: deze functie vereist een motor op de geselecteerde poort die encodergebaseerde besturing ondersteunt.

### `Start motor met snelheid` (Beginner) {#block_hubs_all_motors_port_start_motor_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="block_hubs_all_motors_port_start_motor_at_speed.svg" />
Start de motor met een expliciete snelheidswaarde.

### `Draaien voor met snelheid` (Gevorderd) {#block_hubs_all_motors_port_run_for_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for_at_speed.svg')} alt="block_hubs_all_motors_port_run_for_at_speed.svg" />
Laat de motor draaien voor een doelduur/hoeveelheid met een expliciete snelheid.

- Eenheidsopties: `rotaties`, `graden`, `seconden`
- Opmerking: deze functie vereist een motor op de geselecteerde poort die encodergebaseerde besturing ondersteunt.

### `Stel motorsnelheid in` (Gevorderd) {#block_hubs_all_motors_port_set_motor_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_speed.svg')} alt="block_hubs_all_motors_port_set_motor_speed.svg" />
Stelt de snelheid in die wordt gebruikt door gerelateerde motorblokken.

## Positie- en bewegingsblokken

### `Ga naar positie` (Gevorderd) {#block_hubs_all_motors_port_go_to_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_position.svg')} alt="block_hubs_all_motors_port_go_to_position.svg" />
Verplaatst de motor naar een absolute doelpositie.

- Padopties: `kortste pad`, `rechtsom`, `linksom`
- Opmerking: deze functie vereist een motor op de geselecteerde poort die encodergebaseerde besturing ondersteunt.

### `Ga naar relatieve positie` (Beginner) {#block_hubs_all_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_relative_position.svg')} alt="block_hubs_all_motors_port_go_to_relative_position.svg" />
Verplaatst de motor met een relatieve offset.

- Opmerking: deze functie vereist een motor op de geselecteerde poort die encodergebaseerde besturing ondersteunt.

### `BuWizz 3 ga naar relatieve positie` (Beginner) {#block_hubs_buwizz3_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_motors_port_go_to_relative_position.svg')} alt="block_hubs_buwizz3_motors_port_go_to_relative_position.svg" />
BuWizz 3-variant van het relatieve positioneringsblok.

- Opmerking: deze functie vereist een motor op de geselecteerde poort die encodergebaseerde besturing ondersteunt.

### `Stel relatieve positie in` (Beginner) {#block_hubs_all_motors_port_set_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_relative_position.svg')} alt="block_hubs_all_motors_port_set_relative_position.svg" />
Stelt de referentie voor de relatieve motorpositie in.

- Opmerking: deze functie vereist een motor op de geselecteerde poort die encodergebaseerde besturing ondersteunt.

### `Kalibreer stuurmechanisme` (Beginner) {#block_hubs_all_motors_port_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_calibrate_steering_rack.svg')} alt="block_hubs_all_motors_port_calibrate_steering_rack.svg" />
Kalibreert de neutrale/referentiepositie van het stuurmechanisme.

- Vereiste: de motor op de geselecteerde poort moet absolute/relatieve hoekmeting ondersteunen (interne encoder).
- Mechanische vereiste: de beweging van de stuuras moet fysiek beperkt zijn tot een geldig bereik (bijvoorbeeld met eindstops).
- Werking: het blok scant en meet het beschikbare draaibereik en berekent kalibratiegegevens voor stuurconfiguratie.
- Uitvoer: blokargumenten schrijven resultaten naar variabelen die aan het blok worden doorgegeven (pass-by-reference gedrag).

## Motorafstelling en veiligheidsblokken

### `Stel motorstopgedrag in` (Guru) {#block_hubs_all_motors_port_set_motor_to_at_stop}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_to_at_stop.svg')} alt="block_hubs_all_motors_port_set_motor_to_at_stop.svg" />
Stelt de stopmodus van de motor in (bijvoorbeeld remmen/vasthouden/vrijloop).

- Stopmodi: `rem`, `positie vasthouden`, `vrijloop`
- Opmerking: deze functie vereist een motor op de geselecteerde poort die encodergebaseerde besturing ondersteunt.

### `Stel blokkadedetectie in` (Guru) {#block_hubs_all_motors_port_set_motors_stall_detection}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motors_stall_detection.svg')} alt="block_hubs_all_motors_port_set_motors_stall_detection.svg" />
Schakelt blokkadedetectie in of uit.

- Opmerking: alleen beschikbaar voor de MINDSTORMS Robot Inventor hub.

### `Stel acceleratie in` (Guru) {#block_hubs_all_motors_port_set_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_acceleration.svg')} alt="block_hubs_all_motors_port_set_acceleration.svg" />
Stelt het acceleratieprofiel/snelheid van de motor in.

- Profielopties: `standaard`, `snel`, `gebalanceerd`, `vloeiend`, `traag`, `zeer traag`
- Opmerking: deze functie vereist een motor op de geselecteerde poort die encodergebaseerde besturing ondersteunt.

### `Stel deceleratie in` (Guru) {#block_hubs_all_motors_port_set_deceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_deceleration.svg')} alt="block_hubs_all_motors_port_set_deceleration.svg" />
Stelt het deceleratieprofiel/snelheid van de motor in.

- Profielopties: `standaard`, `snel`, `gebalanceerd`, `vloeiend`, `traag`, `zeer traag`
- Opmerking: deze functie vereist een motor op de geselecteerde poort die encodergebaseerde besturing ondersteunt.

## Motor rapporteurblokken

### `Positie` (Beginner) {#block_hubs_all_motors_port_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_position.svg')} alt="block_hubs_all_motors_port_position.svg" />
Geeft de huidige motorpositie terug.

### `Relatieve positie` (Beginner) {#block_hubs_all_motors_port_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_relative_position.svg')} alt="block_hubs_all_motors_port_relative_position.svg" />
Geeft de huidige relatieve positie terug.

### `Snelheid` (Beginner) {#block_hubs_all_motors_port_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_speed.svg')} alt="block_hubs_all_motors_port_speed.svg" />
Geeft de huidige motorsnelheid terug.

### `Vermogen` (Gevorderd) {#block_hubs_all_motors_port_power}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_power.svg')} alt="block_hubs_all_motors_port_power.svg" />
Geeft het huidige motorvermogen terug.

- Opmerking: alleen beschikbaar voor de MINDSTORMS Robot Inventor hub.

## Technic Move motorblokken

### `Start motoren met snelheid` (Beginner) {#block_hubs_technicmove_motors_start_motors_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_start_motors_at_speed.svg')} alt="block_hubs_technicmove_motors_start_motors_at_speed.svg" />
Start Technic Move aandrijfmotoren met de geselecteerde snelheid.

### `Vermogenspuls` (Beginner) {#block_hubs_technicmove_motors_power_pulse}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="block_hubs_technicmove_motors_power_pulse.svg" />
Stuurt een vermogenspulsopdracht naar de geselecteerde Technic Move Hub.

- Alleen beschikbaar voor Technic Move Hub.
- Typisch gebruik: geef het Technic Move-aandrijfsysteem kort een boost of wek het voordat de volgende blokken doorgaan.

### `Stop motoren` (Beginner) {#block_hubs_technicmove_motors_stop_motors}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_stop_motors.svg')} alt="block_hubs_technicmove_motors_stop_motors.svg" />
Stopt Technic Move aandrijfmotoren.

### `Rem` (Beginner) {#block_hubs_technicmove_motors_brake}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_brake.svg')} alt="block_hubs_technicmove_motors_brake.svg" />
Past remgedrag toe op Technic Move motoren.

- Remopties: `uit`, `aan`

### `Stel stuurmechanisme in op` (Beginner) {#block_hubs_technicmove_motors_set_steering_rack_to}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_set_steering_rack_to.svg')} alt="block_hubs_technicmove_motors_set_steering_rack_to.svg" />
Stelt de doelpositie/waarde van het stuurmechanisme in.

### `Kalibreer stuurmechanisme` (Beginner) {#block_hubs_technicmove_motors_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_calibrate_steering_rack.svg')} alt="block_hubs_technicmove_motors_calibrate_steering_rack.svg" />
Kalibreert het Technic Move stuurmechanisme met behulp van het interne kalibratie-algoritme en automatische detectie van het stuur bereik.

- Opmerking: de motoras moet mechanisch begrensd zijn (bijvoorbeeld door een stuurmechanisme).
