---
id: Operators
title: Operátory
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Operátory

Operátory jsou reportovací a booleovské bloky používané pro výpočty, porovnání, logiku a práci s textem.

## Aritmetické operátory

### `Sčítání` (Začátečník) {#block_operator_plus}
<img src={useBaseUrl('/img/blocks/block_operator_plus.svg')} alt="block_operator_plus.svg" />
Vrací součet dvou hodnot.

### `Odčítání` (Začátečník) {#block_operator_minus}
<img src={useBaseUrl('/img/blocks/block_operator_minus.svg')} alt="block_operator_minus.svg" />
Vrací výsledek odčítání dvou hodnot.

### `Násobení` (Začátečník) {#block_operator_multiply}
<img src={useBaseUrl('/img/blocks/block_operator_multiply.svg')} alt="block_operator_multiply.svg" />
Vrací součin dvou hodnot.

### `Dělení` (Začátečník) {#block_operator_divide}
<img src={useBaseUrl('/img/blocks/block_operator_divide.svg')} alt="block_operator_divide.svg" />
Vrací výsledek dělení dvou hodnot.

### `Modulo` (Guru) {#block_operator_modulus}
<img src={useBaseUrl('/img/blocks/block_operator_modulus.svg')} alt="block_operator_modulus.svg" />
Vrací zbytek po dělení.

### `Zaokrouhlit` (Guru) {#block_operator_round}
<img src={useBaseUrl('/img/blocks/block_operator_round.svg')} alt="block_operator_round.svg" />
Zaokrouhlí na nejbližší celé číslo (např. `2.6 -> 3`).

### `Math single` (Guru) {#block_operator_math_single}
<img src={useBaseUrl('/img/blocks/block_operator_math_single.svg')} alt="block_operator_math_single.svg" />
Použije matematickou funkci s jedním argumentem.

Dostupné funkce:

- `absolutní hodnota`: absolutní hodnota čísla
- `celé menší`: zaokrouhlení dolů na nejbližší celé číslo
- `celé větší`: zaokrouhlení nahoru na nejbližší celé číslo
- `odmocnina`: druhá odmocnina
- `sin`: sinus (podle úhlu)
- `cos`: kosinus (podle úhlu)
- `tan`: tangens (podle úhlu)
- `asin`: arkus sinus
- `acos`: arkus kosinus
- `atan`: arkus tangens
- `ln`: přirozený logaritmus (základ `e`)
- `log`: logaritmus o základu `10`
- `e^`: umocní `e` na hodnotu vstupu
- `10^`: umocní `10` na hodnotu vstupu

### `Math pair` (Guru) {#block_operator_math_pair}
<img src={useBaseUrl('/img/blocks/block_operator_math_pair.svg')} alt="block_operator_math_pair.svg" />
Použije matematickou funkci se dvěma argumenty.

Dostupné funkce:

- `min`: menší ze dvou hodnot
- `max`: větší ze dvou hodnot
- `mocnina`: první hodnota umocněná na druhou
- `atan2`: úhel z dvojice X/Y
- `hypot`: délka přepony ze dvou složek
- `copysign`: první hodnota se znaménkem druhé hodnoty

### `Náhodné číslo` (Guru) {#block_operator_pick_random}
<img src={useBaseUrl('/img/blocks/block_operator_pick_random.svg')} alt="block_operator_pick_random.svg" />
Vrací náhodné číslo ve zvoleném rozsahu.

## Porovnávací operátory

### `Rovná se` (Začátečník) {#block_operator_equal}
<img src={useBaseUrl('/img/blocks/block_operator_equal.svg')} alt="block_operator_equal.svg" />
Vrací `true`, když jsou dvě hodnoty stejné.

### `Nerovná se` (Pokročilý) {#block_operator_not_equal}
<img src={useBaseUrl('/img/blocks/block_operator_not_equal.svg')} alt="block_operator_not_equal.svg" />
Vrací `true`, když dvě hodnoty nejsou stejné.

### `Větší než` (Začátečník) {#block_operator_greater_than}
<img src={useBaseUrl('/img/blocks/block_operator_greater_than.svg')} alt="block_operator_greater_than.svg" />
Vrací `true`, když je levá hodnota větší než pravá.

### `Menší než` (Začátečník) {#block_operator_less_than}
<img src={useBaseUrl('/img/blocks/block_operator_less_than.svg')} alt="block_operator_less_than.svg" />
Vrací `true`, když je levá hodnota menší než pravá.

### `Je mezi` (Pokročilý) {#block_operator_is_in_between}
<img src={useBaseUrl('/img/blocks/block_operator_is_in_between.svg')} alt="block_operator_is_in_between.svg" />
Vrací `true`, když je hodnota uvnitř zadaných mezí.

## Booleovská logika

### `A` (Pokročilý) {#block_operator_and}
<img src={useBaseUrl('/img/blocks/block_operator_and.svg')} alt="block_operator_and.svg" />
Vrací `true` pouze tehdy, když jsou obě podmínky `true`.

### `Nebo` (Pokročilý) {#block_operator_or}
<img src={useBaseUrl('/img/blocks/block_operator_or.svg')} alt="block_operator_or.svg" />
Vrací `true`, když je alespoň jedna podmínka `true`.

### `Ne` (Pokročilý) {#block_operator_not}
<img src={useBaseUrl('/img/blocks/block_operator_not.svg')} alt="block_operator_not.svg" />
Neguje booleovskou hodnotu.

## Textové operátory

### `Spojit` (Pokročilý) {#block_operator_join}
<img src={useBaseUrl('/img/blocks/block_operator_join.svg')} alt="block_operator_join.svg" />
Spojí dvě textové hodnoty.

### `Písmeno na pozici` (Guru) {#block_operator_letter_at}
<img src={useBaseUrl('/img/blocks/block_operator_letter_at.svg')} alt="block_operator_letter_at.svg" />
Vrátí znak na vybrané pozici v textu.

### `Délka řetězce` (Pokročilý) {#block_operator_size_of_string}
<img src={useBaseUrl('/img/blocks/block_operator_size_of_string.svg')} alt="block_operator_size_of_string.svg" />
Vrací délku řetězce.

### `Řetězec obsahuje` (Guru) {#block_operator_string_contains}
<img src={useBaseUrl('/img/blocks/block_operator_string_contains.svg')} alt="block_operator_string_contains.svg" />
Vrací `true`, pokud text obsahuje zadaný podřetězec.