---
id: AboutApp
title: Despre MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Construiește. Condu. Controlează tot.

**MOCPilot** este o aplicație pentru crearea profilurilor de control personalizate pentru LEGO® și construcții compatibile cu Bluetooth.

Le oferă constructorilor un singur loc pentru conectarea huburilor, controlul motoarelor, citirea senzorilor, proiectarea panourilor și crearea programelor vizuale pentru modele, mecanisme, mașini, camioane, trenuri, roboți și MOC-uri personalizate.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="Aplicația MOCPilot pe un telefon" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Ce oferă MOCPilot</h2>
    <ul>
      <li>Profiluri personalizate pentru modelele tale.</li>
      <li>Profiluri gata făcute pentru seturi oficiale acceptate.</li>
      <li>Conectarea și gestionarea huburilor Bluetooth.</li>
      <li>Programare vizuală cu blocuri pentru automatizare și logică.</li>
      <li>Controale de panou pentru condus și operarea modelelor.</li>
      <li>Suport pentru LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motoare, senzori și dispozitive Bluetooth compatibile.</li>
    </ul>
  </div>
</div>

## Ideea

Cele mai multe construcții motorizate au nevoie de mai mult decât o telecomandă simplă. O mașină poate necesita direcție, accelerație, lumini, monitorizarea bateriei, o secvență de cutie de viteze sau o rutină specială de pornire. Un robot poate necesita senzori, evenimente, logică condițională și mai multe huburi care lucrează împreună.

MOCPilot este proiectat pentru zona dintre o telecomandă de bază și un mediu complet de programare. Poți începe prin a conduce modelul dintr-un panou pe ecran, apoi poți adăuga logică, senzori și automatizare.

## Profiluri

Un **profil** este centrul de control al unui model.

Într-un profil poți alege huburile modelului, poți crea programul care rulează modelul și poți proiecta panoul folosit pentru control.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="Pagina de profiluri MOCPilot" width="420" />

<details>
<summary>Profiluri pregătite</summary>

Profilurile pregătite sunt exemple gata făcute pentru seturi oficiale acceptate. Sunt utile când vrei să începi rapid sau să studiezi cum este construit un profil funcțional.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Profiluri pregătite MOCPilot" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Program cu blocuri pregătit MOCPilot" width="1100" />

</details>

<details>
<summary>Profiluri personalizate</summary>

Profilurile personalizate sunt pentru propriile MOC-uri și experimente. Poți crea un profil, adăuga huburi, conecta motoare și senzori, construi un program și proiecta un panou potrivit modelului exact.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Crearea unui profil MOCPilot personalizat" width="420" />

</details>

## Conectarea huburilor și dispozitivelor

MOCPilot se poate conecta la huburi Bluetooth acceptate și dispozitive compatibile, apoi le face disponibile în profilul tău.

Poți folosi un profil cu un singur hub pentru o construcție simplă sau poți conecta mai multe huburi când modelul are nevoie de mai multe porturi, sisteme de alimentare separate sau module independente.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Pagina Huburile mele Bluetooth în MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Huburi Bluetooth conectate în MOCPilot" width="1100" />

<details>
<summary>Exemple de hardware acceptat</summary>

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

Vezi pagina [huburi, motoare și senzori acceptați](/docs/Introducing/SupportedDevices/) pentru lista completă.

</details>

## Construirea logicii cu blocuri

MOCPilot include un constructor vizual de blocuri. Poți crea programe conectând blocuri în loc să scrii cod.

Blocurile pot reacționa la evenimente, controla motoare, citi senzori, lucra cu variabile, folosi intrarea de la gamepad, actualiza controalele panoului și coordona mai multe acțiuni.

MOCPilot acceptă complet gamepadurile fizice conectate. Blocurile de gamepad pot citi butoane, trăgaci, direcții D-pad și stickuri, astfel încât poți mapa un controler real la model când controlul fizic este preferabil ecranului tactil.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="Program MOCPilot construit cu blocuri" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Bloc la pornirea programului" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Bloc pornire motor la viteză" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Bloc nivel baterie hub" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Bloc valoare volan" />
</div>

