---
id: AboutApp
title: Om MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Byg det. Kør det. Styr alt.

**MOCPilot** er en app til at oprette brugerdefinerede kontrolprofiler til LEGO® og kompatible Bluetooth-drevne modeller.

Den giver byggere ét sted til at forbinde hubs, styre motorer, læse sensorer, designe dashboards og oprette visuelle programmer til modeller, mekanismer, biler, lastbiler, tog, robotter og egne MOC’er.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="MOCPilot-appen på en telefon" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Hvad MOCPilot giver dig</h2>
    <ul>
      <li>Brugerdefinerede profiler til dine egne modeller.</li>
      <li>Klar-til-brug profiler til understøttede officielle sæt.</li>
      <li>Forbindelse og styring af Bluetooth-hubs.</li>
      <li>Visuel blokprogrammering til automatisering og logik.</li>
      <li>Dashboardkontroller til at køre og betjene modeller.</li>
      <li>Understøttelse af LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motorer, sensorer og kompatible Bluetooth-enheder.</li>
    </ul>
  </div>
</div>

## Idéen

De fleste motoriserede byggerier kræver mere end en simpel fjernbetjening. En bil kan have brug for styring, gas, lys, batteriovervågning, gearsekvens eller en særlig startrutine. En robot kan have brug for sensorer, hændelser, betinget logik og flere hubs, der arbejder sammen.

MOCPilot er designet til området mellem en enkel fjernbetjening og et fuldt programmeringsmiljø. Du kan starte med at køre en model fra et dashboard på skærmen og senere tilføje logik, sensorer og automatisering.

## Profiler

En **profil** er kontrolcenteret for én model.

I en profil kan du vælge, hvilke hubs der hører til modellen, oprette programmet der kører modellen, og designe dashboardet til styring.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="MOCPilot-profilsiden" width="420" />

<details>
<summary>Forudbyggede profiler</summary>

Forudbyggede profiler er færdige eksempler til understøttede officielle sæt. De er nyttige, når du vil hurtigt i gang eller se, hvordan en fungerende profil er sat sammen.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Forudbyggede MOCPilot-profiler" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Forudbygget MOCPilot-blokprogram" width="1100" />

</details>

<details>
<summary>Brugerdefinerede profiler</summary>

Brugerdefinerede profiler er til dine egne MOC’er og eksperimenter. Du kan oprette en profil, tilføje hubs, forbinde motorer og sensorer, bygge et program og designe et kontrol-dashboard, der passer til modellen.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Opret en brugerdefineret MOCPilot-profil" width="420" />

</details>

## Forbind hubs og enheder

MOCPilot kan forbinde til understøttede Bluetooth-hubs og kompatible enheder og gøre dem tilgængelige i din profil.

Du kan bruge én hub til en enkel model eller forbinde flere hubs, når modellen kræver flere porte, separate strømsystemer eller uafhængige moduler.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Mine Bluetooth-hubs-siden i MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Forbundne Bluetooth-hubs i MOCPilot" width="1100" />

<details>
<summary>Eksempler på understøttet hardware</summary>

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

Se siden med [understøttede hubs, motorer og sensorer](/docs/Introducing/SupportedDevices/) for hele listen.

</details>

## Byg logik med blokke

MOCPilot indeholder en visuel blokbygger. Du kan oprette programmer ved at forbinde blokke i stedet for at skrive kode.

Blokke kan reagere på hændelser, styre motorer, læse sensorer, arbejde med variabler, bruge gamepad-input, opdatere dashboardkontroller og koordinere flere handlinger.

MOCPilot understøtter fuldt ud tilsluttede fysiske gamepads. Gamepad-blokke kan læse knapper, triggere, D-pad-retninger og sticks, så du kan mappe en rigtig controller til modellen, når fysisk kontrol er bedre end touchskærmen.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="MOCPilot-brugerprogram bygget med blokke" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Blok når programmet starter" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Blok start motor med hastighed" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Blok for hub-batteriniveau" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Blok for ratværdi" />
</div>

<details>
<summary>Hvad du kan gøre med blokprogrammer</summary>

- Starte, stoppe og styre motorer.
- Læse batteriniveau, spænding, hældning, orientering, temperatur og sensorværdier.
- Konfigurere fysisk gamepadstyring til styring, gas, triggere, handlinger og tilstandsskift.
- Reagere når knapper, sensorer, timere eller dashboardkontroller ændres.
- Oprette startkontroller før modellen bevæger sig.
- Tilføje egen logik til lys, styrekalibrering, powertilstande og hub-konfiguration.
- Bruge variabler, lister, betingelser, løkker, broadcasts og egne blokke til kompleks adfærd.

</details>

## Design et køredashboard

Dashboardet er skærmen, du bruger, mens du styrer modellen. Det kan indeholde rat, joysticks, skydere, knapper, kontakter, pedaler, monitorer og andre kontroller.

Du kan forbinde dashboardkontroller og fysisk gamepad-input til blokke og hub-handlinger, så grænsefladen passer til modellen.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="MOCPilot-dashboardkontroller" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="MOCPilot-kontrolskærm med rat og pedaler" width="1100" />

<details>
<summary>Dashboardeksempler</summary>

- Brug rat og pedaler til biler.
- Brug skydere til kraner, lifte og lineære aktuatorer.
- Brug knapper til lys, horn, gearskift eller scriptede handlinger.
- Brug monitorer til batteri, hastighed, sensorværdier eller egen programtilstand.
- Brug en tilsluttet gamepad, hvis du foretrækker fysiske knapper, sticks og triggere.

</details>

## Hold avancerede byggerier overskuelige

Når en model vokser, kan profilen vokse med den. MOCPilot understøtter genbrugelig logik med **My Blocks**, profilspecifik hubopsætning, flere kontroller og programflows, der kombinerer manuel styring med automatisering.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Eksempel på brug af My Blocks i MOCPilot" width="1100" />

Det hjælper med at holde store programmer læsbare. En profil kan f.eks. have en egen blok til batteriopdateringer, en anden til styrekalibrering og en tredje til en særlig køretilstand.

## Typisk arbejdsgang

1. Opret eller åbn en profil.
2. Tilføj Bluetooth-hubs og enheder, som modellen bruger.
3. Byg programmet med blokke.
4. Design et dashboard til kørsel og interaktion.
5. Tryk på **Play**.
6. Test, justér og forbedr profilen, indtil modellen opfører sig som ønsket.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Flow for hubforbindelse i MOCPilot" width="1100" />

## Hvem MOCPilot er til

MOCPilot er nyttig for byggere, der ønsker:

- En bedre fjernbetjening til motoriserede LEGO® modeller.
- En måde at styre kompatible tredjeparts Bluetooth-hubs.
- Et visuelt programmeringsmiljø til mekanismer og robotter.
- Forudbyggede profiler til understøttede officielle sæt.
- Egne dashboards til biler, lastbiler, tog, crawlere, kraner og andre MOC’er.
- Én app, der kombinerer hubs, motorer, sensorer, gamepads og skærmkontroller.

## Begynd at udforske

- Følg [hurtigstartvejledningen](/docs/Introducing/QuickStart/) for at bygge din første profil.
- Tjek [understøttede enheder](/docs/Introducing/SupportedDevices/), før du vælger hardware.
- Udforsk [BlockBuilder-dokumentationen](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/), når du er klar til at tilføje logik.
- Se [opdatering af hub-firmware](/docs/Application/Hubs/FirmwareUpdating/), hvis en hub kræver en understøttet firmwareversion.
