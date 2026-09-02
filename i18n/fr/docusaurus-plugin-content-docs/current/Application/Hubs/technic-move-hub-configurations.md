---
id: TechnicMoveHubConfigurations
title: Configurations du Technic Move Hub
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Configurations du Technic Move Hub

## Présentation

Technic Move Hub a introduit une fonction unique dans la famille des hubs LEGO Powered Up : le hub peut changer de comportement selon la configuration actuellement appliquée.

MOCPilot permet de modifier la configuration du Technic Move Hub afin que son comportement corresponde au set LEGO officiel que vous souhaitez contrôler.

## Configurations prises en charge

Pour le moment, les configurations Technic Move Hub connues sont :

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Options de configuration du Technic Move Hub dans le bloc Définir la configuration du hub" />

## Changer la configuration depuis Mes hubs Bluetooth

Vous pouvez changer la configuration depuis la page **Mes hubs Bluetooth** :

1. Ouvrez **Mes hubs Bluetooth**.
2. Trouvez le Technic Move Hub.
3. Ouvrez le menu contextuel du hub.
4. Sélectionnez **Sélectionner la configuration**.
5. Choisissez la configuration requise.
6. Confirmez la boîte de dialogue de reconfiguration.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Menu contextuel du Technic Move Hub avec l’action Sélectionner la configuration" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Sous-menu de configuration du Technic Move Hub" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Boîte de dialogue de confirmation de reconfiguration du Technic Move Hub" />

:::warning Important
Changer la configuration du hub flashe un sous-programme dans le hub et ressemble à une mise à jour du firmware.

Gardez le hub allumé pendant toute la procédure. Gardez le téléphone, la tablette ou l’ordinateur alimenté et proche du hub afin que la connexion Bluetooth reste stable. Ne fermez pas MOCPilot, ne désactivez pas Bluetooth et n’éteignez pas le hub pendant le changement de configuration.

Interrompre le changement de configuration peut endommager le firmware du hub. Dans ce cas, une récupération du firmware peut être nécessaire avant de l’utiliser à nouveau. Suivez le guide de [récupération du firmware du hub](/docs/Application/Hubs/RecoveryHubFirmware/) si une récupération est requise.
:::

Pendant la reconfiguration, le hub ne répond pas aux commandes normales. Sa LED clignote avec une indication colorée par étapes jusqu’à la fin du processus. Une fois la nouvelle configuration appliquée, le hub est réinitialisé.

## Blocs de configuration

MOCPilot inclut aussi des blocs pour lire et changer la configuration du Technic Move Hub pendant un programme.

### Définir la configuration du hub

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="Bloc Définir la configuration du hub" />

Le bloc **Définir la configuration du hub** change le hub sélectionné vers l’un de ses profils de configuration pris en charge.

- Sélecteur de hub : choisit le hub à reconfigurer.
- Sélecteur de configuration : choisit la configuration cible.
- Configurations disponibles pour Technic Move Hub : **Porsche GT4 e-Performance**, **Lamborghini Revuelto** et **Batmobile™ Tumbler**.

Consultez la [documentation du bloc Définir la configuration du hub](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config).

### Configuration du hub

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="Bloc rapporteur Configuration du hub" />

Le bloc **Configuration du hub** indique la configuration actuelle du hub sélectionné.

- Sélecteur de hub : choisit le hub à lire.
- Format de sortie : **texte** renvoie le nom de la configuration.
- Format de sortie : **indice** renvoie l’indice de la configuration, utile pour les comparaisons dans les conditions.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="Options de format de sortie du bloc Configuration du hub" />

Consultez la [documentation du bloc Configuration du hub](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config).

### Impulsion de puissance

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="Bloc Impulsion de puissance du Technic Move Hub" />

Le bloc **Impulsion de puissance** envoie une commande d’impulsion de puissance au Technic Move Hub sélectionné. Ce bloc fonctionne uniquement lorsque le Technic Move Hub est configuré en **Batmobile™ Tumbler**.

Lorsqu’il s’exécute, le hub démarre les moteurs avec la puissance et la vitesse maximales disponibles pendant une courte durée, généralement 1 à 2 secondes.

Consultez la [documentation du bloc Impulsion de puissance](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse).

## Changer la configuration pendant l’exécution du programme

Il est aussi possible de changer la configuration du Technic Move Hub pendant qu’un programme s’exécute.

L’approche habituelle est :

1. Lire la configuration actuelle du hub.
2. La comparer avec la configuration requise par le profil.
3. Si la configuration est différente, appliquer la configuration requise.
4. Relire la configuration après la reconfiguration.
5. Continuer uniquement lorsque le hub indique la configuration attendue.
6. Déconnecter ou arrêter le programme si la configuration requise n’a pas été appliquée.

Le profil prédéfini qui utilise ce hub peut servir de référence pour cette approche.

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="Exemple de blocs montrant le changement de configuration du Technic Move Hub pendant l’exécution" />
