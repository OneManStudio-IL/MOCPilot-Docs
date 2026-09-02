---
id: AboutApp
title: À propos de MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Construisez. Pilotez. Contrôlez tout.

**MOCPilot** — une application pour créer des profils de contrôle personnalisés pour LEGO® et les créations Bluetooth compatibles.

Elle offre aux constructeurs un seul endroit pour connecter les hubs, contrôler les moteurs, lire les capteurs, concevoir des tableaux de bord et créer des programmes visuels pour modèles, mécanismes, voitures, camions, trains, robots et MOC personnalisés.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="Application MOCPilot sur un téléphone" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>Ce que MOCPilot vous apporte</h2>
    <ul>
      <li>Profils personnalisés pour vos propres modèles.</li>
      <li>Profils prêts à l’emploi pour les sets officiels pris en charge.</li>
      <li>Connexion et gestion des hubs Bluetooth.</li>
      <li>Programmation visuelle par blocs pour l’automatisation et la logique.</li>
      <li>Commandes de tableau de bord pour piloter et utiliser les modèles.</li>
      <li>Prise en charge de LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, des moteurs, capteurs et appareils Bluetooth compatibles.</li>
    </ul>
  </div>
</div>

## L’idée

La plupart des constructions motorisées ont besoin de plus qu’une simple télécommande. Une voiture peut nécessiter direction, accélérateur, lumières, surveillance de batterie, séquence de boîte de vitesses ou routine de démarrage spéciale. Un robot peut nécessiter capteurs, événements, logique conditionnelle et plusieurs hubs travaillant ensemble.

MOCPilot est conçu pour l’espace entre une télécommande basique et un environnement de programmation complet. Vous pouvez commencer par piloter un modèle depuis un tableau de bord à l’écran, puis ajouter logique, capteurs et automatisation quand la construction devient plus avancée.

## Profils

Un **profil** est le centre de contrôle d’un modèle.

Dans un profil, vous choisissez les hubs du modèle, créez le programme qui le fait fonctionner et concevez le tableau de bord utilisé pour le contrôler.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="Page des profils MOCPilot" width="420" />

<details>
<summary>Profils prédéfinis</summary>

Les profils prédéfinis sont des exemples prêts à l’emploi pour les sets officiels pris en charge. Ils sont utiles pour démarrer vite ou comprendre comment un profil fonctionnel est construit.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="Profils prédéfinis MOCPilot" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Programme de blocs prédéfini MOCPilot" width="1100" />

</details>

<details>
<summary>Profils personnalisés</summary>

Les profils personnalisés servent à vos MOC et expérimentations. Vous pouvez créer un profil, ajouter des hubs, connecter moteurs et capteurs, construire un programme et concevoir un tableau de bord adapté au modèle exact.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Créer un profil personnalisé MOCPilot" width="420" />

</details>

## Connecter les hubs et appareils

MOCPilot peut se connecter aux hubs Bluetooth pris en charge et aux appareils compatibles, puis les rendre disponibles dans votre profil.

Vous pouvez utiliser un profil avec un seul hub pour une construction simple, ou connecter plusieurs hubs quand le modèle nécessite plus de ports, des alimentations séparées ou des modules indépendants.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="Page Mes hubs Bluetooth dans MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Hubs Bluetooth connectés dans MOCPilot" width="1100" />

<details>
<summary>Exemples de matériel pris en charge</summary>

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

Consultez la page des [hubs, moteurs et capteurs pris en charge](/docs/Introducing/SupportedDevices/) pour la liste complète.

</details>

## Construire la logique avec des blocs

MOCPilot inclut un constructeur visuel de blocs. Vous pouvez créer des programmes en connectant des blocs au lieu d’écrire du code.

Les blocs peuvent réagir aux événements, contrôler les moteurs, lire les capteurs, utiliser des variables, exploiter l’entrée d’une manette, mettre à jour les contrôleurs du tableau de bord et coordonner plusieurs actions.

MOCPilot prend entièrement en charge les manettes physiques connectées. Les blocs de manette lisent boutons, gâchettes, directions du D-pad et sticks, afin d’associer une vraie manette au modèle lorsque le contrôle physique est préférable à l’écran tactile.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="Programme utilisateur MOCPilot construit avec des blocs" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="Bloc au démarrage du programme" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Bloc démarrer le moteur à une vitesse" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Bloc niveau de batterie du hub" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Bloc valeur du volant" />
</div>

