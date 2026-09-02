---
id: Operators
title: Opérateurs
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Opérateurs

Les opérateurs sont des blocs de type Reporter et Booléen utilisés pour les calculs, les comparaisons, la logique et le traitement de chaînes de caractères.

## Opérateurs arithmétiques

### `Plus` (Débutant) {#block_operator_plus}

<img src={useBaseUrl('/img/blocks/block_operator_plus.svg')} alt="block_operator_plus.svg" />

Retourne la somme de deux valeurs.

### `Minus` (Débutant) {#block_operator_minus}

<img src={useBaseUrl('/img/blocks/block_operator_minus.svg')} alt="block_operator_minus.svg" />

Retourne le résultat de la soustraction de deux valeurs.

### `Multiply` (Débutant) {#block_operator_multiply}

<img src={useBaseUrl('/img/blocks/block_operator_multiply.svg')} alt="block_operator_multiply.svg" />

Retourne le produit de deux valeurs.

### `Divide` (Débutant) {#block_operator_divide}

<img src={useBaseUrl('/img/blocks/block_operator_divide.svg')} alt="block_operator_divide.svg" />

Retourne le résultat de la division de deux valeurs.

### `Modulus` (Guru) {#block_operator_modulus}

<img src={useBaseUrl('/img/blocks/block_operator_modulus.svg')} alt="block_operator_modulus.svg" />

Retourne le reste après division.

### `Round` (Guru) {#block_operator_round}

<img src={useBaseUrl('/img/blocks/block_operator_round.svg')} alt="block_operator_round.svg" />

Arrondit à l'entier le plus proche (par exemple `2.6 -> 3`).

### `Math single` (Guru) {#block_operator_math_single}

<img src={useBaseUrl('/img/blocks/block_operator_math_single.svg')} alt="block_operator_math_single.svg" />

Applique une fonction mathématique à un seul argument.

Fonctions disponibles :

- `valeur absolue` : valeur absolue d’un nombre
- `entier inférieur` : arrondi à l’entier inférieur
- `entier supérieur` : arrondi à l’entier supérieur
- `racine carrée` : racine carrée
- `sin` : sinus (basé sur un angle)
- `cos` : cosinus (basé sur un angle)
- `tan` : tangente (basée sur un angle)
- `asin` : sinus inverse
- `acos` : cosinus inverse
- `atan` : tangente inverse
- `ln` : logarithme naturel (base `e`)
- `log` : logarithme en base `10`
- `e^` : élève `e` à la puissance donnée
- `10^` : élève `10` à la puissance donnée

### `Math pair` (Guru) {#block_operator_math_pair}

<img src={useBaseUrl('/img/blocks/block_operator_math_pair.svg')} alt="block_operator_math_pair.svg" />

Applique une fonction mathématique à deux arguments.

Fonctions disponibles :

- `min` : plus petite des deux valeurs
- `max` : plus grande des deux valeurs
- `puissance` : première valeur élevée à la puissance de la seconde
- `atan2` : angle à partir d’une paire X/Y
- `hypot` : longueur de l’hypoténuse à partir de deux composantes
- `copysign` : première valeur avec le signe de la seconde

### `Pick random` (Guru) {#block_operator_pick_random}

<img src={useBaseUrl('/img/blocks/block_operator_pick_random.svg')} alt="block_operator_pick_random.svg" />

Retourne un nombre aléatoire dans l’intervalle sélectionné.

## Opérateurs de comparaison

### `Equal` (Débutant) {#block_operator_equal}

<img src={useBaseUrl('/img/blocks/block_operator_equal.svg')} alt="block_operator_equal.svg" />

Retourne `true` lorsque deux valeurs sont égales.

### `Not equal` (Avancé) {#block_operator_not_equal}

<img src={useBaseUrl('/img/blocks/block_operator_not_equal.svg')} alt="block_operator_not_equal.svg" />

Retourne `true` lorsque deux valeurs sont différentes.

### `Greater than` (Débutant) {#block_operator_greater_than}

<img src={useBaseUrl('/img/blocks/block_operator_greater_than.svg')} alt="block_operator_greater_than.svg" />

Retourne `true` lorsque la valeur de gauche est supérieure à celle de droite.

### `Less than` (Débutant) {#block_operator_less_than}

<img src={useBaseUrl('/img/blocks/block_operator_less_than.svg')} alt="block_operator_less_than.svg" />

Retourne `true` lorsque la valeur de gauche est inférieure à celle de droite.

### `Is in between` (Avancé) {#block_operator_is_in_between}

<img src={useBaseUrl('/img/blocks/block_operator_is_in_between.svg')} alt="block_operator_is_in_between.svg" />

Retourne `true` lorsqu’une valeur se situe dans les limites spécifiées.

## Opérateurs logiques (booléens)

### `And` (Avancé) {#block_operator_and}

<img src={useBaseUrl('/img/blocks/block_operator_and.svg')} alt="block_operator_and.svg" />

Retourne `true` uniquement lorsque les deux conditions sont `true`.

### `Or` (Avancé) {#block_operator_or}

<img src={useBaseUrl('/img/blocks/block_operator_or.svg')} alt="block_operator_or.svg" />

Retourne `true` lorsqu’au moins une condition est `true`.

### `Not` (Avancé) {#block_operator_not}

<img src={useBaseUrl('/img/blocks/block_operator_not.svg')} alt="block_operator_not.svg" />

Inverse une valeur booléenne.

## Opérateurs de texte

### `Join` (Avancé) {#block_operator_join}

<img src={useBaseUrl('/img/blocks/block_operator_join.svg')} alt="block_operator_join.svg" />

Concatène deux valeurs de texte.

### `Letter at` (Guru) {#block_operator_letter_at}

<img src={useBaseUrl('/img/blocks/block_operator_letter_at.svg')} alt="block_operator_letter_at.svg" />

Retourne le caractère à une position donnée dans le texte.

### `Size of string` (Avancé) {#block_operator_size_of_string}

<img src={useBaseUrl('/img/blocks/block_operator_size_of_string.svg')} alt="block_operator_size_of_string.svg" />

Retourne la longueur de la chaîne.

### `String contains` (Guru) {#block_operator_string_contains}

<img src={useBaseUrl('/img/blocks/block_operator_string_contains.svg')} alt="block_operator_string_contains.svg" />

Retourne `true` si le texte contient la sous-chaîne spécifiée.
