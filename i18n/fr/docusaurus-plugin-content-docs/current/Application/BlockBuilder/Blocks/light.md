---
id: Light
title: Lumière
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Lumière

Cette page décrit les blocs de la catégorie Lumière utilisés pour contrôler les LED et les sorties lumineuses sur les hubs compatibles.

## Blocs lumineux communs

### `Définir la couleur de la LED` (Débutant) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

Définit la couleur de la LED du hub en utilisant des options de couleur prédéfinies.

- Type : bloc de commande
- Utilisation typique : indiquer un état (prêt, en cours, avertissement, erreur)

### `Allumer la lumière à` (Débutant) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

Définit la sortie lumineuse sélectionnée à une luminosité/valeur cible.

- Type : bloc de commande
- Utilisation typique : intensité des phares, indication d’état

### `Éteindre la lumière` (Débutant) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

Éteint la sortie lumineuse sélectionnée.

- Type : bloc de commande
- Utilisation typique : séquence d’arrêt, économie de batterie

### `Technic Move allumer la lumière à` (Débutant) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Variante de `Allumer la lumière à` pour le hub Technic Move.

- Type : bloc de commande
- Utilisation typique : définir le niveau de sortie lumineuse du hub Move

## Blocs de matrice LED interne

### `Allumer la matrice lumineuse` (Avancé) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

Affiche l’image sélectionnée sur la matrice LED interne du hub et passe immédiatement au bloc suivant de la pile. L’image reste affichée jusqu’à ce qu’un autre bloc modifie la matrice LED interne ou que le programme s’arrête.

- Type : bloc de commande
- Remarque : le hub sélectionné doit posséder une matrice LED interne.

### `Écrire sur la matrice lumineuse` (Débutant) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

Affiche une chaîne de texte sur la matrice LED interne du hub en faisant défiler une lettre à la fois.

- Type : bloc de commande
- Remarque : le hub sélectionné doit posséder une matrice LED interne.

### `Éteindre les pixels de la matrice` (Débutant) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

Éteint toutes les lumières de la matrice LED interne du hub.

- Type : bloc de commande
- Remarque : le hub sélectionné doit posséder une matrice LED interne.

### `Définir un pixel de la matrice` (Avancé) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

Définit la luminosité d’un pixel sur la matrice LED interne du hub. Seul le pixel sélectionné est mis à jour ; le reste de l’affichage reste inchangé. Les champs de position du pixel utilisent les valeurs de colonne et de ligne, avec le pixel `1, 1` dans le coin supérieur gauche.

- Type : bloc de commande
- Remarque : le hub sélectionné doit posséder une matrice LED interne.

### `Faire pivoter l’orientation de la matrice` (Avancé) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

Fait pivoter l’orientation de ce qui est affiché sur la matrice LED interne du hub, dans le sens horaire ou antihoraire. Chaque rotation modifie l’orientation de l’affichage de 90 degrés et affecte les blocs Lumière exécutés ensuite.

- Type : bloc de commande
- Remarque : le hub sélectionné doit posséder une matrice LED interne.

### `Définir l’orientation de la matrice` (Avancé) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

Définit l’orientation de ce qui est affiché sur la matrice LED interne du hub. L’orientation par défaut est verticale, et l’orientation sélectionnée affecte les blocs Lumière exécutés ensuite.

- Type : bloc de commande
- Options d’orientation : `verticale`, `gauche`, `droite`, `à l’envers`
- Remarque : le hub sélectionné doit posséder une matrice LED interne.

## Blocs lumineux du capteur de distance

### `Allumer le capteur de distance` (Débutant) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

Définit les lumières du capteur de distance sélectionné. Le bloc peut allumer ou éteindre les lumières individuelles du capteur et peut utiliser un bloc rapporteur de liste pour contrôler la luminosité de chaque lumière.

- Type : bloc de commande
- Remarque : disponible uniquement pour le hub MINDSTORMS Robot Inventor.

## Blocs lumineux BuWizz 3

### `BuWizz 3 définir la couleur de la LED` (Débutant) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

Définit la couleur de la LED sur le port BuWizz 3 sélectionné avec des options intégrées.

- Type : bloc de commande

### `BuWizz 3 définir la couleur de la LED (texte)` (Guru) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

Définit la couleur de la LED BuWizz 3 à partir d’une valeur texte.

- Type : bloc de commande
- Utilisation typique : couleurs dynamiques provenant de variables

### `BuWizz 3 définir la couleur de la LED (RGB)` (Avancé) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

Définit la couleur de la LED BuWizz 3 à l’aide des canaux RGB.

- Type : bloc de commande
- Utilisation typique : contrôle complet des couleurs et dégradés
