---
id: AboutApp
title: O MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Zbuduj. Prowadź. Kontroluj wszystko.

**MOCPilot** — aplikacja do tworzenia własnych profili sterowania dla LEGO® i zgodnych konstrukcji Bluetooth.

Daje konstruktorom jedno miejsce do łączenia hubów, sterowania silnikami, odczytu czujników, projektowania pulpitów i tworzenia programów wizualnych dla modeli, mechanizmów, samochodów, ciężarówek, pociągów, robotów i własnych MOC.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="Aplikacja MOCPilot na telefonie" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Co daje MOCPilot</h2>
    <ul>
      <li>Własne profile dla twoich modeli.</li>
      <li>Gotowe profile dla obsługiwanych oficjalnych zestawów.</li>
      <li>Łączenie i zarządzanie hubami Bluetooth.</li>
      <li>Programowanie wizualne blokami dla automatyzacji i logiki.</li>
      <li>Kontrolery pulpitu do jazdy i obsługi modeli.</li>
      <li>Obsługa LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, silników, czujników i zgodnych urządzeń Bluetooth.</li>
    </ul>
  </div>
</div>

## Pomysł

Większość zmotoryzowanych konstrukcji potrzebuje więcej niż prostego pilota. Samochód może wymagać skrętu, gazu, świateł, monitorowania baterii, sekwencji skrzyni biegów albo specjalnej procedury startowej. Robot może potrzebować czujników, zdarzeń, logiki warunkowej i kilku współpracujących hubów.

MOCPilot jest zaprojektowany dla przestrzeni między prostym pilotem a pełnym środowiskiem programowania. Możesz zacząć od prowadzenia modelu z pulpitu ekranowego, a potem dodawać logikę, czujniki i automatyzację.

## Profile

**Profil** jest centrum sterowania jednego modelu.

W profilu możesz wybrać huby należące do modelu, utworzyć program uruchamiający model i zaprojektować pulpit używany do sterowania.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="Strona profili MOCPilot" width="420" />

<details>
<summary>Profile gotowe</summary>

Gotowe profile to przygotowane przykłady dla obsługiwanych oficjalnych zestawów. Przydają się, gdy chcesz szybko zacząć albo zobaczyć, jak zbudowany jest działający profil.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Gotowe profile MOCPilot" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Gotowy program blokowy MOCPilot" width="1100" />

</details>

<details>
<summary>Profile własne</summary>

Własne profile są przeznaczone dla twoich MOC i eksperymentów. Możesz utworzyć profil, dodać huby, podłączyć silniki i czujniki, zbudować program oraz zaprojektować pulpit pasujący do konkretnego modelu.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Tworzenie własnego profilu MOCPilot" width="420" />

</details>

## Łączenie hubów i urządzeń

MOCPilot może łączyć się z obsługiwanymi hubami Bluetooth i zgodnymi urządzeniami, a potem udostępniać je w profilu.

Dla prostej konstrukcji możesz użyć profilu z jednym hubem albo podłączyć kilka hubów, gdy model wymaga większej liczby portów, oddzielnych systemów zasilania lub niezależnych modułów.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Strona Moje huby Bluetooth w MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Połączone huby Bluetooth w MOCPilot" width="1100" />

<details>
<summary>Przykłady obsługiwanego sprzętu</summary>

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

Pełną listę znajdziesz na stronie [obsługiwane huby, silniki i czujniki](/docs/Introducing/SupportedDevices/).

</details>

## Budowanie logiki blokami

MOCPilot zawiera wizualny kreator bloków. Programy można tworzyć przez łączenie bloków zamiast pisania kodu.

Bloki mogą reagować na zdarzenia, sterować silnikami, odczytywać czujniki, pracować ze zmiennymi, używać wejścia z gamepada, aktualizować kontrolery pulpitu i koordynować kilka akcji.

MOCPilot w pełni obsługuje podłączone fizyczne gamepady. Bloki gamepada odczytują przyciski, spusty, kierunki D-pad i drążki, więc możesz przypisać prawdziwy kontroler do modelu, gdy sterowanie fizyczne jest wygodniejsze niż ekran dotykowy.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="Program użytkownika MOCPilot zbudowany z bloków" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Blok uruchomienia programu" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Blok uruchomienia silnika z prędkością" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Blok poziomu baterii huba" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Blok wartości kierownicy" />
</div>

