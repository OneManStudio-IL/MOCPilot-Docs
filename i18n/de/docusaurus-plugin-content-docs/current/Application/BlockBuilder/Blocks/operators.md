---
id: Operators
title: Operatoren
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Operatoren

Operatoren sind Reporter- und boolesche Blöcke für Berechnungen, Vergleiche, Logik und Textverarbeitung.

## Arithmetische Operatoren

### `Plus` (Anfänger) {#block_operator_plus}

<img src={useBaseUrl('/img/blocks/block_operator_plus.svg')} alt="block_operator_plus.svg" />

Gibt die Summe zweier Werte zurück.

### `Minus` (Anfänger) {#block_operator_minus}

<img src={useBaseUrl('/img/blocks/block_operator_minus.svg')} alt="block_operator_minus.svg" />

Gibt das Ergebnis der Subtraktion zweier Werte zurück.

### `Multiplizieren` (Anfänger) {#block_operator_multiply}

<img src={useBaseUrl('/img/blocks/block_operator_multiply.svg')} alt="block_operator_multiply.svg" />

Gibt das Produkt zweier Werte zurück.

### `Dividieren` (Anfänger) {#block_operator_divide}

<img src={useBaseUrl('/img/blocks/block_operator_divide.svg')} alt="block_operator_divide.svg" />

Gibt das Ergebnis der Division zweier Werte zurück.

### `Modulo` (Guru) {#block_operator_modulus}

<img src={useBaseUrl('/img/blocks/block_operator_modulus.svg')} alt="block_operator_modulus.svg" />

Gibt den Rest einer Division zurück.

### `Runden` (Guru) {#block_operator_round}

<img src={useBaseUrl('/img/blocks/block_operator_round.svg')} alt="block_operator_round.svg" />

Rundet auf die nächste ganze Zahl (z. B. `2.6 -> 3`).

### `Math single` (Guru) {#block_operator_math_single}

<img src={useBaseUrl('/img/blocks/block_operator_math_single.svg')} alt="block_operator_math_single.svg" />

Wendet eine mathematische Funktion mit einem Argument an.

Verfügbare Funktionen:

- `absoluter Wert`: absoluter Wert einer Zahl
- `abrunden`: auf die nächstkleinere ganze Zahl runden
- `aufrunden`: auf die nächstgrößere ganze Zahl runden
- `Wurzel`: Quadratwurzel
- `sin`: Sinus (winkelbasiert)
- `cos`: Kosinus (winkelbasiert)
- `tan`: Tangens (winkelbasiert)
- `asin`: Arkussinus
- `acos`: Arkuskosinus
- `atan`: Arkustangens
- `ln`: natürlicher Logarithmus (Basis `e`)
- `log`: Logarithmus zur Basis `10`
- `e^`: `e` hoch Eingabewert
- `10^`: `10` hoch Eingabewert

### `Math pair` (Guru) {#block_operator_math_pair}

<img src={useBaseUrl('/img/blocks/block_operator_math_pair.svg')} alt="block_operator_math_pair.svg" />

Wendet eine mathematische Funktion mit zwei Argumenten an.

Verfügbare Funktionen:

- `min`: der kleinere von zwei Werten
- `max`: der größere von zwei Werten
- `Potenz`: erster Wert hoch zweiter Wert
- `atan2`: Winkel aus X/Y-Wertepaar
- `hypot`: Hypotenusenlänge aus zwei Komponenten
- `copysign`: erster Wert mit Vorzeichen des zweiten Werts

### `Zufallszahl` (Guru) {#block_operator_pick_random}

<img src={useBaseUrl('/img/blocks/block_operator_pick_random.svg')} alt="block_operator_pick_random.svg" />

Gibt eine Zufallszahl im gewählten Bereich zurück.

## Vergleichsoperatoren

### `Gleich` (Anfänger) {#block_operator_equal}

<img src={useBaseUrl('/img/blocks/block_operator_equal.svg')} alt="block_operator_equal.svg" />

Gibt `true` zurück, wenn zwei Werte gleich sind.

### `Ungleich` (Fortgeschritten) {#block_operator_not_equal}

<img src={useBaseUrl('/img/blocks/block_operator_not_equal.svg')} alt="block_operator_not_equal.svg" />

Gibt `true` zurück, wenn zwei Werte ungleich sind.

### `Größer als` (Anfänger) {#block_operator_greater_than}

<img src={useBaseUrl('/img/blocks/block_operator_greater_than.svg')} alt="block_operator_greater_than.svg" />

Gibt `true` zurück, wenn der linke Wert größer als der rechte ist.

### `Kleiner als` (Anfänger) {#block_operator_less_than}

<img src={useBaseUrl('/img/blocks/block_operator_less_than.svg')} alt="block_operator_less_than.svg" />

Gibt `true` zurück, wenn der linke Wert kleiner als der rechte ist.

### `Ist zwischen` (Fortgeschritten) {#block_operator_is_in_between}

<img src={useBaseUrl('/img/blocks/block_operator_is_in_between.svg')} alt="block_operator_is_in_between.svg" />

Gibt `true` zurück, wenn ein Wert innerhalb der angegebenen Grenzen liegt.

## Boolesche Logikoperatoren

### `Und` (Fortgeschritten) {#block_operator_and}

<img src={useBaseUrl('/img/blocks/block_operator_and.svg')} alt="block_operator_and.svg" />

Gibt nur dann `true` zurück, wenn beide Bedingungen `true` sind.

### `Oder` (Fortgeschritten) {#block_operator_or}

<img src={useBaseUrl('/img/blocks/block_operator_or.svg')} alt="block_operator_or.svg" />

Gibt `true` zurück, wenn mindestens eine Bedingung `true` ist.

### `Nicht` (Fortgeschritten) {#block_operator_not}

<img src={useBaseUrl('/img/blocks/block_operator_not.svg')} alt="block_operator_not.svg" />

Invertiert einen booleschen Wert.

## Textoperatoren

### `Verbinden` (Fortgeschritten) {#block_operator_join}

<img src={useBaseUrl('/img/blocks/block_operator_join.svg')} alt="block_operator_join.svg" />

Verknüpft zwei Textwerte.

### `Buchstabe an Position` (Guru) {#block_operator_letter_at}

<img src={useBaseUrl('/img/blocks/block_operator_letter_at.svg')} alt="block_operator_letter_at.svg" />

Gibt das Zeichen an einer gewählten Position im Text zurück.

### `Länge von Text` (Fortgeschritten) {#block_operator_size_of_string}

<img src={useBaseUrl('/img/blocks/block_operator_size_of_string.svg')} alt="block_operator_size_of_string.svg" />

Gibt die Textlänge zurück.

### `Text enthält` (Guru) {#block_operator_string_contains}

<img src={useBaseUrl('/img/blocks/block_operator_string_contains.svg')} alt="block_operator_string_contains.svg" />

Gibt `true` zurück, wenn der Text die angegebene Teilzeichenfolge enthält.