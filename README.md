# 🛡️ Détection de Fraude par Carte Bancaire

### Machine Learning — Groupe 25 | ESTIAM Paris

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3-orange?logo=scikit-learn)
![Gradio](https://img.shields.io/badge/Gradio-4.x-teal)
![Kaggle](https://img.shields.io/badge/Kaggle-Dataset-20BEFF?logo=kaggle)
![Status](https://img.shields.io/badge/Statut-En%20cours-yellow)

-----

## 👥 Équipe

|Nom |Rôle Scrum |
|------------------|-------------|
|DRIHEM Marwa |Product Owner|
|TARCHOUNE Khadidja|Scrum Master |

**École :** ESTIAM Paris 
**Notebook Kaggle :** [credit-card-fraud-detection](https://www.kaggle.com/code/khadidjatarch/credit-card-fraud-detection)

-----

## 🎯 Objectif

Développer un système intelligent capable de détecter automatiquement les transactions bancaires frauduleuses à partir d’un dataset réel fortement déséquilibré (seulement **0,17% de fraudes**).

-----

## 📊 Dataset

- **Source :** [Kaggle — Credit Card Fraud Detection]
- **Taille :** 284 807 transactions × 31 colonnes
- **Fraudes :** 492 (0,17%) — ratio 578:1
- **Features :** Time, Amount, V1–V28 (PCA), Class (0=Légitime, 1=Fraude)


-----

## 🗂️ Structure du projet

```
credit-card-fraud-detection-groupe25/
│
├── 📓 notebooks/
│ └── Rendu03_Groupe25_Final.ipynb # Notebook principal Kaggle
│
├── 🐍 src/
│ └── gradio_groupe25.py # Interface Gradio (5 onglets)
│
├── 🤖 models/
│ └── fraud_model_g25.pkl # Modèle entraîné (joblib)
│
├── 📄 docs/
│ ├── Document_Conception_R02.pdf # Rendu 02 — Conception
│ └── Rendu03_G25_COMPLET.pdf # Rendu 03 — Rapport
│
├── .gitignore
├── requirements.txt
└── README.md
```

-----

## 🚀 Avancement — Sprints Scrum

|Sprint |Epic |Description |Statut |
|--------|------|--------------------------------------|----------|
|Sprint 1|EPIC 1|Import & Exploration (EDA) |✅ Terminé |
|Sprint 2|EPIC 2|Prétraitement — Classe `Pretraitement`|✅ Terminé |
|Sprint 3|EPIC 3|Modèles ML — Classe `ModeleML` |🔜 En cours|
|Sprint 3|EPIC 4|Évaluation — Classe `Evaluation` |🔜 En cours|
|Sprint 4|EPIC 5|Interface Gradio complète |🔜 En cours|
|Sprint 5|EPIC 6|Export Power BI |⏳ Prévu |
|Sprint 6|EPIC 7|Tests finaux + Documentation |⏳ Prévu |

-----

## ⚙️ Installation

```bash
# 1. Cloner le dépôt
git clone https://github.com/[votre-username]/credit-card-fraud-detection-groupe25.git
cd credit-card-fraud-detection-groupe25

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Placer le dataset dans le dossier data/
# Télécharger depuis : https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
```

-----

## 🧪 Technologies utilisées

|Librairie |Usage |
|------------------------|-------------------------------------|
|`pandas` / `numpy` |Manipulation des données |
|`scikit-learn` |Modèles ML, prétraitement, évaluation|
|`imbalanced-learn` |SMOTE — rééquilibrage des classes |
|`xgboost` |Gradient Boosting |
|`matplotlib` / `seaborn`|Visualisations |
|`gradio` |Interface utilisateur |
|`joblib` |Sauvegarde du modèle |

-----

## 📈 Résultats (en cours)

|Modèle |Precision|Recall|F1-Score|ROC-AUC|
|-------------------|---------|------|--------|-------|
|Logistic Regression|— |— |— |— |
|Random Forest |— |— |— |— |
|XGBoost |— |— |— |— |




-----

*Projet pédagogique — ESTIAM Paris | Avril 2026*
