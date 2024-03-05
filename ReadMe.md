# Challenge Crédit Logement - MoSEF


## Description
The aim of this challenge is to develop a predictive model capable of anticipating cases of Term Default (DET) by relying on a detailed dataset of individuals' payment incidents. To achieve this, we began by conducting data analysis and preparation work. We then developed several models: Logit, XGBoost, as well as 3 different duration models.

## Project Structure
The project is structured as follows:

- `notebook/`: Folder containing the Jupyter Notebooks for analysis and modeling.
    - `Analyse_exploratoire.ipynb`: Notebook for the exploratory data analysis.
    - `CoxPHFitter - Explicability.ipynb`: Notebook dedicated to the Cox Proportional Hazards model - Explicability.
    - `CoxPHFitter - Performance.ipynb`: Notebook for the Cox Proportional Hazards model - Performance.
    - `CoxTimeVaryingFitter.ipynb`: Notebook for the Cox model with mixed effects.
    - `Data treatment.ipynb`: Notebook for data preprocessing.
    - `Logit baseline.ipynb`: Notebook for setting up a logistic regression model.
    - `XGBoost.ipynb`: Notebook for modeling and evaluating an XGBoost model.
  
## To retrieve the project

1. Clone the repository

    ```bash
    git clone git@github.com:samuel-LP/challenge-credit-logement.git
    cd challenge-credit-logement
    ```

2. Create a virtual environment

   2.1 for Windows : 
   
   ```bash
    python -m venv venv
    .\venv\Scripts\activate
   ```
   
   2.2  for Mac/Linux : 

   ```bash
    python3 -m venv venv
    source venv/bin/activate
   ```

3. Install dependencies : 
   ```bash
    pip install -r requirements.txt
   ```

## Authors

- [Samuel Baheux](https://github.com/SamuelBaheux)
- [Samuel Launay Pariente](https://github.com/samuel-LP)
- [Axel Fritz](https://github.com/AxelFritz1)
