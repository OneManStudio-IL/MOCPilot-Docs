---
id: AboutApp
title: O MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Postavte to. Šoférujte to. Ovládajte všetko.

**MOCPilot** je aplikácia na vytváranie vlastných ovládacích profilov pre LEGO® a kompatibilné Bluetooth modely s pohonom.

Dáva staviteľom jedno miesto na pripojenie hubov, ovládanie motorov, čítanie senzorov, návrh panelov a tvorbu vizuálnych programov pre modely, mechanizmy, autá, nákladné autá, vlaky, roboty a vlastné MOC.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="Aplikácia MOCPilot spustená v telefóne" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Čo MOCPilot ponúka</h2>
    <ul>
      <li>Vlastné profily pre vaše modely.</li>
      <li>Hotové profily pre podporované oficiálne sety.</li>
      <li>Pripojenie a správa Bluetooth hubov.</li>
      <li>Vizuálne programovanie blokmi pre automatizáciu a logiku.</li>
      <li>Ovládacie prvky panelu na jazdu a obsluhu modelov.</li>
      <li>Podpora LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motorov, senzorov a kompatibilných Bluetooth zariadení.</li>
    </ul>
  </div>
</div>

## Myšlienka

Väčšina motorizovaných stavieb potrebuje viac než jednoduchý ovládač. Auto môže potrebovať riadenie, plyn, svetlá, sledovanie batérie, sekvenciu prevodovky alebo špeciálnu štartovaciu rutinu. Robot môže potrebovať senzory, udalosti, podmienenú logiku a viac hubov pracujúcich spolu.

MOCPilot je navrhnutý pre priestor medzi jednoduchým diaľkovým ovládaním a plnohodnotným programovacím prostredím. Môžete začať jazdou z obrazovkového panelu a neskôr pridať logiku, senzory a automatizáciu.

## Profily

**Profil** je riadiace centrum jedného modelu.

V profile môžete zvoliť huby patriace k modelu, vytvoriť program, ktorý model spúšťa, a navrhnúť ovládací panel.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="Stránka profilov MOCPilot" width="420" />

<details>
<summary>Predpripravené profily</summary>

Predpripravené profily sú hotové príklady pre podporované oficiálne sety. Sú užitočné na rýchly štart alebo na štúdium toho, ako je zostavený funkčný profil.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Predpripravené profily MOCPilot" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Predpripravený blokový program MOCPilot" width="1100" />

</details>

<details>
<summary>Vlastné profily</summary>

Vlastné profily sú určené pre vaše MOC a experimenty. Môžete vytvoriť profil, pridať huby, pripojiť motory a senzory, zostaviť program a navrhnúť panel presne pre daný model.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Vytvorenie vlastného profilu MOCPilot" width="420" />

</details>

## Pripojenie hubov a zariadení

MOCPilot sa môže pripojiť k podporovaným Bluetooth hubom a kompatibilným zariadeniam a sprístupniť ich v profile.

Pre jednoduchú stavbu môžete použiť jeden hub alebo pripojiť viac hubov, keď model potrebuje viac portov, samostatné napájanie alebo nezávislé moduly.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Stránka Moje Bluetooth huby v MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Pripojené Bluetooth huby v MOCPilot" width="1100" />

<details>
<summary>Príklady podporovaného hardvéru</summary>

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(140px, 1fr))', gap: '16px', alignItems: 'end', margin: '16px 0'}}>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_hub_p.webp')} alt="LEGO Technic Hub" style={{maxWidth: '130px'}} />
    <div><strong>Technic Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_move_hub_p.webp')} alt="LEGO Technic Move Hub" style={{maxWidth: '130px'}} />
    <div><strong>Technic Move Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/buwizz3_hub_p.webp')} alt="BuWizz 3.0 Pro Hub" style={{maxWidth: '130px'}} />
    <div><strong>BuWizz 3.0</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/sbrick_hub_p.webp')} alt="SBrick Hub" style={{maxWidth: '130px'}} />
    <div><strong>SBrick</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/mould_king_4_p.webp')} alt="Mould King Hub" style={{maxWidth: '130px'}} />
    <div><strong>Mould King</strong></div>
  </div>
</div>

Úplný zoznam nájdete na stránke [podporované huby, motory a senzory](/docs/Introducing/SupportedDevices/).

</details>

## Tvorba logiky pomocou blokov

MOCPilot obsahuje vizuálny tvorca blokov. Programy môžete vytvárať spájaním blokov namiesto písania kódu.

Bloky môžu reagovať na udalosti, ovládať motory, čítať senzory, pracovať s premennými, používať vstup z gamepadu, aktualizovať ovládače panelu a koordinovať viac akcií.

