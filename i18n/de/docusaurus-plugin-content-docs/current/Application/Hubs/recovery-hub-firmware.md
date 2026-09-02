---
id: RecoveryHubFirmware
title: Hub-Firmware wiederherstellen
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Hub-Firmware wiederherstellen

Die Hub-Firmware-Wiederherstellung wird verwendet, wenn ein Hub nach einer unterbrochenen oder fehlgeschlagenen Firmware-Aktualisierung nicht normal startet.

Während der Wiederherstellung stellt MOCPilot den Firmware-Pfad des Hubs wieder her, damit der Hub erneut auf die neueste unterstützte Version aktualisiert werden kann. Verwenden Sie diesen Vorgang nur, wenn der Hub nicht normal reagiert, MOCPilot den Wiederherstellungsmodus meldet oder eine vorherige Aktualisierung fehlgeschlagen ist.

:::warning Wichtig
Lassen Sie den Hub eingeschaltet und halten Sie Ihr Gerät während der gesamten Wiederherstellung nahe am Hub. Das Trennen von Bluetooth, Schließen von MOCPilot, Entfernen der Batterien oder Ausschalten des Hubs während des Firmware-Uploads kann die Wiederherstellung fehlschlagen lassen.
:::

## Wann eine Wiederherstellung erforderlich ist

Eine Firmware-Wiederherstellung kann erforderlich sein, wenn:

- Eine Firmware-Aktualisierung nicht erfolgreich abgeschlossen wurde.
- Der Hub verbindet sich nicht mehr als normaler Hub.
- Hub se v MOCPilot zobrazí jako **LEGO Bootloader**.
- MOCPilot erkennt, dass der Hub im Firmware-Wiederherstellungsmodus verbunden ist.

Stellen Sie vor dem Start sicher, dass der Hub genug Batterieladung hat. Wenn möglich, stellen Sie auch sicher, dass Telefon, Tablet oder Computer mit MOCPilot geladen ist und Bluetooth aktiviert ist.

## Unterstützte Hubs

Die Firmware-Wiederherstellung wird für dieselben Hubs unterstützt wie die Firmware-Aktualisierung:

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(160px, 1fr))', gap: '16px', margin: '16px 0 24px'}}>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/technic_hub_p.webp')} alt="Technic Hub" style={{maxWidth: '140px'}} /><div><strong>Technic Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/city_hub_p.webp')} alt="City Hub" style={{maxWidth: '140px'}} /><div><strong>City Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/boost_hub_p.webp')} alt="Boost Hub" style={{maxWidth: '140px'}} /><div><strong>Boost Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/technic_move_hub_p.webp')} alt="Technic Move Hub" style={{maxWidth: '140px'}} /><div><strong>Technic Move Hub</strong></div></div>
</div>

## Technic Hub, Boost Hub und City Hub in den Wiederherstellungsmodus versetzen

Technic Hub, Boost Hub und der kleine City Hub verwenden den Verbindungsablauf über den bootloader:

1. Schalten Sie den Hub aus.
2. Halten Sie die grüne Taste gedrückt.
3. Halten Sie die Taste weiter gedrückt, bis die LED des Hubs violett blinkt.
4. Lassen Sie die Taste nicht los, während die LED violett blinkt.
5. Halten Sie die Taste weiter gedrückt, öffnen Sie **Meine Bluetooth-Hubs** in MOCPilot und verbinden Sie sich mit dem Hub.
6. Nachdem der Hub im bootloader-Modus verbunden ist, können Sie die Taste loslassen.

Im Wiederherstellungsmodus kann der Hub als **LEGO Bootloader** statt mit seinem normalen Namen erscheinen.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="LEGO Bootloader" />

## Technic Move Hub in den Wiederherstellungsmodus versetzen

Technic Move Hub verwendet eine andere Wiederherstellungssequenz als die anderen unterstützten Hubs. Er verbindet sich nicht als **LEGO Bootloader**. Stattdessen lädt diese Sequenz die Werksfirmware **1.2.3**, die nicht als finale Firmware für den normalen Gebrauch vorgesehen ist.

