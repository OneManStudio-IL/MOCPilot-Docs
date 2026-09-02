---
id: AboutApp
title: Om MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Bygg det. Kjør det. Kontroller alt.

**MOCPilot** er en app for å lage egne kontrollprofiler for LEGO® og kompatible Bluetooth-drevne modeller.

Den gir byggere ett sted for å koble til huber, styre motorer, lese sensorer, designe dashbord og lage visuelle programmer for modeller, mekanismer, biler, lastebiler, tog, roboter og egne MOC-er.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="MOCPilot-appen på en telefon" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Hva MOCPilot gir deg</h2>
    <ul>
      <li>Egne profiler for dine egne modeller.</li>
      <li>Ferdige profiler for støttede offisielle sett.</li>
      <li>Tilkobling og administrasjon av Bluetooth-huber.</li>
      <li>Visuell blokkprogrammering for automatisering og logikk.</li>
      <li>Dashbordkontroller for kjøring og betjening av modeller.</li>
      <li>Støtte for LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motorer, sensorer og kompatible Bluetooth-enheter.</li>
    </ul>
  </div>
</div>

## Ideen

De fleste motoriserte bygg trenger mer enn en enkel fjernkontroll. En bil kan trenge styring, gass, lys, batteriovervåking, girsekvens eller en spesiell startrutine. En robot kan trenge sensorer, hendelser, betinget logikk og flere huber som jobber sammen.

MOCPilot er laget for området mellom en enkel fjernkontroll og et fullverdig programmeringsmiljø. Du kan starte med å kjøre en modell fra et skjermdashbord og senere legge til logikk, sensorer og automatisering.

## Profiler

En **profil** er kontrollsenteret for én modell.

I en profil kan du velge hvilke huber som hører til modellen, lage programmet som kjører modellen, og designe dashbordet som brukes til å styre den.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="MOCPilot-profilsiden" width="420" />

<details>
<summary>Forhåndsbygde profiler</summary>

Forhåndsbygde profiler er ferdige eksempler for støttede offisielle sett. De er nyttige når du vil komme raskt i gang eller studere hvordan en fungerende profil er satt sammen.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Forhåndsbygde MOCPilot-profiler" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Forhåndsbygd MOCPilot-blokkprogram" width="1100" />

</details>

<details>
<summary>Egne profiler</summary>

Egne profiler er for dine egne MOC-er og eksperimenter. Du kan lage en profil, legge til huber, koble motorer og sensorer, bygge et program og designe et kontrolldashbord som passer modellen.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Lag en egen MOCPilot-profil" width="420" />

</details>

## Koble til huber og enheter

MOCPilot kan koble til støttede Bluetooth-huber og kompatible enheter og gjøre dem tilgjengelige i profilen din.

Du kan bruke én hub for et enkelt bygg eller koble til flere huber når modellen trenger flere porter, separate strømsystemer eller uavhengige moduler.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Mine Bluetooth-huber-siden i MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Tilkoblede Bluetooth-huber i MOCPilot" width="1100" />

<details>
<summary>Eksempler på støttet maskinvare</summary>

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

Se siden med [støttede huber, motorer og sensorer](/docs/Introducing/SupportedDevices/) for hele listen.

</details>

## Bygg logikk med blokker

MOCPilot inkluderer en visuell blokkbygger. Du kan lage programmer ved å koble sammen blokker i stedet for å skrive kode.

Blokker kan reagere på hendelser, styre motorer, lese sensorer, jobbe med variabler, bruke gamepad-inndata, oppdatere dashbordkontroller og koordinere flere handlinger.

MOCPilot støtter tilkoblede fysiske gamepader fullt ut. Gamepad-blokker lar deg lese knapper, triggere, D-pad-retninger og styrespaker, slik at du kan bruke en ekte kontroller med modellen når fysisk kontroll er bedre enn berøringsskjerm.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="MOCPilot-brukerprogram bygget med blokker" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Blokk når programmet starter" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Blokk start motor med hastighet" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Blokk for hubens batterinivå" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Blokk for rattverdi" />
</div>

