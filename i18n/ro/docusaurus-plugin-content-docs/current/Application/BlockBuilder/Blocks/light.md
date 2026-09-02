---
id: Light
title: Lumină
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Lumină

Această pagină documentează blocurile din categoria Lumină utilizate pentru a controla LED-urile și ieșirile de lumină pe hub-urile compatibile.

## Blocuri comune de lumină

### `Setează culoarea LED-ului` (Începător) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Setează culoarea LED-ului hub-ului folosind opțiuni de culori predefinite.

- Tip: bloc de comandă
- Utilizare tipică: afișarea stării (gata, în execuție, avertizare, eroare)

### `Setează lumina la` (Începător) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Setează ieșirea de lumină selectată la o valoare/inten­sitate țintă.

- Tip: bloc de comandă
- Utilizare tipică: luminozitatea farurilor, intensitatea stării

### `Oprește lumina` (Începător) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Oprește ieșirea de lumină selectată.

- Tip: bloc de comandă
- Utilizare tipică: secvență de oprire, economisire baterie

### `Technic Move setează lumina la` (Începător) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variantă a blocului `Setează lumina la` pentru hub-ul/lumina Technic Move.

- Tip: bloc de comandă
- Utilizare tipică: setarea nivelului de lumină pentru hub-ul Move

## Blocuri pentru matricea LED internă

### `Pornește matricea de lumini` (Avansat) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Afișează imaginea selectată pe matricea LED internă a hubului și trece imediat la următorul bloc din stivă. Imaginea rămâne pe afișaj până când un alt bloc modifică matricea LED internă sau programul se oprește.

- Tip: bloc de comandă
- Notă: hubul selectat trebuie să aibă o matrice LED internă.

### `Scrie pe matricea de lumini` (Începător) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Afișează un șir de text pe matricea LED internă a hubului, derulând câte o literă pe rând.

- Tip: bloc de comandă
- Notă: hubul selectat trebuie să aibă o matrice LED internă.

### `Oprește pixelii matricei` (Începător) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Oprește toate luminile de pe matricea LED internă a hubului.

- Tip: bloc de comandă
- Notă: hubul selectat trebuie să aibă o matrice LED internă.

### `Setează pixelul matricei` (Avansat) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Setează luminozitatea unui pixel pe matricea LED internă a hubului. Numai pixelul selectat este actualizat; restul afișajului rămâne neschimbat. Câmpurile de poziție ale pixelului folosesc valori de coloană și rând, cu pixelul `1, 1` în colțul din stânga sus.

- Tip: bloc de comandă
- Notă: hubul selectat trebuie să aibă o matrice LED internă.

### `Rotește orientarea matricei` (Avansat) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Rotește orientarea conținutului afișat pe matricea LED internă a hubului în sens orar sau antiorar. Fiecare rotație schimbă orientarea afișajului cu 90 de grade și afectează blocurile de Lumină rulate după ea.

- Tip: bloc de comandă
- Notă: hubul selectat trebuie să aibă o matrice LED internă.

### `Setează orientarea matricei` (Avansat) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Setează orientarea conținutului afișat pe matricea LED internă a hubului. Orientarea implicită este verticală, iar orientarea selectată afectează blocurile de Lumină rulate după ea.

- Tip: bloc de comandă
- Opțiuni de orientare: `vertical`, `stânga`, `dreapta`, `cu susul în jos`
- Notă: hubul selectat trebuie să aibă o matrice LED internă.

## Blocuri de lumină pentru senzorul de distanță

### `Aprinde senzorul de distanță` (Începător) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Setează luminile de pe senzorul de distanță selectat. Blocul poate porni sau opri luminile individuale ale senzorului și poate folosi un bloc reporter de listă pentru a controla luminozitatea fiecărei lumini.

- Tip: bloc de comandă
- Notă: disponibil numai pentru hubul MINDSTORMS Robot Inventor.

## Blocuri de lumină BuWizz 3

### `BuWizz 3 setează culoarea LED-ului` (Începător) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Setează culoarea LED-ului pe portul BuWizz 3 selectat folosind opțiuni de culori integrate.

- Tip: bloc de comandă

### `BuWizz 3 setează culoarea LED-ului (text)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Setează culoarea LED-ului BuWizz 3 folosind o valoare de culoare sub formă de text.

- Tip: bloc de comandă
- Utilizare tipică: utilizarea dinamică a numelor de culori din variabile

### `BuWizz 3 setează culoarea LED-ului (RGB)` (Avansat) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Setează culoarea LED-ului BuWizz 3 folosind canale RGB explicite.

- Tip: bloc de comandă
- Utilizare tipică: control complet al culorii și gradienți
