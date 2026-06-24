# 🚗 Analyse de l'Accidentalité Routière en France (2024)

## 📌 Présentation

Ce projet analyse les accidents corporels de la circulation routière en France en 2024 à partir des données ouvertes de l'accidentalité routière.

L'objectif est d'identifier les facteurs de risque, mesurer la gravité des accidents, classer les types de routes selon leur niveau de risque et proposer des recommandations pour améliorer la sécurité routière.

---

## 🎯 Objectifs

* Analyser la répartition des accidents dans le temps.
* Étudier l'influence des conditions météorologiques.
* Comparer les différents types de routes.
* Mesurer la gravité des accidents.
* Construire un score de risque.
* Générer des recommandations d'aide à la décision.

---

## 📂 Structure du projet

```text
.
├── caract-2024.csv
├── lieux-2024.csv
├── usagers-2024.csv
├── analyse_accidents.py
├── classement_risque.csv
└── README.md
```

---

## 📊 Données utilisées

Les analyses reposent sur trois fichiers :

| Fichier          | Description                               |
| ---------------- | ----------------------------------------- |
| caract-2024.csv  | Caractéristiques générales des accidents  |
| lieux-2024.csv   | Informations sur les lieux des accidents  |
| usagers-2024.csv | Informations sur les personnes impliquées |

---

## 🛠 Technologies

* Python
* Pandas
* Matplotlib

---

## ⚙️ Méthodologie

### 1. Chargement des données

Import des trois jeux de données.

### 2. Agrégation des usagers

Calcul du nombre de :

* tués ;
* blessés hospitalisés ;
* blessés légers ;

pour chaque accident.

### 3. Fusion des données

Fusion des tables à l'aide de l'identifiant unique :

```python
Num_Acc
```

### 4. Création de variables

* Date complète de l'accident.
* Variable indiquant si l'accident est grave.

### 5. Analyse exploratoire

Production de visualisations :

* Nombre d'accidents par mois ;
* Accidents selon la météo ;
* Accidents selon le type de route ;
* Accidents selon la vitesse maximale autorisée.

### 6. Calcul du taux de gravité

Un accident est considéré comme grave lorsqu'il comporte au moins :

* un tué ;
* ou un blessé hospitalisé.

### 7. Construction d'un score de risque

Le score de risque est défini par :

```text
Score = Accidents + 3 × Blessés graves + 5 × Tués
```

Ce score permet de hiérarchiser les types de routes selon leur dangerosité.

---

## 📈 Résultats

Le programme produit :

* Des graphiques d'analyse.
* Un tableau de bord statistique.
* Un classement des types de routes selon leur score de risque.
* Un fichier d'export CSV.

---

## 📁 Export

```text
classement_risque.csv
```

Ce fichier contient le classement des catégories de routes du plus risqué au moins risqué.

---

## 🚀 Installation

Cloner le dépôt :

```bash
git clone https://github.com/votre-utilisateur/accidentalite-routiere.git
```

Installer les dépendances :

```bash
pip install pandas matplotlib
```

Lancer le script :

```bash
python analyse_accidents.py
```

---

## 💡 Perspectives d'amélioration

* Développement d'un tableau de bord interactif avec Streamlit ou Power BI.
* Modèle de Machine Learning pour prédire la gravité des accidents.
* Analyse géographique des zones accidentogènes.
* Intégration de données météorologiques en temps réel.
* Détection automatique des zones à risque.

---

## 👤 Auteur

**Lamessi Jérôme OGAH**

Étudiant en Master Modélisation de Données – Université de Lille

Intéressé par la Data Science, la modélisation statistique, l'intelligence artificielle et l'aide à la décision.
