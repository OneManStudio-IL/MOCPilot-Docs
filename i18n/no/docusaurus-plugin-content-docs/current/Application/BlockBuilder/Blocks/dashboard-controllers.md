---
id: DashboardControllers
title: Dashboard-kontrollere
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Dashboard-kontrollere

Disse blokkene brukes til å lese brukerinput fra skjermkontroller, reagere på brukerhandlinger og oppdatere dashboardets UI-tilstand.

## Globale dashboard-kontrollerblokker

### `Sett kontrollerfarge` (Avansert) {#block_dashboard_controller_all_set_color}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_all_set_color.svg')} alt="block_dashboard_controller_all_set_color.svg" />

Endrer den visuelle aksentfargen til valgt dashboard-kontroller.

- Type: kommandoblokk
- Typisk bruk: indikere kjøretidstilstander eller dynamisk endre kontrollerstil basert på betingelser

### `Sett kontrollerinteraktivitet` (Avansert) {#block_dashboard_controller_all_set_interactivity}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_all_set_interactivity.svg')} alt="block_dashboard_controller_all_set_interactivity.svg" />

Kontrollerer interaktiviteten til valgt dashboard-kontroller.  
Hvis interaktivitet er deaktivert, reagerer ikke kontrolleren på berøringsinput.

- Type: kommandoblokk
- Typisk bruk: midlertidig låse kontroller under spesifikk logikk eller sikkerhetstilstander
- Tilstandsvalg: `aktiver`, `deaktiver`

## Knappblokker

### `Knapphendelse` (Nybegynner) {#block_dashboard_controller_button_event}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_button_event.svg')} alt="block_dashboard_controller_button_event.svg" />

Utløses når dashboard-knappen endrer tilstand (trykket/sluppet).

- Type: hendelsesblokk
- Output: starter tilkoblet skript
- Tilstandsvalg: `trykket`, `sluppet`

### `Knappverdi (boolsk)` (Nybegynner) {#block_dashboard_controller_button_value_boolean}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_button_value_boolean.svg')} alt="block_dashboard_controller_button_value_boolean.svg" />

Rapporterer gjeldende tilstand for dashboard-knappen.

- Type: verdiblokk
- Output: `true`/`false`
- Tilstandsvalg: `trykket`, `sluppet`

## D-pad-blokker

### `D-pad-hendelse` (Nybegynner) {#block_dashboard_controller_dpad_event}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_dpad_event.svg')} alt="block_dashboard_controller_dpad_event.svg" />

Utløses når D-pad-retningen endres eller matcher konfigurert retning.

- Type: hendelsesblokk
- Output: starter tilkoblet skript
- Retningsvalg: `opp`, `ned`, `venstre`, `høyre`
- Knappetilstand: `trykket`, `sluppet`

### `D-pad-verdi (boolsk)` (Nybegynner) {#block_dashboard_controller_dpad_value_boolean}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_dpad_value_boolean.svg')} alt="block_dashboard_controller_dpad_value_boolean.svg" />

Rapporterer om valgt D-pad-retning er aktiv.

- Type: verdiblokk
- Output: `true`/`false`
- Retningsvalg: `opp`, `ned`, `venstre`, `høyre`
- Knappetilstand: `trykket`, `sluppet`

## Joystick-blokker

### `Joystick-hendelse` (Nybegynner) {#block_dashboard_controller_joystick_event}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_joystick_event.svg')} alt="block_dashboard_controller_joystick_event.svg" />

Utløses når joystick-posisjonen endres.

- Type: hendelsesblokk
- Output: starter tilkoblet skript
- Tilstandsvalg: `opp`, `ned`, `venstre`, `høyre`, `flyttet`, `sluppet`

### `Joystick-verdi (float)` (Nybegynner) {#block_dashboard_controller_joystick_value_float}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_joystick_value_float.svg')} alt="block_dashboard_controller_joystick_value_float.svg" />

Rapporterer joystick-akseverdi.

- Type: verdiblokk
- Output: numerisk (float), vanligvis i et normalisert område
- Aksevalg: `x-akse`, `y-akse`

### `Joystick-verdi (boolean)` (Nybegynner) {#block_dashboard_controller_joystick_value_boolean}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_joystick_value_boolean.svg')} alt="block_dashboard_controller_joystick_value_boolean.svg" />

Rapporterer om den valgte joysticken er trykket eller sluppet.

- Type: verdiblokk
- Output: `true`/`false`
- Statusvalg: `trykket`, `sluppet`

## Pedalblokker

### `Pedalhendelse` (Nybegynner) {#block_dashboard_controller_pedals_event}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_pedals_event.svg')} alt="block_dashboard_controller_pedals_event.svg" />

Utløses når pedalinput endres.

- Type: hendelsesblokk
- Output: starter tilkoblet skript
- Pedalvalg: `hvilken som helst`, `brems`, `akselerasjon`
- Tilstandsvalg: `flyttet`, `trykket`, `sluppet`

### `Pedalverdi (float)` (Nybegynner) {#block_dashboard_controller_pedals_value_float}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_pedals_value_float.svg')} alt="block_dashboard_controller_pedals_value_float.svg" />

Rapporterer analog pedalverdi.

