---
id: Sensors
title: Senzory
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Senzory

Bloky senzorů čtou stav hubu/zařízení a poskytují data pro podmínky, události a řídicí logiku.

## Senzory zařízení a hubu

### `Úroveň baterie hubu` (Začátečník) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Vrací aktuální úroveň baterie hubu.

### `Napětí baterie hubu` (Pokročilý) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Vrací napětí baterie vybraného hubu ve voltech.

- Typ: číselný reportovací blok
- Dostupné pouze pro huby, které hlásí napětí baterie.
- Když vybraný hub není připojen, vrací `NaN`.

### `Baterie zařízení %` (Začátečník) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Vrací aktuální úroveň baterie telefonu/tabletu, na kterém běží MOCPilot (v procentech).

### `Teplota desky` (Pokročilý) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Vrací teplotu desky hubu.

- Dostupné pouze pro `BuWizz 2` a `BuWizz 3`.

### `Akcelerometr hubu` (Guru) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Vrací surová data akcelerometru hlášená vybraným hubem.

- Osy: `x`, `y`, `z`

### `Zrychlení hubu` (Guru) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Vrací data zrychlení hlášená vybraným hubem.

- Osy: `x`, `y`, `z`

### `Tlačítko stisknuto` (Začátečník) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Kontroluje, zda vybrané tlačítko hubu odpovídá vybranému stavu.

- Možnosti stavu: `stisknuto`, `uvolněno`
- Typická možnost tlačítka: `střed` (závisí na hubu)

- Poznámka: dostupné možnosti tlačítek se mohou lišit podle modelu hubu.

### `Typ zařízení` (Začátečník) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Vrací typ připojeného zařízení pro vybraný port.

- Typ: reportovací blok
- Typické použití: zjistit, jaké zařízení je připojeno, před spuštěním logiky specifické pro zařízení

### `Akcelerometr zařízení` (Guru) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Vrací surové hodnoty akcelerometru ze senzorů zařízení.

- Možnosti osy: `x`, `y`, `z`

### `Zrychlení zařízení` (Guru) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Vrací data zrychlení ze senzorů zařízení.

- Možnosti osy: `x`, `y`, `z`

## Senzory orientace a náklonu

### `Náklon zařízení` (Pokročilý) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Vrací data náklonu z telefonu/tabletu, na kterém běží MOCPilot.

- Osy: `pitch`, `roll`

### `Náklon` (Začátečník) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Vrací úhel náklonu pro vybranou osu.

- Možnosti osy: `náklon`, `rotace`, `kormidlování`
- Poznámka: `kormidlování` je dostupné jen na hubech, které tuto hodnotu poskytují.

### `Získat orientaci` (Začátečník) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Vrací aktuální stav orientace hubu.

- Možnosti formátu výstupu: `text`, `index`
- Hodnoty orientace: `Přední`, `Horní`, `Vpravo`, `Zpět`, `Dno`, `Vlevo`

### `Je orientace nahoru` (Začátečník) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Kontroluje, zda orientace hubu odpovídá vybrané orientaci „nahoru“.

- Možnosti orientace: `Přední`, `Horní`, `Vpravo`, `Zpět`, `Dno`, `Vlevo`

### `Nastavit orientaci náklonu` (Pokročilý) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Nastaví referenční orientaci používanou bloky náklonu/orientace.

- Možnosti orientace: `Přední`, `Horní`, `Vpravo`, `Zpět`, `Dno`, `Vlevo`

## Časovač a pohybové senzory zařízení

### `Časovač` (Pokročilý) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Vrací hodnotu časovače v sekundách.

### `Resetovat časovač` (Pokročilý) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Resetuje časovač na nulu.

## Bloky senzorů na portech

### `Senzor vzdálenosti Technic` (Začátečník) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Vrací hodnoty vzdálenosti ze senzoru vzdálenosti Technic.

- Možnosti jednotek: `mm`, `cm`, `palce`, `%`

### `Technic když je vzdálenost` (Začátečník) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Spouští/kontroluje podmínku vzdálenosti pro senzor vzdálenosti Technic.

