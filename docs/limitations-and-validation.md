# Limites et validation requise

## État du prototype

La version actuelle est une interface HTML/JavaScript autonome. Elle ne reçoit aucune télémétrie IoT, ne lit aucun capteur, ne stocke pas de mesures de terrain et ne se synchronise pas avec une installation.

## Limites de calcul

- Le rendement global est une seule hypothèse d'entrée ; les rendements des panneaux, du contrôleur, du moteur et de la pompe ne sont pas modélisés séparément.
- Les pertes de charge, niveaux statique et dynamique, caractéristiques de conduite et courbe de pompe ne sont pas calculés.
- La production PV ne tient pas explicitement compte de la température, de l'ombrage, de l'orientation, du câblage ou des limites du contrôleur.
- Les valeurs initiales sont des valeurs de démonstration, pas des mesures de site.
- Le schéma représente des composants conceptuels ; il ne constitue pas un plan d'exécution ni une nomenclature validée.

## Sécurité sanitaire

Les mentions relatives à la turbidité, à l'UV-C, à l'absence d'E. coli et à l'eau potable sont des indications affichées par l'interface, pas des résultats mesurés ni une certification. La potabilité exige une conception adaptée, des analyses en laboratoire et le respect des exigences réglementaires applicables.

## Validation avant usage réel

Collecter les données du site et les fiches techniques des équipements ; faire vérifier les calculs et le dimensionnement par des professionnels qualifiés ; comparer les estimations aux mesures de fonctionnement ; documenter les essais et les résultats de qualité de l'eau. Toute affirmation de conformité ou de performance doit être étayée.
