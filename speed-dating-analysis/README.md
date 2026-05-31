# 💘 Speed Dating — Exploratory Data Analysis

**Certification :** Data Science Full Stack — Bac+4  
**Bloc :** Exploratory Data Analysis  
**Dataset :** Columbia Business School speed-dating experiments (2002–2004)

---

## 🎯 Objectif

Analyser les facteurs qui influencent la décision de se revoir après un speed date (`match = 1`).  
Le dataset couvre 8 378 observations et 195 variables : notes attribuées sur 6 attributs, données démographiques, habitudes de rencontre et auto-perception des participants.

---

## 📁 Structure du projet

```
speed-dating-analysis/
├── data/
│   └── raw/
│       └── speed_dating.csv        # Dataset source (non versionné)
├── notebooks/
│   └── 01_speed_dating_eda.ipynb   # Notebook principal
├── outputs/
│   └── figures/                    # Graphiques exportés (HTML / PNG)
├── src/
│   └── __init__.py
├── environment.yml
├── .gitignore
└── README.md
```

---

## 🔍 Analyses réalisées

| # | Question | Section |
|---|----------|---------|
| 1 | Aperçu général & valeurs manquantes | Section 2 |
| 2 | Statistiques descriptives & taux de match par genre | Section 3 |
| 3 | Quels attributs sont les moins désirables ? (H vs F) | Section 4 |
| 4 | L'attractivité : importance déclarée vs impact réel | Section 5 |
| 5 | Intérêts communs vs origine ethnique partagée | Section 6 |
| 6 | Les gens peuvent-ils prédire leur valeur perçue ? | Section 7 |
| 7 | Vaut-il mieux être le premier ou le dernier date ? | Section 8 |

---

## 🛠 Stack technique

| Outil | Usage |
|-------|-------|
| Python 3.11 | Langage principal |
| Pandas | Manipulation des données |
| NumPy | Calculs numériques |
| Plotly | Visualisations interactives |
| Statsmodels | Régressions OLS (trendlines Plotly) |
| Jupyter / VS Code | Environnement de développement |

---

## ⚙️ Installation

```bash
# 1. Cloner le repo
git clone [https://github.com/Ibra-Ba/speed-dating]
cd speed-dating-analysis

# 2. Créer et activer l'environnement conda
conda env create -f environment.yml
conda activate speed-dating

# 3. Enregistrer le kernel Jupyter
python -m ipykernel install --user --name speed-dating --display-name "Python (speed-dating)"

# 4. Placer le dataset
cp /path/to/speed_dating.csv data/raw/

# 5. Ouvrir le notebook
code .
```

---

## 📊 Principaux résultats

- **L'attractivité** est le prédicteur n°1 du match pour les deux genres, particulièrement chez les hommes.
- **L'ambition** est l'attribut le moins corrélé avec le match — pour les deux genres.
- Les participants **sous-estiment l'importance de l'attractivité** dans leurs déclarations (biais de désirabilité sociale).
- Les **intérêts partagés** prédisent mieux le match que l'origine ethnique commune.
- La **connaissance de soi** est modérée : corrélation positive mais faible entre auto-évaluation et score reçu, avec une tendance à se surestimer.
- Être le **premier date de la soirée** confère un léger avantage (fatigue décisionnelle en fin de soirée).

---

## 📬 Livrables

- `notebooks/01_speed_dating_eda.ipynb` — Notebook complet avec statistiques descriptives, visualisations et interprétations
- `outputs/figures/` — Graphiques exportés en HTML interactif

---

## 👤 Ibrahim BAH

Projet réalisé dans le cadre de la certification **Jedha Bootcamp — Bac+4 Data Science Full Stack**.