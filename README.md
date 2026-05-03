# 🛡️ Détection de Fraude par Carte Bancaire

### Machine Learning — Groupe 25 | ESTIAM Paris

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3-orange?logo=scikit-learn)
![Gradio](https://img.shields.io/badge/Gradio-4.x-teal)
![Kaggle](https://img.shields.io/badge/Kaggle-Dataset-20BEFF?logo=kaggle)
![Status](https://img.shields.io/badge/Statut-R03%20Terminé-brightgreen)

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

- **Source :** [Kaggle — Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Taille :** 284 807 transactions × 31 colonnes
- **Fraudes :** 492 (0,17%) — ratio 578:1
- **Features :** Time, Amount, V1–V28 (PCA), Class (0=Légitime, 1=Fraude)


-----

## 🗂️ Structure du projet

```
credit-card-fraud-detection/
│
├── 📓 notebooks/
│   └── Rendu03_Groupe25_Final.ipynb   # Notebook principal (EDA + ML + Évaluation)
│
├── requirements.txt                   # Dépendances Python
├── .gitignore
└── README.md
```

-----

## 🚀 Avancement — Sprints Scrum

|Sprint |Epic |Description |Statut |
|--------|------|--------------------------------------|----------|
|Sprint 1|EPIC 1|Import & Exploration (EDA) |✅ Terminé |
|Sprint 2|EPIC 2|Prétraitement — Classe `Pretraitement`|✅ Terminé |
|Sprint 3|EPIC 3|Modèles ML — Classe `ModeleML` |✅ Terminé|
|Sprint 3|EPIC 4|Évaluation — Classe `Evaluation` |✅ Terminé|
|Sprint 4|EPIC 5|Interface Gradio complète |🔜 En cours |
|Sprint 5|EPIC 6|Export Power BI |⏳ Prévu |
|Sprint 6|EPIC 7|Tests finaux + Documentation |⏳ Prévu |

-----

## ⚙️ Installation

```bash
# 1. Cloner le dépôt
git clone https://github.com/marwadr/credit-card-fraud-detection.git
cd credit-card-fraud-detection

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Télécharger le dataset depuis Kaggle
# https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
# Placer le fichier creditcard.csv dans un dossier data/ à la racine
```

-----

## 🚀 Lancer le notebook

```bash
jupyter notebook notebooks/Rendu03_Groupe25_Final.ipynb
```

Le notebook peut également être exécuté directement sur Kaggle (sans installation) :
👉 [credit-card-fraud-detection sur Kaggle](https://www.kaggle.com/code/khadidjatarch/credit-card-fraud-detection)

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

## 📈 Résultats 

| Modèle              | Accuracy   | Précision  | Rappel | F1-score   | ROC-AUC    |
| ------------------- | ---------- | ---------- | ------ | ---------- | ---------- |
| Logistic Regression | 0.9741     | 0.0539     | 0.8737 | 0.1015     | 0.9601     |
| Decision Tree       | 0.9896     | 0.1137     | 0.7684 | 0.1981     | 0.8535     |
| Random Forest       | **0.9993** | **0.7732** | 0.7895 | **0.7812** | **0.9729** |
| XGBoost             | 0.9762     | 0.0571     | 0.8526 | 0.1070     | 0.9510     |




-----

*Projet pédagogique — ESTIAM Paris | Avril 2026*
