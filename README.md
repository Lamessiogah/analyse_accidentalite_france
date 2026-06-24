# 🚗 Analyse de l'Accidentalité Routière en France (2024)

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)

Projet d'analyse exploratoire des accidents corporels de la circulation en France à partir des données ouvertes 2024.

Objectif : identifier les facteurs de risque routier, mesurer la gravité des accidents et construire des indicateurs d'aide à la décision pour la sécurité routière.
## 📌 Présentation

Ce projet analyse les accidents corporels de la circulation routière en France en 2024 à partir des données ouvertes de l'accidentalité routière.

L'objectif est d'identifier les facteurs de risque, mesurer la gravité des accidents, classer les types de routes selon leur niveau de risque et proposer des recommandations pour améliorer la sécurité routière.

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
## 📌 Résultats clés

L'analyse a permis de :

- Identifier les catégories de routes les plus accidentogènes.
- Mesurer le taux d'accidents graves selon le type d'infrastructure.
- Évaluer l'influence des conditions météorologiques.
- Construire un score de risque combinant fréquence et gravité des accidents.
- Générer automatiquement un classement des infrastructures prioritaires.

---

## 📷 Visualisations

### Tableaux de bord
![Affichage du terminal](https://github.com/Lamessiogah/analyse_accidentalite_france/blob/main/tableau%20de%20bord.png)

### Accidents par mois

![Accidents par mois](https://github.com/Lamessiogah/analyse_accidentalite_france/blob/main/accidents%20mois.png)

### Accidents selon la météo

![Météo](https://github.com/Lamessiogah/analyse_accidentalite_france/blob/main/accidents%20meteo.png)

### Accidents par type de route

![Routes](https://github.com/Lamessiogah/analyse_accidentalite_france/blob/main/accidents%20route.png)

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
git clone https://github.com/Lamessiogah/analyse_accidentalite_france.git
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

🎓 Master Modélisation de Données – Université de Lille

📊 Data Analytics | Data Science | Machine Learning

🔗 LinkedIn : https://www.linkedin.com/in/lamessi-jer%C3%B4me-ogah-b14186329/
