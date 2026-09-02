---
id: Motors
title: Moottorit
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Moottorit

Moottorilohkoja käytetään käynnistämään, pysäyttämään, asemointiin ja säätämään hubin portteihin liitettyjä moottoreita.

## Perusmoottorikomennot

### `Käynnistä moottori` (Aloittelija) {#block_hubs_all_motors_port_start_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor.svg')} alt="block_hubs_all_motors_port_start_motor.svg" />
Käynnistää valitun moottorin.

- Suuntavaihtoehdot: myötäpäivään / vastapäivään

### `Pysäytä moottori` (Aloittelija) {#block_hubs_all_motors_port_stop_motor}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_stop_motor.svg')} alt="block_hubs_all_motors_port_stop_motor.svg" />
Pysäyttää valitun moottorin.

### `Suorita ajan verran` (Edistynyt) {#block_hubs_all_motors_port_run_for}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for.svg')} alt="block_hubs_all_motors_port_run_for.svg" />
Suorittaa moottoria määritetyn ajan/kulman/pyörähdyksen ajan.

- Suuntavaihtoehdot: myötäpäivään / vastapäivään
- Yksiköt: `kierrokset`, `asteet`, `sekunnit`
- Huom: vaatii encoder-tuetun moottorin.

### `Käynnistä moottori nopeudella` (Aloittelija) {#block_hubs_all_motors_port_start_motor_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="block_hubs_all_motors_port_start_motor_at_speed.svg" />
Käynnistää moottorin annetulla nopeudella.

### `Suorita ajan verran nopeudella` (Edistynyt) {#block_hubs_all_motors_port_run_for_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_run_for_at_speed.svg')} alt="block_hubs_all_motors_port_run_for_at_speed.svg" />
Suorittaa moottoria annetun ajan määrän tietyllä nopeudella.

- Yksiköt: `kierrokset`, `asteet`, `sekunnit`
- Huom: vaatii encoder-tuetun moottorin.

### `Aseta moottorin nopeus` (Edistynyt) {#block_hubs_all_motors_port_set_motor_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_speed.svg')} alt="block_hubs_all_motors_port_set_motor_speed.svg" />
Asettaa nopeuden, jota muut moottorilohkot käyttävät.

## Asema ja liike

### `Siirry sijaintiin` (Edistynyt) {#block_hubs_all_motors_port_go_to_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_position.svg')} alt="block_hubs_all_motors_port_go_to_position.svg" />
Siirtää moottorin absoluuttiseen sijaintiin.

- Polkuvaihtoehdot: `lyhin reitti`, `myötäpäivään`, `vastapäivään`
- Huom: vaatii encoder-tuetun moottorin.

### `Siirry suhteelliseen sijaintiin` (Aloittelija) {#block_hubs_all_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_go_to_relative_position.svg')} alt="block_hubs_all_motors_port_go_to_relative_position.svg" />
Siirtää moottoria suhteellisella siirtymällä.

- Huom: vaatii encoder-tuetun moottorin.

### `BuWizz 3 siirry suhteelliseen sijaintiin` (Aloittelija) {#block_hubs_buwizz3_motors_port_go_to_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_motors_port_go_to_relative_position.svg')} alt="block_hubs_buwizz3_motors_port_go_to_relative_position.svg" />
BuWizz 3 -versio suhteellisesta liikkeestä.

- Huom: vaatii encoder-tuetun moottorin.

### `Aseta suhteellinen sijainti` (Aloittelija) {#block_hubs_all_motors_port_set_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_relative_position.svg')} alt="block_hubs_all_motors_port_set_relative_position.svg" />
Asettaa suhteellisen sijainnin nollapisteen.

- Huom: vaatii encoder-tuetun moottorin.

### `Kalibroi ohjaustanko` (Aloittelija) {#block_hubs_all_motors_port_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_calibrate_steering_rack.svg')} alt="block_hubs_all_motors_port_calibrate_steering_rack.svg" />
Kalibroi ohjauksen nollapisteen.

- Vaatimus: moottorin tulee tukea kulman mittausta (encoder).
- Mekaaninen vaatimus: liikealueen tulee olla rajoitettu.
- Toiminta: mittaa liikealueen ja laskee kalibroinnin.
- Tuloste: tallentaa tulokset muuttujille.

## Säätö ja turvallisuus