- Možnosti porovnání: `blíže než`, `dál než`, `přesně na`
- Možnosti jednotek: `mm`, `cm`, `palce`, `%`

### `Technic nastavit režim barevného senzoru` (Pokročilý) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Tento blok nastaví barevný senzor Technic do zvoleného režimu.

- Poznámka: Změna režimu barevného senzoru může ovlivnit váš program neočekávaným způsobem. Například barevný senzor Technic nemůže číst barvy ani odražené světlo, když je v režimu `"okolní"`.

### `Hodnota barvy senzoru Technic` (Začátečník) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Vrací zjištěnou hodnotu barvy ze senzoru Technic.

- Možnosti výstupu: `hodnota`, `řetězec`

### `Technic když je barva` (Začátečník) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Spouští/kontroluje, když zjištěná barva odpovídá vybrané barvě.

### `Odražené světlo Technic` (Začátečník) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Vrací intenzitu odraženého světla.

### `Technic když je odražené světlo` (Začátečník) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Spouští/kontroluje prahovou podmínku odraženého světla.

- Možnosti porovnání: `<`, `=`, `>`

### `Okolní světlo Technic` (Začátečník) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Vrací intenzitu okolního světla.

### `Technic když je okolní světlo` (Začátečník) {#block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg" />
Spouští/kontroluje prahovou podmínku okolního světla.

- Možnosti porovnání: `<`, `=`, `>`

### `Surová barva Technic` (Začátečník) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Vrací surovou hodnotu barevného kanálu ze senzoru Technic.

- Možnosti kanálu: `červený`, `zelený`, `modrý`

### `Vzdálenost senzoru BOOST` (Začátečník) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Vrací vzdálenost ze senzoru vzdálenosti BOOST.

- Možnosti jednotek: `%`, `cm`, `palce`

### `BOOST když je vzdálenost` (Začátečník) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Spouští/kontroluje podmínku vzdálenosti pro senzor vzdálenosti BOOST.

- Možnosti porovnání: `blíže než`, `dál než`, `přesně na`
- Možnosti jednotek: `%`, `cm`, `palce`

### `Barva senzoru BOOST` (Začátečník) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Vrací barvu detekovanou senzorem BOOST.

- Možnosti výstupu: `hodnota`, `řetězec`

### `BOOST je barva` (Začátečník) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Kontroluje, zda senzor BOOST aktuálně detekuje vybranou barvu.

### `Odražené světlo BOOST` (Začátečník) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Vrací hodnotu odraženého světla ze senzoru BOOST.

### `BOOST když je odražené světlo` (Začátečník) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Spouští/kontroluje prahovou podmínku odraženého světla pro senzor BOOST.

- Možnosti porovnání: `<`, `=`, `>`

### `Technic Move nastavit režim výkonu` (Začátečník) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Nastaví režim výkonu Technic Move.

- Možnosti režimu: `normální`, `turbo`

### `Výstupní napětí BuWizz` (Guru) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Vrací aktuální výstupní napětí hlášené hubem BuWizz.

- Dostupné pouze pro podporované huby BuWizz.

### `Proud portu BuWizz` (Guru) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Vrací proudový odběr hlášený pro vybraný port hubu BuWizz.

- Dostupné pouze pro podporované huby a porty BuWizz.

### `Vzdálenost WeDo 2` (Začátečník) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Vrací vzdálenost ze senzoru vzdálenosti WeDo 2.

- Možnosti jednotek: `%`, `cm`, `palce`

### `WeDo 2 když je vzdálenost` (Začátečník) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Spouští/kontroluje podmínku vzdálenosti pro senzor vzdálenosti WeDo 2.

- Možnosti porovnání: `closer than`, `farther than`, `exactly at`
- Jednotky: `%`, `cm`, `inch`

### `Náklon WeDo 2` (Začátečník) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Vrací hodnotu náklonu ze senzoru náklonu WeDo 2.

- Možnosti osy: `náklon`, `rotace`