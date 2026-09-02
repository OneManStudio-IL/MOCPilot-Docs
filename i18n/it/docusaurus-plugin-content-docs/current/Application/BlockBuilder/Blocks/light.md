---
id: Light
title: Luce
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Luce

Questa pagina documenta i blocchi della categoria Luce usati per controllare LED e uscite luminose sugli hub supportati.

## Blocchi luce comuni

### `Imposta colore LED` (Principiante) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Imposta il colore del LED dell'hub usando opzioni colore predefinite.

- Tipo: blocco comando
- Uso tipico: mostrare lo stato (pronto, in esecuzione, avviso, errore)

### `Luce imposta su` (Principiante) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Imposta l'uscita luce selezionata a una luminosità/valore target.

- Tipo: blocco comando
- Uso tipico: luminosità fari, intensità stato

### `Spegni luce` (Principiante) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Spegne l'uscita luce selezionata.

- Tipo: blocco comando
- Uso tipico: sequenza di spegnimento, risparmio batteria

### `Technic Move luce imposta su` (Principiante) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variante di `Luce imposta su` per target hub/luce Technic Move.

- Tipo: blocco comando
- Uso tipico: impostare il livello di uscita luce dell'hub Move

## Blocchi matrice LED interna

### `Accendi matrice luminosa` (Avanzato) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Mostra l'immagine selezionata sulla matrice LED interna dell'hub e passa subito al blocco successivo nella pila. L'immagine resta sul display finché un altro blocco non modifica la matrice LED interna o il programma si ferma.

- Tipo: blocco comando
- Nota: l'hub selezionato deve avere una matrice LED interna.

### `Scrivi sulla matrice luminosa` (Principiante) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Mostra una stringa di testo sulla matrice LED interna dell'hub facendo scorrere una lettera alla volta.

- Tipo: blocco comando
- Nota: l'hub selezionato deve avere una matrice LED interna.

### `Spegni pixel matrice` (Principiante) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Spegne tutte le luci sulla matrice LED interna dell'hub.

- Tipo: blocco comando
- Nota: l'hub selezionato deve avere una matrice LED interna.

### `Imposta pixel matrice` (Avanzato) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Imposta la luminosità di un pixel sulla matrice LED interna dell'hub. Viene aggiornato solo il pixel selezionato; il resto del display rimane invariato. I campi della posizione del pixel usano valori di colonna e riga, con il pixel `1, 1` nell'angolo in alto a sinistra.

- Tipo: blocco comando
- Nota: l'hub selezionato deve avere una matrice LED interna.

### `Ruota orientamento matrice` (Avanzato) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Ruota l'orientamento di ciò che viene mostrato sulla matrice LED interna dell'hub in senso orario o antiorario. Ogni rotazione cambia l'orientamento del display di 90 gradi e influisce sui blocchi Luce eseguiti dopo.

- Tipo: blocco comando
- Nota: l'hub selezionato deve avere una matrice LED interna.

### `Imposta orientamento matrice` (Avanzato) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Imposta l'orientamento di ciò che viene mostrato sulla matrice LED interna dell'hub. L'orientamento predefinito è verticale e l'orientamento selezionato influisce sui blocchi Luce eseguiti dopo.

- Tipo: blocco comando
- Opzioni di orientamento: `verticale`, `sinistra`, `destra`, `capovolto`
- Nota: l'hub selezionato deve avere una matrice LED interna.

## Blocchi luce del sensore di distanza

### `Illumina sensore di distanza` (Principiante) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Imposta le luci sul sensore di distanza selezionato. Il blocco può accendere o spegnere le singole luci del sensore e può usare un blocco reporter lista per controllare la luminosità di ogni luce.

- Tipo: blocco comando
- Nota: disponibile solo per l'hub MINDSTORMS Robot Inventor.

## Blocchi luce BuWizz 3

### `BuWizz 3 imposta colore LED` (Principiante) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Imposta il colore LED sulla porta BuWizz 3 selezionata con opzioni colore integrate.

- Tipo: blocco comando

### `BuWizz 3 imposta colore LED (stringa)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Imposta il colore LED BuWizz 3 usando un valore colore testuale.

- Tipo: blocco comando
- Uso tipico: nomi colore dinamici da variabili

### `BuWizz 3 imposta colore LED (RGB)` (Avanzato) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Imposta il colore LED BuWizz 3 usando canali RGB espliciti.

- Tipo: blocco comando
- Uso tipico: controllo colore completamente personalizzato e gradienti
