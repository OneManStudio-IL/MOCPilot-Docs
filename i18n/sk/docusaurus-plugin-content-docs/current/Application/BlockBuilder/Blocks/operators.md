---
id: Operators
title: Operátory
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Operátory

Operátory sú bloky typu Reporter a Boolean, ktoré sa používajú na výpočty, porovnávanie, logiku a prácu s textom.

## Aritmetické operátory

### `Sčítanie` (Začiatočník) {#block_operator_plus}

<img src={useBaseUrl('/img/blocks/block_operator_plus.svg')} alt="block_operator_plus.svg" />

Vracia súčet dvoch hodnôt.

### `Odčítanie` (Začiatočník) {#block_operator_minus}

<img src={useBaseUrl('/img/blocks/block_operator_minus.svg')} alt="block_operator_minus.svg" />

Vracia výsledok odčítania dvoch hodnôt.

### `Násobenie` (Začiatočník) {#block_operator_multiply}

<img src={useBaseUrl('/img/blocks/block_operator_multiply.svg')} alt="block_operator_multiply.svg" />

Vracia súčin dvoch hodnôt.

### `Delenie` (Začiatočník) {#block_operator_divide}

<img src={useBaseUrl('/img/blocks/block_operator_divide.svg')} alt="block_operator_divide.svg" />

Vracia výsledok delenia dvoch hodnôt.

### `Zvyšok po delení` (Guru) {#block_operator_modulus}

<img src={useBaseUrl('/img/blocks/block_operator_modulus.svg')} alt="block_operator_modulus.svg" />

Vracia zvyšok po delení.

### `Zaokrúhliť` (Guru) {#block_operator_round}

<img src={useBaseUrl('/img/blocks/block_operator_round.svg')} alt="block_operator_round.svg" />

Zaokrúhli na najbližšie celé číslo (napr. `2.6 -> 3`).

### `Matematická funkcia (jedna hodnota)` (Guru) {#block_operator_math_single}

<img src={useBaseUrl('/img/blocks/block_operator_math_single.svg')} alt="block_operator_math_single.svg" />

Použije matematickú funkciu na jednu hodnotu.

Dostupné funkcie:

- `absolútna hodnota`: absolútna hodnota čísla  
- `celé menšie`: zaokrúhlenie nadol na najbližšie celé číslo  
- `celé väčšie`: zaokrúhlenie nahor na najbližšie celé číslo  
- `druhá odmocnina`: druhá odmocnina  
- `sin`: sínus (podľa uhla)  
- `cos`: kosínus (podľa uhla)  
- `tan`: tangens (podľa uhla)  
- `asin`: arkus sínus  
- `acos`: arkus kosínus  
- `atan`: arkus tangens  
- `ln`: prirodzený logaritmus (základ `e`)  
- `log`: logaritmus so základom `10`  
- `e^`: číslo `e` umocnené na vstupnú hodnotu  
- `10^`: číslo `10` umocnené na vstupnú hodnotu  

### `Matematická funkcia (dve hodnoty)` (Guru) {#block_operator_math_pair}

<img src={useBaseUrl('/img/blocks/block_operator_math_pair.svg')} alt="block_operator_math_pair.svg" />

Použije matematickú funkciu na dve hodnoty.

Dostupné funkcie:

- `min`: menšia z dvoch hodnôt  
- `max`: väčšia z dvoch hodnôt  
- `mocnina`: prvá hodnota umocnená na druhú  
- `atan2`: uhol zo súradníc X/Y  
- `hypot`: dĺžka prepony zo súradníc  
- `copysign`: prvá hodnota so znamienkom druhej  

### `Náhodné číslo` (Guru) {#block_operator_pick_random}

<img src={useBaseUrl('/img/blocks/block_operator_pick_random.svg')} alt="block_operator_pick_random.svg" />

Vracia náhodné číslo v zadanom intervale.

## Porovnávacie operátory

### `Rovná sa` (Začiatočník) {#block_operator_equal}

<img src={useBaseUrl('/img/blocks/block_operator_equal.svg')} alt="block_operator_equal.svg" />

Vracia `true`, keď sú dve hodnoty rovnaké.

### `Nerovná sa` (Pokročilý) {#block_operator_not_equal}

<img src={useBaseUrl('/img/blocks/block_operator_not_equal.svg')} alt="block_operator_not_equal.svg" />

Vracia `true`, keď sa hodnoty líšia.

### `Väčšie ako` (Začiatočník) {#block_operator_greater_than}

<img src={useBaseUrl('/img/blocks/block_operator_greater_than.svg')} alt="block_operator_greater_than.svg" />

Vracia `true`, keď je ľavá hodnota väčšia ako pravá.

### `Menšie ako` (Začiatočník) {#block_operator_less_than}

<img src={useBaseUrl('/img/blocks/block_operator_less_than.svg')} alt="block_operator_less_than.svg" />

Vracia `true`, keď je ľavá hodnota menšia ako pravá.

### `Je medzi` (Pokročilý) {#block_operator_is_in_between}

<img src={useBaseUrl('/img/blocks/block_operator_is_in_between.svg')} alt="block_operator_is_in_between.svg" />

Vracia `true`, keď sa hodnota nachádza medzi zadanými hranicami.

## Logické operátory

### `A zároveň` (Pokročilý) {#block_operator_and}

<img src={useBaseUrl('/img/blocks/block_operator_and.svg')} alt="block_operator_and.svg" />

Vracia `true`, iba keď sú obe podmienky pravdivé.

### `Alebo` (Pokročilý) {#block_operator_or}

<img src={useBaseUrl('/img/blocks/block_operator_or.svg')} alt="block_operator_or.svg" />

Vracia `true`, keď je aspoň jedna podmienka pravdivá.

### `Nie` (Pokročilý) {#block_operator_not}

<img src={useBaseUrl('/img/blocks/block_operator_not.svg')} alt="block_operator_not.svg" />

Neguje (obracia) boolean hodnotu.

## Textové operátory

### `Spojiť` (Pokročilý) {#block_operator_join}

<img src={useBaseUrl('/img/blocks/block_operator_join.svg')} alt="block_operator_join.svg" />

Spojí dva textové reťazce.

### `Znak na pozícii` (Guru) {#block_operator_letter_at}

<img src={useBaseUrl('/img/blocks/block_operator_letter_at.svg')} alt="block_operator_letter_at.svg" />

Vracia znak na vybranej pozícii v texte.

### `Dĺžka textu` (Pokročilý) {#block_operator_size_of_string}

<img src={useBaseUrl('/img/blocks/block_operator_size_of_string.svg')} alt="block_operator_size_of_string.svg" />

Vracia dĺžku textového reťazca.

### `Text obsahuje` (Guru) {#block_operator_string_contains}

<img src={useBaseUrl('/img/blocks/block_operator_string_contains.svg')} alt="block_operator_string_contains.svg" />

Vracia `true`, ak text obsahuje zadaný podreťazec.
