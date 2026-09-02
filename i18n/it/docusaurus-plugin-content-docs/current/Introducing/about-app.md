---
id: AboutApp
title: Informazioni su MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Costruisci. Guida. Controlla tutto.

**MOCPilot** — un’app per creare profili di controllo personalizzati per LEGO® e creazioni Bluetooth compatibili.

Offre ai costruttori un unico posto per collegare hub, controllare motori, leggere sensori, progettare dashboard e creare programmi visuali per modelli, meccanismi, auto, camion, treni, robot e MOC personalizzati.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="App MOCPilot su un telefono" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Cosa offre MOCPilot</h2>
    <ul>
      <li>Profili personalizzati per i tuoi modelli.</li>
      <li>Profili pronti per set ufficiali supportati.</li>
      <li>Connessione e gestione degli hub Bluetooth.</li>
      <li>Programmazione visuale a blocchi per automazione e logica.</li>
      <li>Controlli dashboard per guidare e usare i modelli.</li>
      <li>Supporto per LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motori, sensori e dispositivi Bluetooth compatibili.</li>
    </ul>
  </div>
</div>

## L’idea

La maggior parte delle costruzioni motorizzate richiede più di un semplice telecomando. Un’auto può avere bisogno di sterzo, acceleratore, luci, controllo batteria, sequenza del cambio o routine di avvio speciale. Un robot può richiedere sensori, eventi, logica condizionale e più hub che lavorano insieme.

MOCPilot è pensato per lo spazio tra un telecomando base e un ambiente di programmazione completo. Puoi iniziare guidando un modello da una dashboard su schermo e poi aggiungere logica, sensori e automazione quando la costruzione diventa più avanzata.

## Profili

Un **profilo** è il centro di controllo di un modello.

In un profilo puoi scegliere quali hub appartengono al modello, creare il programma che lo fa funzionare e progettare la dashboard usata per controllarlo.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="Pagina profili di MOCPilot" width="420" />

<details>
<summary>Profili predefiniti</summary>

I profili predefiniti sono esempi pronti per i set ufficiali supportati. Sono utili per iniziare rapidamente o studiare come viene assemblato un profilo funzionante.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Profili predefiniti MOCPilot" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Programma a blocchi predefinito MOCPilot" width="1100" />

</details>

<details>
<summary>Profili personalizzati</summary>

I profili personalizzati sono per i tuoi MOC ed esperimenti. Puoi creare un profilo, aggiungere hub, collegare motori e sensori, costruire un programma e progettare una dashboard adatta al modello esatto.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Creare un profilo personalizzato MOCPilot" width="420" />

</details>

## Collegare hub e dispositivi

MOCPilot può collegarsi agli hub Bluetooth supportati e ai dispositivi compatibili, rendendoli disponibili nel tuo profilo.

Puoi usare un profilo con un solo hub per una costruzione semplice oppure collegare più hub quando il modello richiede più porte, sistemi di alimentazione separati o moduli indipendenti.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Pagina I miei hub Bluetooth in MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Hub Bluetooth collegati in MOCPilot" width="1100" />

<details>
<summary>Esempi di hardware supportato</summary>

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

Consulta la pagina [hub, motori e sensori supportati](/docs/Introducing/SupportedDevices/) per l’elenco completo.

</details>

## Costruire la logica con i blocchi

MOCPilot include un builder visuale a blocchi. Puoi creare programmi collegando blocchi invece di scrivere codice.

I blocchi possono reagire agli eventi, controllare motori, leggere sensori, lavorare con variabili, usare input da gamepad, aggiornare i controller della dashboard e coordinare più azioni.

MOCPilot supporta completamente i gamepad fisici collegati. I blocchi gamepad permettono di leggere pulsanti, grilletti, D-pad e levette, così puoi associare un controller reale al modello quando il controllo fisico è preferibile al touchscreen.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="Programma utente MOCPilot creato con blocchi" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Blocco quando il programma si avvia" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Blocco avvia motore a velocità" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Blocco livello batteria hub" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Blocco valore volante" />
</div>

<details>
<summary>Cosa puoi fare con i programmi a blocchi</summary>

- Avviare, fermare e sterzare motori.
- Leggere livello batteria, tensione, inclinazione, orientamento, temperatura e valori dei sensori.
- Configurare controlli con gamepad fisico per sterzo, acceleratore, grilletti, azioni e cambio modalità.
- Reagire quando cambiano pulsanti, sensori, timer o controlli della dashboard.
- Creare controlli di avvio prima che il modello inizi a muoversi.
- Aggiungere logica personalizzata per luci, calibrazione dello sterzo, modalità di potenza e configurazione hub.
- Usare variabili, liste, condizioni, cicli, broadcast e blocchi personalizzati per organizzare comportamenti complessi.

</details>

## Progettare una dashboard di guida

La dashboard è lo schermo usato mentre controlli il modello. Può includere volanti, joystick, slider, pulsanti, interruttori, pedali, monitor e altri controller.

Puoi collegare i controlli della dashboard e gli input del gamepad fisico a blocchi e azioni dell’hub, così l’interfaccia corrisponde al modello.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="Controller dashboard MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="Schermata di controllo MOCPilot con volante e pedali" width="1100" />

<details>
<summary>Esempi di dashboard</summary>

- Usa volante e pedali per le auto.
- Usa slider per gru, sollevatori e attuatori lineari.
- Usa pulsanti per luci, clacson, cambi marcia o azioni scriptate.
- Usa monitor per mostrare batteria, velocità, valori dei sensori o stato personalizzato del programma.
- Usa un gamepad collegato se preferisci pulsanti, levette e grilletti fisici al touchscreen.

</details>

## Mantenere gestibili le costruzioni avanzate

Quando un modello cresce, il profilo può crescere con lui. MOCPilot supporta logica riutilizzabile con **My Blocks**, configurazione hub specifica del profilo, più controller e flussi che combinano controllo manuale e automazione.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Esempio di utilizzo di My Blocks in MOCPilot" width="1100" />

Questo aiuta a mantenere leggibili i programmi grandi. Ad esempio, un profilo può avere un blocco personalizzato per aggiornare la batteria, uno per calibrare lo sterzo e uno per una modalità di guida speciale.

## Flusso tipico

1. Crea o apri un profilo.
2. Aggiungi gli hub Bluetooth e i dispositivi usati dal modello.
3. Costruisci il programma con i blocchi.
4. Progetta una dashboard per guida e interazione.
5. Premi **Play**.
6. Testa, regola e migliora il profilo finché il modello si comporta come desideri.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Flusso di connessione hub in MOCPilot" width="1100" />

## A chi serve MOCPilot

MOCPilot è utile ai costruttori che vogliono:

- Un telecomando migliore per modelli LEGO® motorizzati.
- Un modo per controllare hub Bluetooth compatibili di terze parti.
- Un ambiente di programmazione visuale per meccanismi e robot.
- Profili predefiniti per set ufficiali supportati.
- Dashboard personalizzate per auto, camion, treni, crawler, gru e altri MOC.
- Un’unica app che combina hub, motori, sensori, gamepad e controlli su schermo.

## Inizia a esplorare

- Segui il [tutorial di avvio rapido](/docs/Introducing/QuickStart/) per creare il tuo primo profilo.
- Controlla i [dispositivi supportati](/docs/Introducing/SupportedDevices/) prima di scegliere l’hardware.
- Esplora la [documentazione BlockBuilder](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/) quando sei pronto ad aggiungere logica.
- Consulta [aggiornamento firmware hub](/docs/Application/Hubs/FirmwareUpdating/) se un hub richiede una versione firmware supportata.
