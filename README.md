# Atelier Matplotlib — Capteurs IoT

## Description

Cet atelier prolonge le travail effectué avec NumPy et Pandas sur le jeu de données de capteurs IoT. L'objectif est de visualiser ces données afin de faire apparaître des tendances, des différences entre bâtiments et des anomalies qu'un simple tableau de chiffres ne permet pas de repérer facilement.

Le notebook couvre huit types de graphiques classiques (courbe, diagramme en barres, histogramme, nuage de points, boîte à moustaches, diagramme circulaire, superposition de courbes, sauvegarde de graphiques), complétés par une partie bonus proposant un tableau de bord synthétique.

## Jeu de données

Le fichier `mesures_capteurs.csv` contient, pour chaque mesure : un identifiant, une date/heure, un identifiant de capteur, un bâtiment (B001 à B004), la température (°C), l'humidité (%), la pression (hPa), la consommation énergétique (kWh) et l'état du capteur (OK, ALERTE, ERREUR). Le jeu de données contient volontairement quelques valeurs manquantes et quelques valeurs aberrantes, utilisées pour illustrer comment les graphiques aident à les repérer visuellement.

## Structure du projet

```
atelier_matplotlib_iot/
│
├── data/
│   └── mesures_capteurs.csv
│
├── notebooks/
│   └── atelier_matplotlib_iot.ipynb
│
└── exports/
    ├── temperature.png
    ├── temperature.pdf
    └── dashboard.png
```

Le fichier `mesures_capteurs.csv` est placé dans `data/`, le notebook dans `notebooks/`, et les graphiques exportés au fil de l'atelier sont enregistrés dans `exports/`.

## Contenu du notebook

1. **Courbe** — évolution temporelle de la température, repérage de valeurs aberrantes.
2. **Diagramme en barres** — consommation moyenne par bâtiment, avec une variante horizontale.
3. **Histogramme** — distribution des températures et de la consommation.
4. **Nuage de points** — relation entre température et consommation.
5. **Boîte à moustaches** — médiane, dispersion et valeurs extrêmes.
6. **Diagramme circulaire** — proportion de capteurs OK, ALERTE et ERREUR.
7. **Superposition de courbes** — comparaison des quatre bâtiments.
8. **Sauvegarde de graphiques** — export au format PNG (matriciel) et PDF (vectoriel).
9. **Partie bonus** — tableau de bord synthétique réunissant quatre graphiques clés en une seule figure, avec mise en évidence des mesures ALERTE/ERREUR.

## Prérequis

- Python 3
- pandas
- numpy
- matplotlib

## Utilisation

1. Placer `mesures_capteurs.csv` dans le dossier `data/`.
2. Ouvrir `notebooks/atelier_matplotlib_iot.ipynb`.
3. Exécuter les cellules dans l'ordre.

Les graphiques générés sont automatiquement enregistrés dans le dossier `exports/`.

## Conclusion

L'atelier a permis de couvrir les principaux types de graphiques utilisés en analyse de données, appliqués au jeu de données de capteurs IoT déjà exploré avec Pandas. Les graphiques confirment et enrichissent les constats faits précédemment (valeurs manquantes, valeurs aberrantes, différences entre bâtiments), tout en les rendant beaucoup plus immédiats à interpréter qu'une lecture de tableaux de chiffres.

## Auteur

Abdoulaye DIOUF
Projet réalisé dans le cadre d'un atelier de pratique Matplotlib.