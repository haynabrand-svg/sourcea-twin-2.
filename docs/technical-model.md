# Modèle technique actuel

## Paramètres d'entrée

Le prototype expose quatre paramètres réglables :

- Volume quotidien cible `V` (m³/jour), initialement 10.
- Hauteur manométrique totale `HMT` (m), initialement 15.
- Heures de soleil de pointe `PSH` (h/jour), initialement 7,5.
- Rendement global `η`, initialement 40 %.

## Calculs implémentés

Le JavaScript calcule :

```text
Eh    = (9.81 × V × HMT) / 3600
Eelec = Eh / η
Ppv   = (Eelec / PSH) × 1000
Qmax  = V / PSH
```

Les valeurs sont présentées comme énergie hydraulique (kWh/j), énergie électrique (kWh/j), puissance PV (Wp) et débit (m³/h).

## Interprétation prudente

Il s'agit d'un estimateur simplifié avec paramètres saisis par l'utilisateur. `Qmax = V / PSH` est un débit moyen théorique sur la durée PSH, pas une courbe de pompe ni une simulation horaire. La puissance PV calculée ne remplace pas un dimensionnement intégrant les conditions locales, les pertes, les limites du contrôleur et la plage de fonctionnement de la pompe.