<details>
<summary>Ce poți face cu programele pe blocuri</summary>

- Pornești, oprești și virezi motoare.
- Citești nivelul bateriei, tensiunea, înclinarea, orientarea, temperatura și valorile senzorilor.
- Configurezi controale cu gamepad fizic pentru direcție, accelerație, trăgaci, acțiuni și schimbarea modului.
- Reacționezi când se schimbă butoane, senzori, temporizatoare sau controale de panou.
- Creezi verificări de pornire înainte ca modelul să înceapă să se miște.
- Adaugi logică proprie pentru lumini, calibrarea direcției, moduri de putere și configurarea hubului.
- Folosești variabile, liste, condiții, bucle, difuzări și blocuri personalizate pentru comportamente complexe.

</details>

## Proiectarea unui panou de condus

Panoul este ecranul folosit în timp ce controlezi modelul. Poate include volane, joystickuri, glisoare, butoane, comutatoare, pedale, monitoare și alte controale.

Poți conecta controalele panoului și intrările gamepadului fizic la blocuri și acțiuni ale hubului, astfel încât interfața să se potrivească modelului.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="Controale de panou MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="Ecran de control MOCPilot cu volan și pedale" width="1100" />

<details>
<summary>Exemple de panouri</summary>

- Folosește volan și pedale pentru mașini.
- Folosește glisoare pentru macarale, lifturi și actuatoare liniare.
- Folosește butoane pentru lumini, claxon, schimbări de viteză sau acțiuni scriptate.
- Folosește monitoare pentru baterie, viteză, valori de senzori sau stare personalizată a programului.
- Folosește un gamepad conectat dacă preferi butoane, stickuri și trăgaci fizici în locul comenzilor tactile.

</details>

## Păstrează construcțiile avansate ușor de gestionat

Pe măsură ce modelul crește, profilul poate crește odată cu el. MOCPilot acceptă logică reutilizabilă cu **My Blocks**, configurare de hub specifică profilului, mai multe controale și fluxuri de program care combină controlul manual cu automatizarea.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Exemplu de utilizare My Blocks în MOCPilot" width="1100" />

Acest lucru ajută la menținerea programelor mari ușor de citit. De exemplu, un profil poate avea un bloc personalizat pentru actualizări de baterie, altul pentru calibrarea direcției și altul pentru un mod special de condus.

## Flux tipic

1. Creează sau deschide un profil.
2. Adaugă huburile Bluetooth și dispozitivele folosite de model.
3. Construiește programul cu blocuri.
4. Proiectează un panou pentru condus și interacțiune.
5. Apasă **Play**.
6. Testează, ajustează și îmbunătățește profilul până când modelul se comportă așa cum dorești.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Flux de conectare a hubului în MOCPilot" width="1100" />

## Pentru cine este MOCPilot

MOCPilot este util constructorilor care doresc:

- O telecomandă mai bună pentru modele LEGO® motorizate.
- O modalitate de a controla huburi Bluetooth compatibile de la terți.
- Un mediu de programare vizuală pentru mecanisme și roboți.
- Profiluri pregătite pentru seturi oficiale acceptate.
- Panouri personalizate pentru mașini, camioane, trenuri, crawlere, macarale și alte MOC-uri.
- O singură aplicație care combină huburi, motoare, senzori, gamepaduri și controale pe ecran.

## Începe explorarea

- Urmează [tutorialul de pornire rapidă](/docs/Introducing/QuickStart/) pentru a crea primul profil.
- Verifică [dispozitivele acceptate](/docs/Introducing/SupportedDevices/) înainte de a alege hardware.
- Explorează [documentația BlockBuilder](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/) când ești gata să adaugi logică.
- Consultă [actualizarea firmware-ului hubului](/docs/Application/Hubs/FirmwareUpdating/) dacă un hub necesită o versiune firmware acceptată.
