---
id: TechnicMoveHubConfigurations
title: Configurații Technic Move Hub
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Configurații Technic Move Hub

## Prezentare generală

Technic Move Hub a introdus o funcție unică în familia de huburi LEGO Powered Up: hubul își poate schimba comportamentul în funcție de configurația aplicată în prezent.

MOCPilot îți permite să schimbi configurația Technic Move Hub astfel încât comportamentul hubului să corespundă setului LEGO oficial pe care vrei să îl controlezi.

## Configurații acceptate

În acest moment, sunt cunoscute aceste configurații Technic Move Hub:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Opțiuni de configurare pentru Technic Move Hub" />

## Schimbarea configurației din Huburile mele Bluetooth

Poți schimba configurația din pagina **Huburile mele Bluetooth**:

1. Deschide **Huburile mele Bluetooth**.
2. Găsește Technic Move Hub.
3. Deschide meniul contextual al hubului.
4. Selectează **Selectează configurația**.
5. Alege configurația necesară.
6. Confirmă dialogul de reconfigurare.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Meniul contextual al Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Submeniul de configurare al Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Dialog de confirmare a reconfigurării Technic Move Hub" />

:::warning Important
Schimbarea configurației hubului scrie un subprogram în hub și este similară cu un proces de actualizare firmware.

Păstrează hubul pornit pe tot parcursul procesului. Ține telefonul, tableta sau computerul pornit și aproape de hub, astfel încât conexiunea Bluetooth să rămână stabilă. Nu închide MOCPilot, nu opri Bluetooth și nu opri hubul în timp ce configurația este schimbată.

Întreruperea schimbării configurației poate deteriora firmware-ul hubului. Dacă se întâmplă acest lucru, poate fi necesară recuperarea firmware-ului înainte ca hubul să poată fi folosit din nou. Urmează ghidul de [recuperare a firmware-ului hubului](/docs/Application/Hubs/RecoveryHubFirmware/) dacă este necesară recuperarea.
:::

În timpul reconfigurării, hubul nu răspunde la comenzi normale. LED-ul clipește cu o indicație colorată în pași până când procesul se termină. După aplicarea noii configurații, hubul este reinițializat.

## Blocuri de configurare

MOCPilot include și blocuri pentru citirea și schimbarea configurației Technic Move Hub în timpul unui program.

### Setează configurația hubului

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Blocul Setează configurația hubului" />

Blocul **Setează configurația hubului** schimbă hubul selectat la unul dintre profilurile sale de configurare acceptate.

- Selector hub: alege hubul de reconfigurat.
- Selector configurație: alege configurația țintă.
- Configurații disponibile pentru Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** și **Batmobile™ Tumbler**.

Consultă [documentația blocului Setează configurația hubului](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Configurația hubului

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Blocul Configurația hubului" />

Blocul **Configurația hubului** raportează configurația curentă a hubului selectat.

- Selector hub: alege hubul de citit.
- Format ieșire: **text** returnează numele configurației.
- Format ieșire: **indice** returnează indicele configurației, util pentru comparații în condiții.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Opțiuni de format de ieșire ale blocului Configurația hubului" />

Consultă [documentația blocului Configurația hubului](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Impuls de putere

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Blocul Impuls de putere" />

Blocul **Impuls de putere** trimite o comandă de impuls de putere către Technic Move Hub selectat. Acest bloc funcționează numai când Technic Move Hub este configurat ca **Batmobile™ Tumbler**.

Când rulează, hubul pornește motoarele cu puterea și viteza maximă disponibile pentru o perioadă scurtă, de obicei aproximativ 1-2 secunde.

Consultă [documentația blocului Impuls de putere](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Schimbarea configurației în timpul rulării programului

Este posibilă și schimbarea configurației Technic Move Hub în timpul rulării unui program.

Abordarea obișnuită este:

1. Citește configurația curentă a hubului.
2. Compar-o cu configurația cerută de profil.
3. Dacă configurația este diferită, setează configurația cerută.
4. Citește din nou configurația după reconfigurare.
5. Continuă numai când hubul raportează configurația așteptată.
6. Deconectează sau oprește programul dacă configurația cerută nu a fost aplicată.

Profilul predefinit care folosește acest hub poate fi folosit ca referință pentru această abordare.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Exemplu de blocuri pentru schimbarea configurației Technic Move Hub în timpul rulării" />
