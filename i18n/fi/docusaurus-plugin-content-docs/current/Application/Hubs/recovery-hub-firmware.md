---
id: RecoveryHubFirmware
title: Hubin laiteohjelmiston palautus
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Hubin laiteohjelmiston palautus

Obnova firmwaru hubu se používá, když se hub po přerušené nebo neúspěšné aktualizaci firmwaru nemůže normálně spustit.

Během obnovy MOCPilot opraví cestu firmwaru hubu, aby bylo možné hub znovu aktualizovat na nejnovější podporovanou verzi. Tento postup použijte pouze tehdy, když hub nereaguje běžně, MOCPilot hlásí režim obnovy nebo předchozí aktualizace selhala.

:::warning Tärkeää
Nechte hub zapnutý a držte zařízení blízko hubu po celou dobu obnovy. Odpojení Bluetooth, zavření MOCPilot, vyjmutí baterií nebo vypnutí hubu během nahrávání firmwaru může obnovu přerušit.
:::

## Kdy je obnova potřeba

Obnova firmwaru může být potřeba, pokud:

- Aktualizace firmwaru nebyla úspěšně dokončena.
- Hub se už nepřipojuje jako běžný hub.
- Hub se v MOCPilot zobrazí jako **LEGO Bootloader**.
- MOCPilot rozpozná hub připojený v režimu obnovy firmwaru.

Před spuštěním obnovy zkontrolujte, že hub má dostatek energie. Pokud je to možné, nabijte také telefon, tablet nebo počítač s MOCPilot a zapněte Bluetooth.

## Podporované huby

Obnova firmwaru je podporována pro stejné huby jako aktualizace firmwaru:

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(160px, 1fr))', gap: '16px', margin: '16px 0 24px'}}>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/technic_hub_p.webp')} alt="Technic Hub" style={{maxWidth: '140px'}} /><div><strong>Technic Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/city_hub_p.webp')} alt="City Hub" style={{maxWidth: '140px'}} /><div><strong>City Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/boost_hub_p.webp')} alt="Boost Hub" style={{maxWidth: '140px'}} /><div><strong>Boost Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/technic_move_hub_p.webp')} alt="Technic Move Hub" style={{maxWidth: '140px'}} /><div><strong>Technic Move Hub</strong></div></div>
</div>

## Přepnutí Technic Hub, Boost Hub a City Hub do režimu obnovy

Technic Hub, Boost Hub a malý City Hub používají připojení přes bootloader:

1. Vypněte hub.
2. Stiskněte a držte zelené tlačítko.
3. Držte tlačítko, dokud LED hubu nezačne blikat fialově.
4. Nepouštějte tlačítko, dokud LED bliká fialově.
5. Stále držte tlačítko, otevřete **Omat Bluetooth-hubit** v MOCPilot a připojte hub.
6. Po připojení hubu v režimu bootloader můžete tlačítko pustit.

V režimu obnovy se hub může zobrazit jako **LEGO Bootloader** místo běžného názvu.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="LEGO Bootloader" />

## Přepnutí Technic Move Hub do režimu obnovy

Technic Move Hub používá jinou sekvenci obnovy než ostatní podporované huby. Nepřipojuje se jako **LEGO Bootloader**. Tato sekvence načte tovární firmware **1.2.3**, který není určen jako finální firmware pro běžné používání.

Obnova firmwaru Technic Move Hub:

1. Vypněte hub.
2. Stiskněte a držte zelené tlačítko.
3. Držte zelené tlačítko přibližně jednu minutu.
4. Pusťte tlačítko.
5. Počkejte, dokud LED hubu nezačne blikat bíle.
6. Otevřete **Omat Bluetooth-hubit** v MOCPilot a připojte hub.

Po připojení MOCPilot rozpozná tovární firmware a nabídne aktualizaci hubu na nejnovější dostupnou verzi. Spusťte aktualizaci firmwaru a počkejte na dokončení.

## Spuštění obnovy z dialogu

Když MOCPilot rozpozná hub připojený v režimu obnovy firmwaru, zobrazí dialog obnovy.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_1.png')} alt="Hubin laiteohjelmiston palautus" />

Vyberte **Palauta** pro zahájení nahrávání firmwaru do hubu.

Pokud nejste připraveni obnovu spustit, vyberte **Peruuta**. Obnovu můžete spustit později z kontextové nabídky hubu.

## Spuštění obnovy z nabídky hubu

Ruční spuštění obnovy:

1. Otevřete **Omat Bluetooth-hubit**.
2. Najděte hub zobrazený jako **LEGO Bootloader**.
3. Otevřete kontextovou nabídku hubu.
4. Vyberte **Palauta hubin laiteohjelmisto**.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="Palauta hubin laiteohjelmisto" />

## Během obnovy firmwaru

Po spuštění obnovy MOCPilot nahrává firmware do hubu a zobrazuje průběh na obrazovce.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_3.png')} alt="Hubin laiteohjelmiston palautus" />

Počkejte na dokončení. Nepřesouvejte hub daleko od zařízení, nezavírejte aplikaci, nevypínejte Bluetooth ani neodpojujte napájení hubu.

Hub se může během procesu několikrát restartovat nebo znovu připojit. To je očekávané. Nechte MOCPilot otevřený a počkejte na dokončení obnovy.

## Dokončení obnovy

Po úspěšném dokončení obnovy MOCPilot zobrazí potvrzení.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_4.png')} alt="Hubin laiteohjelmiston palautus" />

Vyberte **OK**. Hub by se měl restartovat a připojit jako běžný hub místo **LEGO Bootloader**.

Po obnově zkontrolujte hub v **Omat Bluetooth-hubit**. Pokud MOCPilot stále hlásí, že je potřeba aktualizace firmwaru, spusťte běžný postup [Laiteohjelmiston päivitys](/docs/Application/Hubs/FirmwareUpdating/).

## Pokud obnova selže

Pokud se obnova nedokončí úspěšně:

1. Držte hub blízko zařízení.
2. Restartujte napájení hubu.
3. Znovu přepněte hub do režimu obnovy.
4. Připojte se k **LEGO Bootloader** v MOCPilot.
5. Znovu spusťte **Palauta hubin laiteohjelmisto**.

Pokud se chybová zpráva objeví znovu, zopakujte obnovu od začátku. Pokud hub nejde obnovit ani po několika pokusech, vyměňte nebo nabijte baterie a zkuste to znovu.
