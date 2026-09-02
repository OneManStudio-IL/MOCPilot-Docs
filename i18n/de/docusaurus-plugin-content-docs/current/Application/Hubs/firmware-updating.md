---
id: FirmwareUpdating
title: Firmware aktualisieren
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Firmware aktualisieren

MOCPilot kann die Firmware unterstützter LEGO Powered Up Hubs aktualisieren, wenn eine neuere kompatible Version verfügbar ist.

Eine Firmware-Aktualisierung kann erforderlich sein, damit ein Hub korrekt mit MOCPilot arbeitet. Neuere Firmware kann die Kompatibilität verbessern, das Verhalten des Hubs korrigieren und die erwarteten Funktionen dieses Modells verfügbar machen.

## Die Firmware-Aktualisierung wird derzeit für diese Hubs unterstützt

Die Firmware-Aktualisierung wird derzeit für diese Hubs unterstützt:

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(160px, 1fr))', gap: '16px', margin: '16px 0 24px'}}>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/technic_hub_p.webp')} alt="Technic Hub" style={{maxWidth: '140px'}} /><div><strong>Technic Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/city_hub_p.webp')} alt="City Hub" style={{maxWidth: '140px'}} /><div><strong>City Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/boost_hub_p.webp')} alt="Boost Hub" style={{maxWidth: '140px'}} /><div><strong>Boost Hub</strong></div></div>
  <div style={{textAlign: 'center'}}><img src={useBaseUrl('/img/devices/technic_move_hub_p.webp')} alt="Technic Move Hub" style={{maxWidth: '140px'}} /><div><strong>Technic Move Hub</strong></div></div>
</div>

## Vor dem Start

Stellen Sie vor dem Start sicher, dass der Hub und das Gerät mit MOCPilot ausreichend geladen sind.

Lassen Sie den Hub während des gesamten Vorgangs eingeschaltet und halten Sie Telefon, Tablet oder Computer nahe am Hub, damit die Bluetooth-Verbindung stabil bleibt. Schließen Sie MOCPilot nicht, deaktivieren Sie Bluetooth nicht und schalten Sie den Hub während des Uploads nicht aus.

:::warning Wichtig
Das Unterbrechen einer Firmware-Aktualisierung kann die Hub-Firmware in einem unvollständigen Zustand belassen. Dann kann eine Firmware-Wiederherstellung erforderlich sein, bevor der Hub wieder verwendet werden kann.
:::

## Aktualisierung starten

Beim Verbinden eines Hubs prüft MOCPilot die installierte Firmware-Version. Wenn eine neuere Version erforderlich ist, zeigt die App einen Dialog zur Firmware-Aktualisierung.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_1.png')} alt="Firmware aktualisieren" />

Wählen Sie **Aktualisieren**, um die Firmware-Aktualisierung sofort zu starten.

Wenn Sie jetzt nicht aktualisieren möchten, wählen Sie **Abbrechen**. Sie können die Aktualisierung später über das Kontextmenü des Hubs starten.

## Später über das Hub-Menü aktualisieren

So starten Sie die Firmware-Aktualisierung manuell:

1. Öffnen Sie **Meine Bluetooth-Hubs**.
2. Suchen Sie den Hub, der aktualisiert werden muss.
3. Öffnen Sie das Kontextmenü des Hubs.
4. Wählen Sie **Firmware aktualisieren**.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_2.png')} alt="Firmware aktualisieren" />

## Während der Firmware-Aktualisierung

Nach dem Start lädt MOCPilot die Firmware auf den Hub und zeigt den Fortschritt.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_3.png')} alt="Firmware aktualisieren" />

Warten Sie, bis der Upload abgeschlossen ist. Der Hub kann neu starten oder vorübergehend getrennt werden, während die neue Firmware angewendet wird.

Nachdem die Firmware hochgeladen wurde, sucht MOCPilot erneut nach dem Hub. Halten Sie den Hub in der Nähe und warten Sie, bis die App die Verbindung wiederherstellt.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_4.png')} alt="Firmware aktualisieren" />

## Aktualisierung abschließen

Wenn die Aktualisierung erfolgreich abgeschlossen ist, zeigt MOCPilot einen Bestätigungsdialog.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_5.png')} alt="Firmware aktualisieren" />

Wählen Sie **OK**. Der Hub verbindet sich erneut, und die Hub-Karte zeigt die aktualisierte Firmware-Version.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_6.png')} alt="Firmware aktualisieren" />

Sie können den Hub nun weiter mit MOCPilot verwenden.

## Wenn die Aktualisierung fehlschlägt

Wenn die Aktualisierung nicht erfolgreich abgeschlossen wird, zeigt MOCPilot eine Fehlermeldung zur Firmware-Aktualisierung.

<img src={useBaseUrl('/img/hubs/firmware-updating/fu_7.png')} alt="Firmware aktualisieren" />

Versuchen Sie zuerst, den Hub aus- und wieder einzuschalten und die Aktualisierung erneut auszuführen:

1. Schalten Sie den Hub aus.
2. Schalten Sie den Hub wieder ein.
3. Halten Sie den Hub nahe bei Ihrem Gerät.
4. Verbinden Sie den Hub in MOCPilot.
5. Starten Sie die Firmware-Aktualisierung erneut.

Wenn der Hub nicht normal reagiert, kann eine Firmware-Wiederherstellung erforderlich sein. Folgen Sie der Anleitung [Hub-Firmware wiederherstellen](/docs/Application/Hubs/RecoveryHubFirmware/) für detaillierte Schritte.
