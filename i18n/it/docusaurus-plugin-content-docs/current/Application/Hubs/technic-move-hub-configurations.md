---
id: TechnicMoveHubConfigurations
title: Configurazioni di Technic Move Hub
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Configurazioni di Technic Move Hub

## Panoramica

Technic Move Hub ha introdotto una funzione unica nella famiglia di hub LEGO Powered Up: l’hub può cambiare comportamento in base alla configurazione attualmente applicata.

MOCPilot consente di modificare la configurazione di Technic Move Hub in modo che il comportamento dell’hub corrisponda al set LEGO ufficiale che vuoi controllare.

## Configurazioni supportate

Al momento sono note queste configurazioni di Technic Move Hub:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Opzioni di configurazione di Technic Move Hub" />

## Modificare la configurazione da I miei hub Bluetooth

Puoi modificare la configurazione dalla pagina **I miei hub Bluetooth**:

1. Apri **I miei hub Bluetooth**.
2. Trova Technic Move Hub.
3. Apri il menu contestuale dell’hub.
4. Seleziona **Seleziona configurazione**.
5. Scegli la configurazione richiesta.
6. Conferma la finestra di riconfigurazione.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Menu contestuale di Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Sottomenu di configurazione di Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Finestra di conferma della riconfigurazione di Technic Move Hub" />

:::warning Importante
La modifica della configurazione dell’hub scrive un sottoprogramma nell’hub ed è simile a un aggiornamento firmware.

Mantieni l’hub acceso durante tutto il processo. Tieni telefono, tablet o computer alimentati e vicini all’hub, così la connessione Bluetooth resta stabile. Non chiudere MOCPilot, non disattivare Bluetooth e non spegnere l’hub mentre la configurazione viene modificata.

Interrompere la modifica della configurazione può danneggiare il firmware dell’hub. In questo caso potrebbe essere necessario ripristinare il firmware prima di usare di nuovo l’hub. Segui la guida al [ripristino del firmware dell’hub](/docs/Application/Hubs/RecoveryHubFirmware/) se il ripristino è necessario.
:::

Durante la riconfigurazione, l’hub non risponde ai comandi normali. Il LED lampeggia con un’indicazione colorata a passaggi fino al completamento del processo. Dopo l’applicazione della nuova configurazione, l’hub viene reinizializzato.

## Blocchi di configurazione

MOCPilot include anche blocchi per leggere e modificare la configurazione di Technic Move Hub durante un programma.

### Imposta configurazione hub

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Blocco Imposta configurazione hub" />

Il blocco **Imposta configurazione hub** cambia l’hub selezionato in uno dei profili di configurazione supportati.

- Selettore hub: sceglie l’hub da riconfigurare.
- Selettore configurazione: sceglie la configurazione di destinazione.
- Configurazioni disponibili per Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** e **Batmobile™ Tumbler**.

Consulta la [documentazione del blocco Imposta configurazione hub](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Configurazione hub

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Blocco Configurazione hub" />

Il blocco **Configurazione hub** indica la configurazione attuale dell’hub selezionato.

- Selettore hub: sceglie l’hub da leggere.
- Formato di output: **testo** restituisce il nome della configurazione.
- Formato di output: **indice** restituisce l’indice della configurazione, utile per i confronti nelle condizioni.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Opzioni del formato di output del blocco Configurazione hub" />

Consulta la [documentazione del blocco Configurazione hub](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Impulso di potenza

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Blocco Impulso di potenza" />

Il blocco **Impulso di potenza** invia un comando di impulso di potenza al Technic Move Hub selezionato. Questo blocco funziona solo quando Technic Move Hub è configurato come **Batmobile™ Tumbler**.

Quando viene eseguito, l’hub avvia i motori con la massima potenza e velocità disponibili per un breve periodo, di solito circa 1-2 secondi.

Consulta la [documentazione del blocco Impulso di potenza](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Modificare la configurazione durante l’esecuzione del programma

È possibile modificare la configurazione di Technic Move Hub anche mentre un programma è in esecuzione.

L’approccio comune è:

1. Leggi la configurazione attuale dell’hub.
2. Confrontala con la configurazione richiesta dal profilo.
3. Se la configurazione è diversa, imposta quella richiesta.
4. Leggi di nuovo la configurazione dopo la riconfigurazione.
5. Continua solo quando l’hub indica la configurazione prevista.
6. Disconnetti o arresta il programma se la configurazione richiesta non è stata applicata.

Il profilo predefinito che usa questo hub può essere utilizzato come riferimento per questo approccio.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Esempio di blocchi per modificare la configurazione di Technic Move Hub durante l’esecuzione" />