So stellen Sie die Firmware von Technic Move Hub wieder her:

1. Schalten Sie den Hub aus.
2. Halten Sie die grüne Taste gedrückt.
3. Halten Sie die grüne Taste etwa eine Minute lang gedrückt.
4. Lassen Sie die Taste los.
5. Warten Sie, bis die LED des Hubs weiß blinkt.
6. Öffnen Sie **Meine Bluetooth-Hubs** in MOCPilot und verbinden Sie sich mit dem Hub.

Nach dem Verbinden erkennt MOCPilot die Werksfirmware und bietet an, den Hub auf die neueste verfügbare Version zu aktualisieren. Starten Sie die Firmware-Aktualisierung und warten Sie, bis sie abgeschlossen ist.

## Wiederherstellung aus dem Dialog starten

Wenn MOCPilot einen Hub im Firmware-Wiederherstellungsmodus erkennt, zeigt die App einen Wiederherstellungsdialog.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_1.png')} alt="Hub-Firmware wiederherstellen" />

Wählen Sie **Wiederherstellen**, um den Firmware-Upload auf den Hub zu starten.

Wenn Sie die Wiederherstellung noch nicht starten möchten, wählen Sie **Abbrechen**. Sie können die Wiederherstellung später über das Kontextmenü des Hubs starten.

## Wiederherstellung über das Hub-Menü starten

So starten Sie die Wiederherstellung manuell:

1. Öffnen Sie **Meine Bluetooth-Hubs**.
2. Suchen Sie den Hub, der als **LEGO Bootloader** angezeigt wird.
3. Öffnen Sie das Kontextmenü des Hubs.
4. Wählen Sie **Hub-Firmware wiederherstellen**.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_2.png')} alt="Hub-Firmware wiederherstellen" />

## Während der Firmware-Wiederherstellung

Nach dem Start der Wiederherstellung lädt MOCPilot Firmware auf den Hub. Die App zeigt den Fortschritt auf dem Bildschirm.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_3.png')} alt="Hub-Firmware wiederherstellen" />

Warten Sie, bis der Vorgang abgeschlossen ist. Entfernen Sie den Hub nicht von Ihrem Gerät, schließen Sie die App nicht, deaktivieren Sie Bluetooth nicht und trennen Sie den Hub nicht von der Stromversorgung.

Der Hub kann während des Vorgangs mehrmals neu starten oder sich neu verbinden. Das ist erwartet. Lassen Sie MOCPilot geöffnet und warten Sie, bis die Wiederherstellung abgeschlossen ist.

## Wiederherstellung abschließen

Wenn die Wiederherstellung erfolgreich abgeschlossen ist, zeigt MOCPilot einen Bestätigungsdialog.

<img src={useBaseUrl('/img/hubs/firmware-recovery/fur_4.png')} alt="Hub-Firmware wiederherstellen" />

Wählen Sie **OK**. Der Hub sollte neu starten und sich als normaler Hub statt als **LEGO Bootloader** verbinden.

Prüfen Sie den Hub nach der Wiederherstellung in **Meine Bluetooth-Hubs**. Wenn MOCPilot weiterhin meldet, dass eine Firmware-Aktualisierung erforderlich ist, führen Sie den normalen Prozess [Firmware aktualisieren](/docs/Application/Hubs/FirmwareUpdating/) aus.

## Wenn die Wiederherstellung fehlschlägt

Wenn die Wiederherstellung nicht erfolgreich abgeschlossen wird:

1. Halten Sie den Hub nahe bei Ihrem Gerät.
2. Schalten Sie den Hub aus und wieder ein.
3. Versetzen Sie den Hub erneut in den Wiederherstellungsmodus.
4. Verbinden Sie sich in MOCPilot mit **LEGO Bootloader**.
5. Starten Sie **Hub-Firmware wiederherstellen** erneut.

Wenn die Fehlermeldung erneut erscheint, wiederholen Sie den Wiederherstellungsvorgang von Anfang an. Wenn der Hub nach mehreren Versuchen weiterhin nicht wiederhergestellt werden kann, ersetzen oder laden Sie die Batterien und versuchen Sie es erneut.
