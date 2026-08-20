# Atelier Seaborn — Analyse exploratoire de données IoT

## Contexte
Analyse exploratoire de mesures de capteurs IoT (température, humidité, pression, 
consommation énergétique) répartis dans plusieurs bâtiments, à l'aide de NumPy, 
Pandas, Matplotlib et Seaborn.

## Structure du projet

    atelier_seaborn_iot/
    │
    ├── data/
    │   └── mesures_capteurs.csv
    │
    ├── notebooks/
    │   └── atelier_seaborn_iot.ipynb
    │
    └── exports/

## Dataset
- id_mesure : identifiant de la mesure
- date_heure : date et heure de la mesure
- id_capteur : identifiant du capteur
- batiment : bâtiment concerné (B001 à B004)
- temperature, humidite, pression, consommation : valeurs mesurées
- etat : état du capteur (OK, ALERTE, ERREUR)

605 mesures, 12 capteurs, 4 bâtiments. Quelques valeurs manquantes présentes 
sur plusieurs colonnes.

## Installation
pip install ipykernel (Si on veut utiliser .venv comme kernel dans Jupyter/VS Code, ipykernel est généralement ce qu'il faut installer dans cet environnement.)
pip install pandas numpy matplotlib seaborn

## Utilisation
Ouvrir le dossier atelier_seaborn_iot dans VS Code, puis ouvrir 
notebooks/atelier_seaborn_iot.ipynb (extension Jupyter requise).

## Avancement
- [x] Structure du projet
- [x] Import et vérification du dataset
- [ ] Partie 1 — histplot()
- [ ] Partie 2 — kdeplot()
- [ ] Partie 3 — boxplot()
- [ ] Partie 4 — violinplot()
- [ ] Partie 5 — countplot()
- [ ] Partie 6 — scatterplot()
- [ ] Partie 7 — regplot()
- [ ] Partie 8 — lmplot()
- [ ] Partie 9 — Corrélations
- [ ] Partie 10 — pairplot()
- [ ] Partie 11 — Export des graphiques
- [ ] Partie 12 — Bonus