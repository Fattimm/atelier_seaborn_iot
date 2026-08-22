# Atelier Seaborn — Analyse exploratoire de données IoT

## Contexte
Analyse exploratoire de mesures de capteurs IoT (température, humidité, pression, 
consommation énergétique) répartis dans plusieurs bâtiments, à l'aide de NumPy, 
Pandas, Matplotlib et Seaborn.

## Librairies utilisées
- **Pandas** : import, nettoyage et exploration du dataset (DataFrame, groupby, corr)
- **NumPy** : calculs numériques sous-jacents (utilisé notamment par Pandas et Seaborn)
- **Matplotlib** : affichage et sauvegarde des graphiques (plt.show, plt.savefig)
- **Seaborn** : visualisations statistiques (histplot, boxplot, heatmap, pairplot, etc.)

## Installation
pip install ipykernel (Si on veut utiliser .venv comme kernel dans Jupyter/VS Code, ipykernel est généralement ce qu'il faut installer dans cet environnement.)
pip install pandas numpy matplotlib seaborn

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

## Utilisation
Ouvrir le dossier atelier_seaborn_iot dans VS Code, puis ouvrir 
notebooks/atelier_seaborn_iot.ipynb (extension Jupyter requise).

## Principales conclusions
- Le bâtiment **B004** concentre la majorité des anomalies (ALERTE, ERREUR) et 
  les valeurs de température les plus extrêmes (-18,50 °C à 58,70 °C).
- Les capteurs **C010** et **C011** (tous deux à B004) sont les plus problématiques.
- La seule corrélation notable est **température/consommation (r = 0,32)**, 
  positive mais modérée ; toutes les autres paires de variables sont quasi 
  indépendantes.

## Avancement
- [x] Structure du projet
- [x] Import et vérification du dataset
- [x] Partie 1 — histplot()
- [x] Partie 2 — kdeplot()
- [x] Partie 3 — boxplot()
- [x] Partie 4 — violinplot()
- [x] Partie 5 — countplot()
- [x] Partie 6 — scatterplot()
- [x] Partie 7 — regplot()
- [x] Partie 8 — lmplot()
- [x] Partie 9 — Corrélations
- [x] Partie 10 — pairplot()
- [x] Partie 11 — Export des graphiques
- [x] Partie 12 — Bonus (analyse temporelle, détection capteurs, nettoyage, 
      rapport de synthèse, FacetGrid)