<details>
<summary>Ce que les programmes par blocs permettent de faire</summary>

- Démarrer, arrêter et diriger les moteurs.
- Lire le niveau de batterie, la tension, l’inclinaison, l’orientation, la température et les valeurs des capteurs.
- Configurer une manette physique pour la direction, l’accélération, les gâchettes, les actions et le changement de mode.
- Réagir aux changements de boutons, capteurs, minuteurs ou contrôleurs du tableau de bord.
- Créer des vérifications de démarrage avant que le modèle commence à bouger.
- Ajouter une logique personnalisée pour les lumières, le calibrage de direction, les modes de puissance et la configuration du hub.
- Utiliser variables, listes, conditions, boucles, diffusions et blocs personnalisés pour organiser des comportements complexes.

</details>

## Concevoir un tableau de bord de pilotage

Le tableau de bord est l’écran utilisé pour contrôler le modèle. Il peut contenir volants, joysticks, curseurs, boutons, interrupteurs, pédales, moniteurs et autres contrôleurs.

Vous pouvez connecter les contrôles du tableau de bord et les entrées d’une manette physique aux blocs et aux actions du hub afin que l’interface corresponde au modèle.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="Contrôleurs du tableau de bord MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="Écran de contrôle MOCPilot avec volant et pédales" width="1100" />

<details>
<summary>Exemples de tableaux de bord</summary>

- Utiliser un volant et des pédales pour les voitures.
- Utiliser des curseurs pour grues, élévateurs et actionneurs linéaires.
- Utiliser des boutons pour lumières, klaxon, changements de vitesse ou actions scriptées.
- Utiliser des moniteurs pour afficher batterie, vitesse, valeurs de capteurs ou état personnalisé du programme.
- Utiliser une manette connectée si vous préférez boutons, sticks et gâchettes physiques aux commandes tactiles.

</details>

## Garder les constructions avancées maîtrisables

À mesure qu’un modèle grandit, le profil peut grandir avec lui. MOCPilot prend en charge la logique réutilisable avec **My Blocks**, la configuration des hubs propre au profil, plusieurs contrôleurs et des flux combinant contrôle manuel et automatisation.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="Exemple d’utilisation de My Blocks dans MOCPilot" width="1100" />

Cela aide à garder les grands programmes lisibles. Par exemple, un profil peut avoir un bloc personnalisé pour les mises à jour de batterie, un autre pour le calibrage de direction et un autre pour un mode de conduite spécial.

## Flux de travail typique

1. Créez ou ouvrez un profil.
2. Ajoutez les hubs Bluetooth et appareils utilisés par le modèle.
3. Construisez le programme avec des blocs.
4. Concevez un tableau de bord pour le pilotage et l’interaction.
5. Appuyez sur **Play**.
6. Testez, ajustez et améliorez le profil jusqu’à ce que le modèle se comporte comme souhaité.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Flux de connexion d’un hub dans MOCPilot" width="1100" />

## À qui s’adresse MOCPilot

MOCPilot est utile aux constructeurs qui veulent :

- Une meilleure télécommande pour les modèles LEGO® motorisés.
- Un moyen de contrôler des hubs Bluetooth compatibles tiers.
- Un environnement de programmation visuelle pour mécanismes et robots.
- Des profils prédéfinis pour les sets officiels pris en charge.
- Des tableaux de bord personnalisés pour voitures, camions, trains, crawlers, grues et autres MOC.
- Une seule app combinant hubs, moteurs, capteurs, manettes et contrôles à l’écran.

## Commencer à explorer

- Suivez le [tutoriel de démarrage rapide](/docs/Introducing/QuickStart/) pour créer votre premier profil.
- Consultez les [appareils pris en charge](/docs/Introducing/SupportedDevices/) avant de choisir le matériel.
- Explorez la [documentation BlockBuilder](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/) lorsque vous êtes prêt à ajouter de la logique.
- Consultez la [mise à jour du firmware du hub](/docs/Application/Hubs/FirmwareUpdating/) si un hub nécessite une version de firmware prise en charge.