- Type: verdiblokk
- Output: numerisk (float)

### `Pedalverdi (boolsk)` (Nybegynner) {#block_dashboard_controller_pedals_value_boolean}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_pedals_value_boolean.svg')} alt="block_dashboard_controller_pedals_value_boolean.svg" />

Returnerer valgt tilstand basert på om en spesifikk pedal er trykket eller sluppet.

- Type: verdiblokk
- Output: `true`/`false`
- Pedalvalg: `brems`, `akselerasjon`
- Tilstandsvalg: `trykket`, `sluppet`

## Sliderblokker

### `Slider-hendelse` (Nybegynner) {#block_dashboard_controller_slider_event}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_slider_event.svg')} alt="block_dashboard_controller_slider_event.svg" />

Utløses når sliderverdi endres.

- Type: hendelsesblokk
- Output: starter tilkoblet skript
- Tilstandsvalg: `lav`, `høy`, `flyttet`, `sluppet`

### `Sliderverdi (float)` (Nybegynner) {#block_dashboard_controller_slider_value_float}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_slider_value_float.svg')} alt="block_dashboard_controller_slider_value_float.svg" />

Rapporterer gjeldende sliderverdi.

- Type: verdiblokk
- Output: numerisk (float)

## Stepperblokker

### `Stepper-hendelse` (Nybegynner) {#block_dashboard_controller_stepper_event}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_stepper_event.svg')} alt="block_dashboard_controller_stepper_event.svg" />

Utløses når stepperverdi endres med ett steg.

- Type: hendelsesblokk
- Output: starter tilkoblet skript
- Stegvalg: `hvilken som helst`, `reset`, `minus`, `pluss`
- Knappetilstand: `trykket`, `sluppet`

### `Stepperverdi (float)` (Nybegynner) {#block_dashboard_controller_stepper_value_float}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_stepper_value_float.svg')} alt="block_dashboard_controller_stepper_value_float.svg" />

Rapporterer gjeldende stepperverdi.

- Type: verdiblokk
- Output: numerisk (float)

## Rattblokker

### `Ratt-hendelse` (Nybegynner) {#block_dashboard_controller_steering_wheel_event}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_event.svg')} alt="block_dashboard_controller_steering_wheel_event.svg" />

Utløses når rattposisjonen endres.

- Type: hendelsesblokk
- Output: starter tilkoblet skript
- Tilstandsvalg: `flyttet`, `trykket`, `sluppet`

### `Rattverdi (float)` (Nybegynner) {#block_dashboard_controller_steering_wheel_value_float}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="block_dashboard_controller_steering_wheel_value_float.svg" />

Rapporterer gjeldende rattverdi.

- Type: verdiblokk
- Output: numerisk (float)

### `Rattverdi (boolsk)` (Nybegynner) {#block_dashboard_controller_steeringwheel_value_boolean}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_steeringwheel_value_boolean.svg')} alt="block_dashboard_controller_steeringwheel_value_boolean.svg" />

Returnerer valgt tilstand basert på om rattet er trykket eller sluppet.

- Type: verdiblokk
- Output: `true`/`false`
- Tilstandsvalg: `flyttet`, `trykket`, `sluppet`

## Bryterblokker

### `Bryter-hendelse` (Nybegynner) {#block_dashboard_controller_switch_event}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_switch_event.svg')} alt="block_dashboard_controller_switch_event.svg" />

Utløses når brytertilstand endres.

- Type: hendelsesblokk
- Output: starter tilkoblet skript
- Valg: `på`, `av`

### `Bryterverdi (boolsk)` (Nybegynner) {#block_dashboard_controller_switch_value_boolean}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_switch_value_boolean.svg')} alt="block_dashboard_controller_switch_value_boolean.svg" />

Rapporterer gjeldende brytertilstand.

- Type: verdiblokk
- Output: `true`/`false`
- Tilstandsvalg: `på`, `av`

## Monitorblokker

### `Vis på monitor` (Nybegynner) {#block_dashboard_controller_monitor_show}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_monitor_show.svg')} alt="block_dashboard_controller_monitor_show.svg" />

Viser informasjon (tekst eller verdi) på dashboard-monitoren.

- Type: kommandoblokk
- Typisk bruk: vise batterinivå, motorvinkel, tilkoblet enhet på hub-port osv.

### `Sett monitorverdi` (Nybegynner) {#block_dashboard_controller_monitor_set_value}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_monitor_set_value.svg')} alt="block_dashboard_controller_monitor_set_value.svg" />

Setter heltallsverdi for en dashboard speedometer-monitor.

- Type: kommandoblokk
- Typisk bruk: oppdatere speedometerverdi under kjøring

### `Sett tiltmonitorverdi` (Nybegynner) {#block_dashboard_controller_monitor_tilt_set_value}

<img src={useBaseUrl('/img/blocks/block_dashboard_controller_monitor_tilt_set_value.svg')} alt="block_dashboard_controller_monitor_tilt_set_value.svg" />

Setter tiltmonitorverdi (stigning/rulling) for dashboard tiltmonitor.

- Type: kommandoblokk
- Typisk bruk: vise tiltverdier i sanntid
- Aksevalg: `stigning`, `rulling`