<details>
<summary>Hva du kan gjøre med blokkprogrammer</summary>

- Starte, stoppe og styre motorer.
- Lese batterinivå, spenning, helling, orientering, temperatur og sensorverdier.
- Konfigurere fysisk gamepadkontroll for styring, gass, triggere, handlinger og modusbytte.
- Reagere når knapper, sensorer, timere eller dashbordkontroller endres.
- Lage startkontroller før modellen begynner å bevege seg.
- Legge til egen logikk for lys, styrekalibrering, effektmoduser og hubkonfigurasjon.
- Bruke variabler, lister, betingelser, løkker, kringkastinger og egne blokker for å organisere kompleks oppførsel.

</details>

## Design et kjøredashbord

Dashbordet er skjermen du bruker når du styrer modellen. Det kan inneholde ratt, joysticker, skyveknapper, knapper, brytere, pedaler, monitorer og andre kontroller.

Du kan koble dashbordkontroller og fysisk gamepad-inndata til blokker og hubhandlinger, slik at grensesnittet passer modellen.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="MOCPilot-dashbordkontroller" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="MOCPilot-kontrollskjerm med ratt og pedaler" width="1100" />

<details>
<summary>Dashbordeksempler</summary>

- Bruk ratt og pedaler for biler.
- Bruk skyveknapper for kraner, lifter og lineære aktuatorer.
- Bruk knapper for lys, horn, girskift eller skriptede handlinger.
- Bruk monitorer for å vise batteri, hastighet, sensorverdier eller egen programtilstand.
- Bruk en tilkoblet gamepad hvis du foretrekker fysiske knapper, spaker og triggere.

</details>

## Hold avanserte bygg håndterlige

Når en modell vokser, kan profilen vokse med den. MOCPilot støtter gjenbrukbar logikk med **My Blocks**, profilspesifikt huboppsett, flere kontroller og programflyter som kombinerer manuell styring med automatisering.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Eksempel på bruk av My Blocks i MOCPilot" width="1100" />

Dette hjelper med å holde store programmer lesbare. En profil kan for eksempel ha én egen blokk for batterioppdateringer, en annen for styrekalibrering og en tredje for en spesiell kjøremodus.

## Typisk arbeidsflyt

1. Opprett eller åpne en profil.
2. Legg til Bluetooth-hubene og enhetene modellen bruker.
3. Bygg programmet med blokker.
4. Design et dashbord for kjøring og interaksjon.
5. Trykk **Play**.
6. Test, juster og forbedre profilen til modellen oppfører seg slik du ønsker.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Flyt for hubtilkobling i MOCPilot" width="1100" />

## Hvem MOCPilot er for

MOCPilot er nyttig for byggere som vil ha:

- En bedre fjernkontroll for motoriserte LEGO®-modeller.
- En måte å kontrollere tredjeparts kompatible Bluetooth-huber på.
- Et visuelt programmeringsmiljø for mekanismer og roboter.
- Forhåndsbygde profiler for støttede offisielle sett.
- Egne dashbord for biler, lastebiler, tog, crawlere, kraner og andre MOC-er.
- Én app som kombinerer huber, motorer, sensorer, gamepader og skjermkontroller.

## Begynn å utforske

- Følg [hurtigstartveiledningen](/docs/Introducing/QuickStart/) for å bygge din første profil.
- Sjekk [støttede enheter](/docs/Introducing/SupportedDevices/) før du velger maskinvare.
- Utforsk [BlockBuilder-dokumentasjonen](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/) når du er klar til å legge til logikk.
- Se [oppdatering av hub-firmware](/docs/Application/Hubs/FirmwareUpdating/) hvis en hub krever en støttet firmwareversjon.
