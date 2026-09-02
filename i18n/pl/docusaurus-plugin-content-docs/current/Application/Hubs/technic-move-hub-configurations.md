---
id: TechnicMoveHubConfigurations
title: Konfiguracje Technic Move Hub
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Konfiguracje Technic Move Hub

## Przegląd

Technic Move Hub wprowadził unikalną funkcję w rodzinie hubów LEGO Powered Up: hub może zmieniać swoje zachowanie w zależności od aktualnie zastosowanej konfiguracji.

MOCPilot pozwala zmienić konfigurację Technic Move Hub, aby zachowanie huba odpowiadało oficjalnemu zestawowi LEGO, którym chcesz sterować.

## Obsługiwane konfiguracje

Obecnie znane są następujące konfiguracje Technic Move Hub:

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Opcje konfiguracji Technic Move Hub" />

## Zmiana konfiguracji z Moje huby Bluetooth

Konfigurację możesz zmienić na stronie **Moje huby Bluetooth**:

1. Otwórz **Moje huby Bluetooth**.
2. Znajdź Technic Move Hub.
3. Otwórz menu kontekstowe huba.
4. Wybierz **Wybierz konfigurację**.
5. Wybierz wymaganą konfigurację.
6. Potwierdź okno rekonfiguracji.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Menu kontekstowe Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Podmenu konfiguracji Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Okno potwierdzenia rekonfiguracji Technic Move Hub" />

:::warning Ważne
Zmiana konfiguracji huba zapisuje w hubie podprogram i jest podobna do procesu aktualizacji firmware.

Pozostaw hub włączony przez cały proces. Telefon, tablet lub komputer powinien być zasilany i znajdować się blisko huba, aby połączenie Bluetooth było stabilne. Nie zamykaj MOCPilot, nie wyłączaj Bluetooth ani huba podczas zmiany konfiguracji.

Przerwanie zmiany konfiguracji może uszkodzić firmware huba. Jeśli tak się stanie, przed ponownym użyciem może być wymagane odzyskanie firmware. W razie potrzeby skorzystaj z instrukcji [odzyskiwania firmware huba](/docs/Application/Hubs/RecoveryHubFirmware/).
:::

Podczas rekonfiguracji hub nie odpowiada na zwykłe polecenia. Dioda LED miga stopniową kolorową sygnalizacją aż do zakończenia procesu. Po zastosowaniu nowej konfiguracji hub jest ponownie inicjalizowany.

## Bloki konfiguracji

MOCPilot zawiera także bloki do odczytu i zmiany konfiguracji Technic Move Hub podczas działania programu.

### Ustaw konfigurację huba

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Blok Ustaw konfigurację huba" />

Blok **Ustaw konfigurację huba** zmienia wybrany hub na jeden z obsługiwanych profili konfiguracji.

- Selektor huba: wybiera hub do rekonfiguracji.
- Selektor konfiguracji: wybiera konfigurację docelową.
- Dostępne konfiguracje dla Technic Move Hub: **Porsche GT4 e-Performance**, **Lamborghini Revuelto** i **Batmobile™ Tumbler**.

Zobacz [dokumentację bloku Ustaw konfigurację huba](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Konfiguracja huba

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Blok Konfiguracja huba" />

Blok **Konfiguracja huba** zgłasza bieżącą konfigurację wybranego huba.

- Selektor huba: wybiera hub do odczytu.
- Format wyjścia: **tekst** zwraca nazwę konfiguracji.
- Format wyjścia: **indeks** zwraca indeks konfiguracji, przydatny do porównań w warunkach.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Opcje formatu wyjścia bloku Konfiguracja huba" />

Zobacz [dokumentację bloku Konfiguracja huba](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Impuls mocy

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Blok Impuls mocy" />

Blok **Impuls mocy** wysyła polecenie impulsu mocy do wybranego Technic Move Hub. Ten blok działa tylko wtedy, gdy Technic Move Hub jest skonfigurowany jako **Batmobile™ Tumbler**.

Po uruchomieniu hub na krótko włącza silniki z maksymalną dostępną mocą i prędkością, zwykle na około 1-2 sekundy.

Zobacz [dokumentację bloku Impuls mocy](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Zmiana konfiguracji podczas działania programu

Konfigurację Technic Move Hub można również zmieniać podczas działania programu.

Typowy sposób działania:

1. Odczytaj bieżącą konfigurację huba.
2. Porównaj ją z konfiguracją wymaganą przez profil.
3. Jeśli konfiguracja jest inna, ustaw wymaganą konfigurację.
4. Odczytaj konfigurację ponownie po rekonfiguracji.
5. Kontynuuj tylko wtedy, gdy hub zgłasza oczekiwaną konfigurację.
6. Odłącz lub zatrzymaj program, jeśli wymagana konfiguracja nie została zastosowana.

Gotowy profil używający tego huba może służyć jako przykład takiego podejścia.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Przykład bloków pokazujący zmianę konfiguracji Technic Move Hub podczas działania" />