### `Aseta moottorin pysäytyskäyttäytyminen` (Guru) {#block_hubs_all_motors_port_set_motor_to_at_stop}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motor_to_at_stop.svg')} alt="block_hubs_all_motors_port_set_motor_to_at_stop.svg" />
Asettaa pysäytystilan.

- Vaihtoehdot: `jarru`, `pidä`, `vapaa`
- Huom: vaatii encoder-tuetun moottorin.

### `Aseta jumituksen tunnistus` (Guru) {#block_hubs_all_motors_port_set_motors_stall_detection}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_motors_stall_detection.svg')} alt="block_hubs_all_motors_port_set_motors_stall_detection.svg" />
Ottaa käyttöön tai poistaa jumituksen tunnistuksen.

- Huom: vain MINDSTORMS Robot Inventor.

### `Aseta kiihtyvyys` (Guru) {#block_hubs_all_motors_port_set_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_acceleration.svg')} alt="block_hubs_all_motors_port_set_acceleration.svg" />
Asettaa kiihtyvyysprofiilin.

- Vaihtoehdot: `oletus`, `nopea`, `tasapainoinen`, `pehmeä`, `hidas`, `erittäin hidas`

### `Aseta hidastuvuus` (Guru) {#block_hubs_all_motors_port_set_deceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_set_deceleration.svg')} alt="block_hubs_all_motors_port_set_deceleration.svg" />
Asettaa hidastuvuusprofiilin.

- Vaihtoehdot: `oletus`, `nopea`, `tasapainoinen`, `pehmeä`, `hidas`, `erittäin hidas`

## Moottorin arvolohkot

### `Sijainti` (Aloittelija) {#block_hubs_all_motors_port_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_position.svg')} alt="block_hubs_all_motors_port_position.svg" />
Palauttaa moottorin sijainnin.

### `Suhteellinen sijainti` (Aloittelija) {#block_hubs_all_motors_port_relative_position}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_relative_position.svg')} alt="block_hubs_all_motors_port_relative_position.svg" />
Palauttaa suhteellisen sijainnin.

### `Nopeus` (Aloittelija) {#block_hubs_all_motors_port_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_speed.svg')} alt="block_hubs_all_motors_port_speed.svg" />
Palauttaa nopeuden.

### `Teho` (Edistynyt) {#block_hubs_all_motors_port_power}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_power.svg')} alt="block_hubs_all_motors_port_power.svg" />
Palauttaa tehon.

- Huom: vain MINDSTORMS Robot Inventor.

## Technic Move -moottorilohkot

### `Käynnistä moottorit nopeudella` (Aloittelija) {#block_hubs_technicmove_motors_start_motors_at_speed}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_start_motors_at_speed.svg')} alt="block_hubs_technicmove_motors_start_motors_at_speed.svg" />
Käynnistää ajomoottorit.

### `Tehopulssi` (Aloittelija) {#block_hubs_technicmove_motors_power_pulse}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="block_hubs_technicmove_motors_power_pulse.svg" />
Lähettää tehopulssikomennon valitulle Technic Move Hubille.

- Käytettävissä vain Technic Move Hubille.
- Tyypillinen käyttö: tehosta tai herätä Technic Move -ajojärjestelmä hetkeksi ennen seuraavia lohkoja.

### `Pysäytä moottorit` (Aloittelija) {#block_hubs_technicmove_motors_stop_motors}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_stop_motors.svg')} alt="block_hubs_technicmove_motors_stop_motors.svg" />
Pysäyttää moottorit.

### `Jarru` (Aloittelija) {#block_hubs_technicmove_motors_brake}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_brake.svg')} alt="block_hubs_technicmove_motors_brake.svg" />
Asettaa jarrun.

- Vaihtoehdot: `pois`, `päällä`

### `Aseta ohjaus` (Aloittelija) {#block_hubs_technicmove_motors_set_steering_rack_to}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_set_steering_rack_to.svg')} alt="block_hubs_technicmove_motors_set_steering_rack_to.svg" />
Asettaa ohjauksen arvon.

### `Kalibroi ohjaus` (Aloittelija) {#block_hubs_technicmove_motors_calibrate_steering_rack}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_calibrate_steering_rack.svg')} alt="block_hubs_technicmove_motors_calibrate_steering_rack.svg" />
Kalibroi ohjauksen.