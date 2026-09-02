---
id: AboutApp
title: Tietoja MOCPilotista
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Rakenna. Aja. Hallitse kaikkea.

**MOCPilot** on sovellus omien ohjausprofiilien luomiseen LEGO®-malleille ja yhteensopiville Bluetooth-ohjatuille rakennelmille.

Se tarjoaa rakentajille yhden paikan hubien yhdistämiseen, moottorien ohjaukseen, anturien lukemiseen, ohjauspaneelien suunnitteluun ja visuaalisten ohjelmien tekemiseen malleille, mekanismeille, autoille, kuorma-autoille, junille, roboteille ja omille MOCeille.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="MOCPilot-sovellus puhelimessa" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Mitä MOCPilot tarjoaa</h2>
    <ul>
      <li>Omat profiilit omille malleillesi.</li>
      <li>Valmiit profiilit tuetuille virallisille seteille.</li>
      <li>Bluetooth-hubien yhdistäminen ja hallinta.</li>
      <li>Visuaalinen lohko-ohjelmointi automaatioon ja logiikkaan.</li>
      <li>Ohjauspaneelin säätimet mallien ajamiseen ja käyttämiseen.</li>
      <li>Tuki LEGO® Powered Up-, Technic-, BuWizz-, SBrick- ja Mould King -laitteille, moottoreille, antureille sekä yhteensopiville Bluetooth-laitteille.</li>
    </ul>
  </div>
</div>

## Ajatus

Useimmat moottoroidut rakennelmat tarvitsevat enemmän kuin yksinkertaisen kaukosäätimen. Auto voi tarvita ohjauksen, kaasun, valot, akun seurannan, vaihteiston sekvenssin tai erityisen käynnistysrutiinin. Robotti voi tarvita antureita, tapahtumia, ehdollista logiikkaa ja useita yhdessä toimivia hubeja.

MOCPilot on suunniteltu peruskaukosäätimen ja täyden ohjelmointiympäristön väliin. Voit aloittaa ajamalla mallia näytön ohjauspaneelista ja lisätä myöhemmin logiikkaa, antureita ja automaatiota.

## Profiilit

**Profiili** on yhden mallin ohjauskeskus.

Profiilissa voit valita malliin kuuluvat hubit, luoda mallia ajavan ohjelman ja suunnitella ohjauspaneelin.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="MOCPilotin profiilisivu" width="420" />

<details>
<summary>Valmiit profiilit</summary>

Valmiit profiilit ovat käyttövalmiita esimerkkejä tuetuille virallisille seteille. Ne auttavat aloittamaan nopeasti tai tutkimaan, miten toimiva profiili on rakennettu.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="MOCPilotin valmiit profiilit" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Valmis MOCPilot-lohko-ohjelma" width="1100" />

</details>

<details>
<summary>Omat profiilit</summary>

Omat profiilit ovat omia MOCeja ja kokeiluja varten. Voit luoda profiilin, lisätä hubeja, yhdistää moottoreita ja antureita, rakentaa ohjelman ja suunnitella malliin sopivan ohjauspaneelin.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Luo oma MOCPilot-profiili" width="420" />

</details>

## Yhdistä hubit ja laitteet

MOCPilot voi yhdistää tuettuihin Bluetooth-hubeihin ja yhteensopiviin laitteisiin ja tuoda ne profiilisi käyttöön.

Yksinkertainen malli voi käyttää yhtä hubia, tai voit yhdistää useita hubeja, kun malli tarvitsee enemmän portteja, erillisiä virtajärjestelmiä tai itsenäisiä moduuleja.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Omat Bluetooth-hubit -sivu MOCPilotissa" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Yhdistetyt Bluetooth-hubit MOCPilotissa" width="1100" />

<details>
<summary>Esimerkkejä tuetusta laitteistosta</summary>

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

Katso koko luettelo [tuetuista hubeista, moottoreista ja antureista](/docs/Introducing/SupportedDevices/).

</details>

## Rakenna logiikkaa lohkoilla

MOCPilot sisältää visuaalisen lohkorakentajan. Voit luoda ohjelmia yhdistämällä lohkoja koodin kirjoittamisen sijaan.

Lohkot voivat reagoida tapahtumiin, ohjata moottoreita, lukea antureita, käsitellä muuttujia, käyttää peliohjaimen syötettä, päivittää ohjauspaneelin säätimiä ja koordinoida useita toimintoja.

MOCPilot tukee täysin yhdistettyjä fyysisiä peliohjaimia. Peliohjainlohkot lukevat painikkeet, liipaisimet, D-padin suunnat ja tatit, joten voit liittää oikean ohjaimen malliin, kun fyysinen ohjaus tuntuu kosketusnäyttöä paremmalta.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="Lohkoilla rakennettu MOCPilot-käyttäjäohjelma" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Ohjelman käynnistyessä -lohko" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Käynnistä moottori nopeudella -lohko" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Hubin akun varaustaso -lohko" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Ohjauspyörän arvo -lohko" />
</div>

