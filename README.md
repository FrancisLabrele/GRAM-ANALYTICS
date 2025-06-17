# Projet GRAM-ANALYTICS
## Présentation du github
Ce projet GitHub regroupe les résultats les plus pertinents que nous avons obtenus après plusieurs phases d’affinage, afin que le dépôt soit clair et facile à utiliser.
Par ailleurs, vous trouverez plus bas la marche à suivre pour lancer les notebooks Jupyter avec PDM.

## Arborescence
- Dans le dossier **Data**, vous trouverez le fichier Cleaned_Dataframe.csv, qui est le csv de la base de donnée nettoyée.
- Dans le dossier **Cleaning** se trouve le notebook de la base de donnée nettoyée.
- Dans le dossier **Prediction**, vous rouverez les modèles de prédictions utilisés et leurs résultats.
- Pour finir, le dossier **EDA** contient les notebooks de la PCA et des statistiques descriptives
------------------------------------------------------------------------------------------------------------------------------
## Installation et utilisation de l’environnement

### 1. Cloner le dépôt :
```bash
git clone https://github.com/FrancisLabrele/GRAM-ANALYTICS.git
cd GRAM-ANALYTICS
```

### 2. Installer pdm si ce n'est pas déjà fait :
```bash
pip install pdm
```

- (OPTIONNEL) Si vous voyez qu'il manque des librairies/dépendances faites :
```bash
pdm add (le nom de la librairie)
```
- (OPTIONNEL) Les librairies de bases sont déjà installées ainsi que xgboost, lightgbm, catboost et imbalanced-learn
ensuite il faut : 
```bash
  git add pyproject.toml pdm.lock
  git commit -m "Ajout dépendances"
  git push
```

### 3. Mettre à jour l'environnement après le git pull :
```bash
git pull
pdm install
```

### 4. Pour lancer les notebooks :
```bash
pdm run jupyter notebook
```
