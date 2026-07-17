# Random Forest - Authentification de Billets de Banque

## Description
Ce projet présente l'utilisation de l'algorithme **Random Forest** avec **Scikit-learn** pour détecter automatiquement les **faux billets de banque** à partir de caractéristiques statistiques extraites d'images (variance, asymétrie, curtosis, entropie).
Le notebook montre l'ensemble du processus de modélisation, de l'exploration des données jusqu'à l'optimisation des hyperparamètres et l'étude de l'impact du nombre d'arbres sur la performance.

---

## Objectifs
* Explorer le jeu de données `data_banknote_authentication.csv`.
* Visualiser la séparabilité des classes (pairplot).
* Diviser les données en ensembles d'entraînement et de test.
* Optimiser les hyperparamètres du Random Forest (nombre d'arbres, max_features, bootstrap, oob_score) avec **GridSearchCV**.
* Évaluer le modèle avec le score **Out-Of-Bag (OOB)** et un rapport de classification.
* Étudier l'évolution du taux d'erreur en fonction du nombre d'arbres (n_estimators).

---

## Technologies utilisées
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Structure du projet
```
.
├── RandomForest_Classification_bank.ipynb
├── data_banknote_authentication.csv
└── README.md
```

---

## Résultats
* Une recherche d'hyperparamètres avec **GridSearchCV** identifie la configuration optimale : **bootstrap = True, max_features = 2, n_estimators = 100**.
* Le modèle final atteint un **score Out-Of-Bag (OOB) d'environ 99,4 %**.
* Sur l'ensemble de test, le modèle obtient une **précision globale de 99 %**, avec une très bonne séparation entre billets authentiques et faux billets.

---

## Lancement
1. Cloner le dépôt ou télécharger le notebook.
2. Installer les dépendances :
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```
3. Ouvrir le notebook `RandomForest_Classification_bank.ipynb`.
4. Exécuter les cellules dans l'ordre.

---

## Compétences développées
* Classification binaire
* Algorithme Random Forest (forêts aléatoires)
* Analyse exploratoire des données (EDA) : pairplot
* Optimisation d'hyperparamètres (GridSearchCV)
* Évaluation Out-Of-Bag (OOB Score)
* Étude de la stabilité d'un modèle en fonction du nombre d'estimateurs
* Évaluation de modèles (classification report, matrice de confusion)
* Machine Learning avec Scikit-learn

---

## Auteur
Emmanuel YOHORE