<details>
<summary>Mitä lohko-ohjelmilla voi tehdä</summary>

- Käynnistää, pysäyttää ja ohjata moottoreita.
- Lukea akun varausta, jännitettä, kallistusta, suuntaa, lämpötilaa ja anturiarvoja.
- Määrittää fyysisen peliohjaimen ohjaukseen, kaasuun, liipaisimiin, toimintoihin ja tilanvaihtoon.
- Reagoida painikkeiden, antureiden, ajastimien tai ohjauspaneelin säätimien muutoksiin.
- Luoda käynnistystarkistuksia ennen mallin liikkumista.
- Lisätä omaa logiikkaa valoille, ohjauksen kalibroinnille, tehotiloille ja hubin määritykselle.
- Käyttää muuttujia, listoja, ehtoja, silmukoita, lähetyksiä ja omia lohkoja monimutkaisen toiminnan järjestämiseen.

</details>

## Suunnittele ajo-ohjauspaneeli

Ohjauspaneeli on näyttö, jota käytät mallin hallintaan. Se voi sisältää ohjauspyöriä, joystickeja, liukusäätimiä, painikkeita, kytkimiä, polkimia, näyttöjä ja muita säätimiä.

Voit yhdistää ohjauspaneelin säätimet ja fyysisen peliohjaimen syötteet lohkoihin ja hubin toimintoihin, jotta käyttöliittymä sopii malliin.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="MOCPilotin ohjauspaneelin säätimet" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="MOCPilotin ohjausnäyttö ohjauspyörällä ja polkimilla" width="1100" />

<details>
<summary>Ohjauspaneeliesimerkkejä</summary>

- Käytä autoille ohjauspyörää ja polkimia.
- Käytä liukusäätimiä nostureille, hisseille ja lineaaritoimilaitteille.
- Käytä painikkeita valoille, torvelle, vaihdoille tai skriptatuille toiminnoille.
- Käytä näyttöjä akun, nopeuden, anturiarvojen tai oman ohjelmatilan esittämiseen.
- Käytä yhdistettyä peliohjainta, jos pidät fyysisistä painikkeista, tateista ja liipaisimista enemmän kuin kosketusohjauksesta.

</details>

## Pidä edistyneet rakennelmat hallittavina

Kun malli kasvaa, profiili voi kasvaa sen mukana. MOCPilot tukee uudelleenkäytettävää logiikkaa **My Blocks** -toiminnolla, profiilikohtaisia hubiasetuksia, useita säätimiä ja ohjelmavirtoja, jotka yhdistävät käsiohjauksen ja automaation.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Esimerkki My Blocks -käytöstä MOCPilotissa" width="1100" />

Tämä auttaa pitämään suuret ohjelmat luettavina. Profiilissa voi olla esimerkiksi oma lohko akun päivityksille, toinen ohjauksen kalibroinnille ja kolmas erityiselle ajotilalle.

## Tyypillinen työnkulku

1. Luo tai avaa profiili.
2. Lisää mallin käyttämät Bluetooth-hubit ja laitteet.
3. Rakenna ohjelma lohkoilla.
4. Suunnittele ohjauspaneeli ajamiseen ja vuorovaikutukseen.
5. Paina **Play**.
6. Testaa, säädä ja paranna profiilia, kunnes malli toimii haluamallasi tavalla.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Hubin yhdistämisen kulku MOCPilotissa" width="1100" />

## Kenelle MOCPilot sopii

MOCPilot sopii rakentajille, jotka haluavat:

- Paremman kaukosäätimen moottoroiduille LEGO®-malleille.
- Tavan ohjata kolmannen osapuolen yhteensopivia Bluetooth-hubeja.
- Visuaalisen ohjelmointiympäristön mekanismeille ja roboteille.
- Valmiit profiilit tuetuille virallisille seteille.
- Omat ohjauspaneelit autoille, kuorma-autoille, junille, crawlereille, nostureille ja muille MOCeille.
- Yhden sovelluksen, joka yhdistää hubit, moottorit, anturit, peliohjaimet ja näyttösäätimet.

## Aloita tutustuminen

- Luo ensimmäinen profiilisi [pika-aloitusohjeen](/docs/Introducing/QuickStart/) avulla.
- Tarkista [tuetut laitteet](/docs/Introducing/SupportedDevices/) ennen laitteiston valintaa.
- Tutustu [BlockBuilder-dokumentaatioon](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/), kun olet valmis lisäämään logiikkaa.
- Lue [hubin laiteohjelmiston päivitys](/docs/Application/Hubs/FirmwareUpdating/), jos hubi vaatii tuetun laiteohjelmistoversion.
