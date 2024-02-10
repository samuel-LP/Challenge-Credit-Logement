# Challenge Crédit Logement - MoSEF

## Description

L'objectif de ce challenge consiste à développer un modèle prédictif capable d'anticiper les cas de Déchéance du Terme (DET) en se basant sur un ensemble de données détaillées relatives aux incidents de paiement des individus.
Pour cela, nous avons commencer par réaliser un travail d'analyse et de préparation des données. Nous avons ensuite développer plusieurs modèles : Logit, XGBoost, ainsi que 3 modèles de durées différents. 

## Structure du Projet

Le projet est structuré comme suit :

- `data/` : Dossier contenant les données utilisées pour le modèle.
    - `base_modelis_pass_det.csv` : Le dataset principal pour le modèle.
    - `df_duree.csv` : Le dataset contenant les données préparées pour les modèles de durée. 
    - `df_logit_xgb` : Le dataset contenant les données préparées pour les modèles logit et XGBoost. 
    - `dictionnaire.json` : Un fichier JSON contenant la définition des variables.
    - `Dictionnaire.xlsx` : Un fichier Excel avec le dictionnaire de données.

- `notebook/` : Dossier contenant les Jupyter Notebooks pour l'analyse et la modélisation.
    - `Analyse_exploratoire.ipynb` : Notebook pour l'analyse exploratoire des données.
    - `CoxPHFitter - Explicabilité.ipynb` : Notebook dédié au modèle de Cox Proportional Hazards - Explicabilité.
    - `CoxPHFitter - Performance.ipynb` : Notebook au modèle de Cox Proportional Hazards - Performance.
    - `CoxTimeVaryingFitter.ipynb` : Notebook au modèle de Cox à effets mixtes.
    - `Data treatment.ipynb` : Notebook pour le prétraitement des données.
    - `Logit baseline.ipynb` : Notebook pour la mise en place d'un modèle de régression logistique.
    - `XGBoost.ipynb` : Notebook pour la modélisation et l'évaluation d'un modèle XGBoost.

## Pour récupérer le projet

1. Cloner le repository

    ```bash
    git clone https://github.com/samuel-LP/finance_quant.git
    ```

2. Créer un environnement virtuel

   2.1 Pour Windows : 
   
   ```bash
    python -m venv venv
    .\venv\Scripts\activate
   ```
   
   2.2  Pour Mac/Linux : 

   ```bash
    python3 -m venv venv
    source venv/bin/activate
   ```

3. Installer les dépendances : 
   ```bash
    pip install -r requirements.txt
   ```

## Authors

- [Samuel Baheux](https://github.com/SamuelBaheux)
- [Samuel Launay Pariente](https://github.com/samuel-LP)
- [Axel Fritz](https://github.com/AxelFritz1)