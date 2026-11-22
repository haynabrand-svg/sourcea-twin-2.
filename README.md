# SOURCEA Twin 2.0

Prototype interactif de dimensionnement préliminaire d'un système de pompage solaire et de traitement de l'eau.

## Statut

Cette version est un prototype de démonstration côté navigateur. Elle ne constitue pas un jumeau numérique connecté à une installation réelle et ses résultats ne sont pas des validations d'ingénierie.

## Utilisation

Ouvrir `index.html` dans un navigateur. Le prototype utilise Tailwind CSS, Lucide et Google Fonts via CDN, donc une connexion Internet est nécessaire pour charger ces ressources.

## Modèle de calcul actuel

- Énergie hydraulique : `Eh = (9.81 × V × HMT) / 3600` (kWh/jour)
- Énergie électrique estimée : `Eelec = Eh / η`
- Puissance PV estimée : `Ppv = (Eelec / PSH) × 1000` (Wp)
- Débit indicatif : `Q = V / PSH` (m³/h)

Ces relations sont simplifiées. Les hypothèses, unités et limites doivent être vérifiées avant tout usage de conception.

## À faire avant toute présentation comme outil d'ingénierie

- Remplacer les statuts et formulations laissant entendre une validation réelle.
- Vérifier les équations, unités et hypothèses avec un ingénieur hydraulique/énergéticien.
- Ajouter les données de terrain, les courbes de pompe, pertes de charge détaillées et contraintes PV.
- Ne jamais déclarer l'eau potable sans conception validée, analyses de laboratoire et conformité réglementaire.

Voir `docs/` pour les notes techniques, limites et prochaines étapes.