<details>
<summary>Co można zrobić programami blokowymi</summary>

- Uruchamiać, zatrzymywać i skręcać silniki.
- Odczytywać poziom baterii, napięcie, przechył, orientację, temperaturę i wartości czujników.
- Konfigurować fizyczny gamepad do skrętu, gazu, spustów, akcji i zmiany trybów.
- Reagować na zmiany przycisków, czujników, timerów lub kontrolerów pulpitu.
- Tworzyć kontrole startowe przed rozpoczęciem ruchu modelu.
- Dodawać własną logikę dla świateł, kalibracji skrętu, trybów mocy i konfiguracji huba.
- Używać zmiennych, list, warunków, pętli, komunikatów i własnych bloków do organizacji złożonego zachowania.

</details>

## Projektowanie pulpitu jazdy

Pulpit to ekran używany podczas sterowania modelem. Może zawierać kierownice, joysticki, suwaki, przyciski, przełączniki, pedały, monitory i inne kontrolery.

Kontrolery pulpitu i wejścia fizycznego gamepada można łączyć z blokami oraz akcjami huba, aby interfejs pasował do modelu.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="Kontrolery pulpitu MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="Ekran sterowania MOCPilot z kierownicą i pedałami" width="1100" />

<details>
<summary>Przykłady pulpitów</summary>

- Użyj kierownicy i pedałów dla samochodów.
- Użyj suwaków dla dźwigów, podnośników i siłowników liniowych.
- Użyj przycisków do świateł, klaksonu, zmiany biegów lub akcji skryptowych.
- Użyj monitorów do pokazywania baterii, prędkości, wartości czujników lub własnego stanu programu.
- Użyj podłączonego gamepada, jeśli wolisz fizyczne przyciski, drążki i spusty od ekranu dotykowego.

</details>

## Utrzymanie zaawansowanych konstrukcji pod kontrolą

Gdy model rośnie, profil może rosnąć razem z nim. MOCPilot obsługuje logikę wielokrotnego użytku przez **My Blocks**, konfigurację hubów dla konkretnego profilu, wiele kontrolerów i przepływy programu łączące sterowanie ręczne z automatyzacją.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Przykład użycia My Blocks w MOCPilot" width="1100" />

Pomaga to utrzymać czytelność dużych programów. Na przykład profil może mieć osobny blok do aktualizacji baterii, drugi do kalibracji skrętu i kolejny do specjalnego trybu jazdy.

## Typowy przepływ pracy

1. Utwórz lub otwórz profil.
2. Dodaj huby Bluetooth i urządzenia używane przez model.
3. Zbuduj program z bloków.
4. Zaprojektuj pulpit do jazdy i interakcji.
5. Naciśnij **Play**.
6. Testuj, dostrajaj i ulepszaj profil, aż model będzie zachowywał się tak, jak chcesz.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Przepływ łączenia huba w MOCPilot" width="1100" />

## Dla kogo jest MOCPilot

MOCPilot przydaje się konstruktorom, którzy chcą:

- Lepszego pilota do zmotoryzowanych modeli LEGO®.
- Sposobu sterowania zgodnymi hubami Bluetooth firm trzecich.
- Wizualnego środowiska programowania dla mechanizmów i robotów.
- Gotowych profili dla obsługiwanych oficjalnych zestawów.
- Własnych pulpitów dla samochodów, ciężarówek, pociągów, crawlerów, dźwigów i innych MOC.
- Jednej aplikacji łączącej huby, silniki, czujniki, gamepady i sterowanie ekranowe.

## Zacznij odkrywać

- Skorzystaj z [samouczka szybkiego startu](/docs/Introducing/QuickStart/), aby zbudować pierwszy profil.
- Sprawdź [obsługiwane urządzenia](/docs/Introducing/SupportedDevices/) przed wyborem sprzętu.
- Poznaj [dokumentację BlockBuilder](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/), gdy chcesz dodać logikę.
- Zobacz [aktualizację firmware huba](/docs/Application/Hubs/FirmwareUpdating/), jeśli hub wymaga obsługiwanej wersji firmware.
