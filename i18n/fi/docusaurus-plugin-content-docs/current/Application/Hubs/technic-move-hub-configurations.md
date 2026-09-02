---
id: TechnicMoveHubConfigurations
title: Technic Move Hub -määritykset
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Technic Move Hub -määritykset

## Yleiskatsaus

Technic Move Hub toi LEGO Powered Up -hubien perheeseen ainutlaatuisen ominaisuuden: hubi voi muuttaa toimintaansa sen mukaan, mikä määritys siihen on tällä hetkellä käytössä.

MOCPilot antaa muuttaa Technic Move Hubin määritystä, jotta hubin toiminta vastaa virallista LEGO-settiä, jota haluat ohjata.

## Tuetut määritykset

Tällä hetkellä tunnetaan nämä Technic Move Hub -määritykset:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Technic Move Hubin määritysvaihtoehdot" />

## Määrityksen muuttaminen Omat Bluetooth-hubit -sivulta

Voit muuttaa määrityksen **Omat Bluetooth-hubit** -sivulta:

1. Avaa **Omat Bluetooth-hubit**.
2. Etsi Technic Move Hub.
3. Avaa hubin kontekstivalikko.
4. Valitse **Valitse määritys**.
5. Valitse tarvittava määritys.
6. Vahvista uudelleenmäärityksen valintaikkuna.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Technic Move Hubin kontekstivalikko" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Technic Move Hubin määritysalivalikko" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Technic Move Hubin uudelleenmäärityksen vahvistusikkuna" />

:::warning Tärkeää
Hubin määrityksen muuttaminen flashaa hubiin aliohjelman ja muistuttaa laiteohjelmiston päivitystä.

Pidä hubi päällä koko prosessin ajan. Pidä puhelin, tabletti tai tietokone päällä ja lähellä hubia, jotta Bluetooth-yhteys pysyy vakaana. Älä sulje MOCPilotia, älä poista Bluetoothia käytöstä äläkä sammuta hubia määrityksen muuttamisen aikana.

Määrityksen muutoksen keskeyttäminen voi vahingoittaa hubin laiteohjelmistoa. Jos näin käy, laiteohjelmiston palautus voi olla tarpeen ennen kuin hubia voi käyttää uudelleen. Seuraa [hubin laiteohjelmiston palautus](/docs/Application/Hubs/RecoveryHubFirmware/) -ohjetta, jos palautus tarvitaan.
:::

Uudelleenmäärityksen aikana hubi ei vastaa normaaleihin komentoihin. Sen LED vilkkuu porrastetulla värillisellä ilmaisulla, kunnes prosessi on valmis. Kun uusi määritys on otettu käyttöön, hubi alustetaan uudelleen.

## Määrityslohkot

MOCPilot sisältää myös lohkoja Technic Move Hubin määrityksen lukemiseen ja muuttamiseen ohjelman aikana.

### Aseta hubin määritys

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Aseta hubin määritys -lohko" />

**Aseta hubin määritys** -lohko muuttaa valitun hubin johonkin sen tuetuista määritysprofiileista.

- Hubivalitsin: valitsee uudelleenmääritettävän hubin.
- Määritysvalitsin: valitsee kohdemäärityksen.
- Technic Move Hubin käytettävissä olevat määritykset: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** ja **Batmobile™ Tumbler**.

Katso [Aseta hubin määritys -lohkon dokumentaatio](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Hubin määritys

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Hubin määritys -lohko" />

**Hubin määritys** -lohko ilmoittaa valitun hubin nykyisen määrityksen.

- Hubivalitsin: valitsee luettavan hubin.
- Tulostusmuoto: **teksti** palauttaa määrityksen nimen.
- Tulostusmuoto: **indeksi** palauttaa määrityksen indeksin, joka on hyödyllinen ehtojen vertailuissa.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Hubin määritys -lohkon tulostusmuodon vaihtoehdot" />

Katso [Hubin määritys -lohkon dokumentaatio](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Tehopulssi

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Tehopulssi -lohko" />

**Tehopulssi** -lohko lähettää tehopulssikomennon valitulle Technic Move Hubille. Tämä lohko toimii vain, kun Technic Move Hub on määritetty **Batmobile™ Tumbler** -asetukseen.

Kun lohko suoritetaan, hubi käynnistää moottorit hetkeksi suurimmalla käytettävissä olevalla teholla ja nopeudella, yleensä noin 1-2 sekunniksi.

Katso [Tehopulssi -lohkon dokumentaatio](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Määrityksen muuttaminen ohjelman suorituksen aikana

Technic Move Hubin määritystä voi muuttaa myös ohjelman suorituksen aikana.

Yleinen toimintatapa on:

1. Lue hubin nykyinen määritys.
2. Vertaa sitä profiilin vaatimaan määritykseen.
3. Jos määritys on eri, aseta vaadittu määritys.
4. Lue määritys uudelleen uudelleenmäärityksen jälkeen.
5. Jatka vain, kun hubi ilmoittaa odotetun määrityksen.
6. Katkaise yhteys tai pysäytä ohjelma, jos vaadittua määritystä ei otettu käyttöön.

Tätä hubia käyttävää valmista profiilia voi käyttää tämän toimintatavan esimerkkinä.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Lohkoesimerkki Technic Move Hubin määrityksen muuttamisesta suorituksen aikana" />
