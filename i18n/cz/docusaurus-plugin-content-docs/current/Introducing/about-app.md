---
id: AboutApp
title: O MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Postavte to. Řiďte to. Ovládejte vše.

**MOCPilot** je aplikace pro vytváření vlastních ovládacích profilů pro LEGO® a kompatibilní Bluetooth modely s pohonem.

Dává stavitelům jedno místo pro připojení hubů, ovládání motorů, čtení senzorů, návrh ovládacích panelů a tvorbu vizuálních programů pro modely, mechanismy, auta, nákladní vozy, vlaky, roboty a vlastní MOC.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="Aplikace MOCPilot spuštěná v telefonu" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Co MOCPilot nabízí</h2>
    <ul>
      <li>Vlastní profily pro vaše modely.</li>
      <li>Hotové profily pro podporované oficiální sady.</li>
      <li>Připojení a správa Bluetooth hubů.</li>
      <li>Vizuální programování bloky pro automatizaci a logiku.</li>
      <li>Ovládací prvky panelu pro řízení a obsluhu modelů.</li>
      <li>Podpora LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motorů, senzorů a kompatibilních Bluetooth zařízení.</li>
    </ul>
  </div>
</div>

## Myšlenka

Většina motorizovaných staveb potřebuje víc než jednoduchý ovladač. Auto může potřebovat řízení, plyn, světla, sledování baterie, sekvenci převodovky nebo speciální startovací rutinu. Robot může potřebovat senzory, události, podmíněnou logiku a několik hubů pracujících společně.

MOCPilot je navržen pro prostor mezi základním dálkovým ovládáním a plnohodnotným programovacím prostředím. Můžete začít řízením modelu z obrazovkového panelu a později přidat logiku, senzory a automatizaci.

## Profily

**Profil** je řídicí centrum jednoho modelu.

V profilu můžete zvolit huby patřící k modelu, vytvořit program, který model spouští, a navrhnout ovládací panel.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="Stránka profilů MOCPilot" width="420" />

<details>
<summary>Předpřipravené profily</summary>

Předpřipravené profily jsou hotové příklady pro podporované oficiální sady. Hodí se pro rychlý start nebo pro pochopení, jak je sestaven funkční profil.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Předpřipravené profily MOCPilot" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Předpřipravený blokový program MOCPilot" width="1100" />

</details>

<details>
<summary>Vlastní profily</summary>

Vlastní profily jsou určeny pro vaše MOC a experimenty. Můžete vytvořit profil, přidat huby, připojit motory a senzory, sestavit program a navrhnout panel přesně pro daný model.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Vytvoření vlastního profilu MOCPilot" width="420" />

</details>

## Připojení hubů a zařízení

MOCPilot se může připojit k podporovaným Bluetooth hubům a kompatibilním zařízením a zpřístupnit je v profilu.

Pro jednoduchou stavbu můžete použít jeden hub nebo připojit více hubů, když model potřebuje více portů, oddělené napájení nebo nezávislé moduly.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Stránka Moje Bluetooth huby v MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Připojené Bluetooth huby v MOCPilot" width="1100" />

<details>
<summary>Příklady podporovaného hardwaru</summary>

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

Úplný seznam najdete na stránce [podporované huby, motory a senzory](/docs/Introducing/SupportedDevices/).

</details>

## Tvorba logiky pomocí bloků

MOCPilot obsahuje vizuální tvůrce bloků. Programy můžete vytvářet spojováním bloků místo psaní kódu.

Bloky mohou reagovat na události, ovládat motory, číst senzory, pracovat s proměnnými, používat vstup z gamepadu, aktualizovat ovladače panelu a koordinovat více akcí.

MOCPilot plně podporuje připojené fyzické gamepady. Bloky gamepadu čtou tlačítka, spouště, směry D-padu a páčky, takže můžete přiřadit skutečný ovladač k modelu, když je fyzické ovládání lepší než dotyková obrazovka.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="Uživatelský program MOCPilot sestavený z bloků" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Blok při spuštění programu" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Blok spuštění motoru rychlostí" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Blok úrovně baterie hubu" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Blok hodnoty volantu" />
</div>

