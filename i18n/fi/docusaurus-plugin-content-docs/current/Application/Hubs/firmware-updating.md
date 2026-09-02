---
id: FirmwareUpdating
title: Laiteohjelmiston päivitys
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Laiteohjelmiston päivitys

MOCPilot může aktualizovat firmware podporovaných hubů LEGO Powered Up, když je dostupná novější kompatibilní verze.

Aktualizace firmwaru může být nutná, aby hub správně fungoval s MOCPilot. Novější firmware může zlepšit kompatibilitu, opravit chování hubu a zpřístupnit funkce očekávané pro daný model.

## Aktualizace firmwaru je aktuálně podporována pro tyto huby

Aktualizace firmwaru je aktuálně podporována pro tyto huby:

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(160px, 1fr))', gap: '16px', margin: '16px 0 24px'}}>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/technic_hub_p.webp')} alt="Technic Hub" style={{maxWidth: '140px'}} /><div><strong>Technic Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/city_hub_p.webp')} alt="City Hub" style={{maxWidth: '140px'}} /><div><strong>City Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/boost_hub_p.webp')} alt="Boost Hub" style={{maxWidth: '140px'}} /><div><strong>Boost Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/technic_move_hub_p.webp')} alt="Technic Move Hub" style={{maxWidth: '140px'}} /><div><strong>Technic Move Hub</strong></div></div>
</div>

## Před spuštěním

Před spuštěním aktualizace se ujistěte, že hub i zařízení s MOCPilot mají dostatek energie.

Po celou dobu nechte hub zapnutý a držte telefon, tablet nebo počítač blízko hubu, aby Bluetooth spojení zůstalo stabilní. Během nahrávání firmwaru nezavírejte MOCPilot, nevypínejte Bluetooth ani hub.

:::warning Tärkeää
Přerušení aktualizace firmwaru může zanechat firmware hubu v neúplném stavu. V takovém případě může být před dalším použitím potřeba obnova firmwaru.
:::

## Spuštění aktualizace

Při připojení hubu MOCPilot zkontroluje nainstalovanou verzi firmwaru. Pokud je potřeba novější verze, aplikace zobrazí dialog aktualizace firmwaru.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_1.png')} alt="Laiteohjelmiston päivitys" />

Vyberte **Päivitä** pro okamžité spuštění aktualizace firmwaru.

Pokud nechcete aktualizovat hned, vyberte **Peruuta**. Aktualizaci můžete spustit později z kontextové nabídky hubu.

## Aktualizace později z nabídky hubu

Ruční spuštění aktualizace firmwaru:

1. Otevřete **Omat Bluetooth-hubit**.
2. Najděte hub, který potřebuje aktualizaci.
3. Otevřete kontextovou nabídku hubu.
4. Vyberte **Päivitä laiteohjelmisto**.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_2.png')} alt="Päivitä laiteohjelmisto" />

## Během aktualizace firmwaru

Po spuštění aktualizace MOCPilot nahraje firmware do hubu a zobrazí průběh.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_3.png')} alt="Laiteohjelmiston päivitys" />

Počkejte na dokončení nahrávání. Hub se může při použití nové verze restartovat nebo dočasně odpojit.

Po nahrání firmwaru MOCPilot znovu vyhledá hub. Držte hub poblíž a počkejte na opětovné připojení.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_4.png')} alt="Laiteohjelmiston päivitys" />

## Dokončení aktualizace

Po úspěšném dokončení aktualizace MOCPilot zobrazí potvrzení.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_5.png')} alt="Laiteohjelmiston päivitys" />

Vyberte **OK**. Hub se znovu připojí a karta hubu zobrazí aktualizovanou verzi firmwaru.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_6.png')} alt="Laiteohjelmiston päivitys" />

Nyní můžete hub dál používat s MOCPilot.

## Pokud aktualizace selže

Pokud se aktualizace nedokončí úspěšně, MOCPilot zobrazí zprávu o selhání aktualizace firmwaru.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_7.png')} alt="Laiteohjelmiston päivitys" />

Nejprve zkuste hub vypnout a znovu zapnout a spustit aktualizaci znovu:

1. Vypněte hub.
2. Znovu zapněte hub.
3. Držte hub blízko zařízení.
4. Připojte hub v MOCPilot.
5. Znovu spusťte aktualizaci firmwaru.

Pokud hub nereaguje normálně, může být potřeba obnova firmwaru. Postupujte podle návodu [Obnova firmwaru hubu](/docs/Application/Hubs/RecoveryHubFirmware/).
