Projet GRAM-ANALYTICS

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