<details>
<summary>Co lze dělat blokovými programy</summary>

- Spouštět, zastavovat a řídit motory.
- Číst úroveň baterie, napětí, náklon, orientaci, teplotu a hodnoty senzorů.
- Nastavit fyzický gamepad pro řízení, plyn, spouště, akce a přepínání režimů.
- Reagovat na změny tlačítek, senzorů, časovačů nebo ovládacích prvků panelu.
- Vytvořit startovací kontroly před pohybem modelu.
- Přidat vlastní logiku pro světla, kalibraci řízení, režimy výkonu a konfiguraci hubu.
- Používat proměnné, seznamy, podmínky, smyčky, zprávy a vlastní bloky pro složité chování.

</details>

## Návrh jízdního panelu

Ovládací panel je obrazovka používaná při řízení modelu. Může obsahovat volanty, joysticky, posuvníky, tlačítka, přepínače, pedály, monitory a další ovladače.

Ovládací prvky panelu a vstupy fyzického gamepadu můžete propojit s bloky a akcemi hubu, aby rozhraní odpovídalo modelu.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="Ovládací prvky panelu MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="Ovládací obrazovka MOCPilot s volantem a pedály" width="1100" />

<details>
<summary>Příklady panelů</summary>

- Použijte volant a pedály pro auta.
- Použijte posuvníky pro jeřáby, zvedáky a lineární aktuátory.
- Použijte tlačítka pro světla, klakson, řazení nebo skriptované akce.
- Použijte monitory pro baterii, rychlost, hodnoty senzorů nebo vlastní stav programu.
- Použijte připojený gamepad, pokud dáváte přednost fyzickým tlačítkům, páčkám a spouštím.

</details>

## Udržte pokročilé stavby přehledné

Jak model roste, může růst i profil. MOCPilot podporuje znovupoužitelnou logiku pomocí **My Blocks**, nastavení hubů pro konkrétní profil, více ovladačů a programové toky kombinující ruční ovládání s automatizací.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Příklad použití My Blocks v MOCPilot" width="1100" />

To pomáhá udržet velké programy čitelné. Profil může mít například vlastní blok pro aktualizaci baterie, další pro kalibraci řízení a další pro speciální jízdní režim.

## Typický postup

1. Vytvořte nebo otevřete profil.
2. Přidejte Bluetooth huby a zařízení používaná modelem.
3. Sestavte program z bloků.
4. Navrhněte panel pro řízení a interakci.
5. Stiskněte **Play**.
6. Testujte, laděte a vylepšujte profil, dokud se model nechová podle vašich představ.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Postup připojení hubu v MOCPilot" width="1100" />

## Pro koho je MOCPilot

MOCPilot je užitečný pro stavitele, kteří chtějí:

- Lepší dálkové ovládání pro motorizované LEGO® modely.
- Způsob ovládání kompatibilních Bluetooth hubů třetích stran.
- Vizuální programovací prostředí pro mechanismy a roboty.
- Předpřipravené profily pro podporované oficiální sady.
- Vlastní panely pro auta, nákladní vozy, vlaky, crawlery, jeřáby a další MOC.
- Jednu aplikaci kombinující huby, motory, senzory, gamepady a ovládání na obrazovce.

## Začít objevovat

- Postupujte podle [rychlého úvodu](/docs/Introducing/QuickStart/) a vytvořte první profil.
- Před výběrem hardwaru zkontrolujte [podporovaná zařízení](/docs/Introducing/SupportedDevices/).
- Až budete připraveni přidat logiku, projděte si [dokumentaci BlockBuilder](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/).
- Pokud hub vyžaduje podporovanou verzi firmwaru, přečtěte si [aktualizaci firmwaru hubu](/docs/Application/Hubs/FirmwareUpdating/).