MOCPilot plne podporuje pripojené fyzické gamepady. Bloky gamepadu čítajú tlačidlá, spúšte, smery D-padu a páčky, takže môžete priradiť skutočný ovládač k modelu, keď je fyzické ovládanie lepšie než dotyková obrazovka.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="Používateľský program MOCPilot zostavený z blokov" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Blok pri spustení programu" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Blok spustenia motora rýchlosťou" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Blok úrovne batérie hubu" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Blok hodnoty volantu" />
</div>

<details>
<summary>Čo možno robiť blokovými programami</summary>

- Spúšťať, zastavovať a riadiť motory.
- Čítať úroveň batérie, napätie, náklon, orientáciu, teplotu a hodnoty senzorov.
- Nastaviť fyzický gamepad pre riadenie, plyn, spúšte, akcie a prepínanie režimov.
- Reagovať na zmeny tlačidiel, senzorov, časovačov alebo ovládacích prvkov panelu.
- Vytvoriť štartovacie kontroly pred pohybom modelu.
- Pridať vlastnú logiku pre svetlá, kalibráciu riadenia, režimy výkonu a konfiguráciu hubu.
- Používať premenné, zoznamy, podmienky, slučky, správy a vlastné bloky na zložité správanie.

</details>

## Návrh jazdného panelu

Ovládací panel je obrazovka používaná pri riadení modelu. Môže obsahovať volanty, joysticky, posuvníky, tlačidlá, prepínače, pedále, monitory a ďalšie ovládače.

Ovládacie prvky panelu a vstupy fyzického gamepadu môžete prepojiť s blokmi a akciami hubu, aby rozhranie zodpovedalo modelu.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="Ovládacie prvky panelu MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="Ovládacia obrazovka MOCPilot s volantom a pedálmi" width="1100" />

<details>
<summary>Príklady panelov</summary>

- Použite volant a pedále pre autá.
- Použite posuvníky pre žeriavy, zdviháky a lineárne aktuátory.
- Použite tlačidlá pre svetlá, klaksón, radenie alebo skriptované akcie.
- Použite monitory na zobrazenie batérie, rýchlosti, hodnôt senzorov alebo vlastného stavu programu.
- Použite pripojený gamepad, ak uprednostňujete fyzické tlačidlá, páčky a spúšte.

</details>

## Udržte pokročilé stavby zvládnuteľné

Ako model rastie, môže rásť aj profil. MOCPilot podporuje znovupoužiteľnú logiku pomocou **My Blocks**, nastavenie hubov pre konkrétny profil, viac ovládačov a programové toky kombinujúce manuálne ovládanie s automatizáciou.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Príklad použitia My Blocks v MOCPilot" width="1100" />

Pomáha to udržať veľké programy čitateľné. Profil môže mať napríklad vlastný blok na aktualizáciu batérie, ďalší na kalibráciu riadenia a ďalší na špeciálny jazdný režim.

## Typický postup

1. Vytvorte alebo otvorte profil.
2. Pridajte Bluetooth huby a zariadenia používané modelom.
3. Zostavte program z blokov.
4. Navrhnite panel na jazdu a interakciu.
5. Stlačte **Play**.
6. Testujte, dolaďujte a zlepšujte profil, kým sa model nespráva podľa vašich predstáv.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Postup pripojenia hubu v MOCPilot" width="1100" />

## Pre koho je MOCPilot

MOCPilot je užitočný pre staviteľov, ktorí chcú:

- Lepšie diaľkové ovládanie pre motorizované LEGO® modely.
- Spôsob ovládania kompatibilných Bluetooth hubov tretích strán.
- Vizuálne programovacie prostredie pre mechanizmy a roboty.
- Predpripravené profily pre podporované oficiálne sety.
- Vlastné panely pre autá, nákladné autá, vlaky, crawlery, žeriavy a ďalšie MOC.
- Jednu aplikáciu kombinujúcu huby, motory, senzory, gamepady a ovládanie na obrazovke.

## Začnite objavovať

- Postupujte podľa [rýchleho úvodu](/docs/Introducing/QuickStart/) a vytvorte prvý profil.
- Pred výberom hardvéru skontrolujte [podporované zariadenia](/docs/Introducing/SupportedDevices/).
- Keď budete pripravení pridať logiku, prezrite si [dokumentáciu BlockBuilder](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/).
- Ak hub vyžaduje podporovanú verziu firmvéru, pozrite si [aktualizáciu firmvéru hubu](/docs/Application/Hubs/FirmwareUpdating/).
