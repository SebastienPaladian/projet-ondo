# 💹 Analyse du Token ONDO – Data Science & Visualisation



## 🧠 Contexte du projet

Ce projet a été réalisé dans un cadre professionnel afin d’analyser les variations de prix et de volume du token **ONDO**, une cryptomonnaie récente.  
L’objectif était de mettre en place une démarche complète de **Data Analysis** et de **Machine Learning** pour :
- détecter les anomalies de marché,
- comprendre les tendances de fond,
- et proposer une **aide à la décision** visuelle pour les investisseurs.



## 🚀 Objectifs
- Nettoyer et structurer des données de marché issues d’un fichier Excel
- Détecter les anomalies de comportement via un algorithme d’**Isolation Forest** (Python)
- Concevoir un **dashboard Power BI interactif** pour restituer les insights
- Créer une **présentation claire** à destination d’un public non-technique



## 🧰 Outils & technologies

| Outil       | Usage principal                           |
|-------------|--------------------------------------------|
| **Python**  | Traitement des données, Machine Learning  |
| **Excel (.xlsx)** | Source de données brute                |
| **Power BI**| Dashboard visuel et interactif            |
| **PowerPoint** | Support de présentation synthétique   |


## 📁 Contenu du dépôt
- `ondo_analysis.ipynb` : Notebook Jupyter avec le code Python complet
- `ondo_data_brute.xlsx`: Données brutes
- `ondo_data_new.xlsx` : Données utilisées pour l’analyse
- `ondo_dashboard.pbix` : Rapport Power BI interactif
- `ondo_projet_presentation.pptx`
- `img/` : Images (captures d’écran du dashboard, graphiques)
  

## 🔍 Démarche analytique

### 1. Introduction
Le projet porte sur l’analyse du token ONDO, une cryptomonnaie liée à la tokenisation des actifs du monde réel (RWA). L’objectif est de comprendre les variations de prix et de volume sur l’année 2024–2025, et d’identifier les anomalies de marché via des méthodes d’analyse avancées.



### 2. Analyse exploratoire des données
- **Prix du token ONDO** :
  - Forte croissance entre janvier et juin 2024, atteignant un sommet à 1,5 $.
  - Stabilisation entre juillet et octobre 2024.
  - Nouveau pic historique à 2,0 $ en décembre, suivi d’une correction en janvier 2025.

- **Volumes de transaction** :
  - Volatilité élevée typique des cryptomonnaies.
  - Pics majeurs en avril, décembre 2024 et janvier 2025.
  - Corrélation partielle entre le volume et le prix observée.



### 3. Détection d’anomalies
- Utilisation des **boxplots** (boîtes à moustaches) pour détecter les variations anormales :
  - **Prix** : valeurs aberrantes détectées entre -18 % et +23 %.
  - **Volumes** : plusieurs outliers liés à des événements majeurs (ex. : partenariats, annonces stratégiques).



### 4. Visualisations & Corrélations
- Création d’une **matrice de corrélation** pour identifier les liens entre les variables clés :
  - Corrélation forte entre **prix et market cap** (+0,93).
  - Corrélation modérée entre **volume et market cap** (~0,51).
  - Absence de corrélation négative marquée, montrant une dynamique globalement positive ou neutre.



### 5. Modélisation prédictive
- Objectif : **prédire le prix et le volume du token** à partir des autres variables.
- Méthode : **régression linéaire**, évaluée avec MSE et R² Score.
  - **Target “Close en $”** :
    - MSE faible, mais R² = 0,17 → capacité explicative limitée.
  - **Target “Volume en $”** :
    - MSE élevé, R² = 0,34 → résultats moyens.

📌 **Interprétation** : la régression linéaire ne suffit pas à modéliser la complexité du marché crypto. Des modèles non-linéaires seraient plus adaptés (Random Forest, XGBoost, LSTM...).



### 6. Recommandations pour les investisseurs
- Surveiller les périodes de pics de volatilité (ex. : lancements, annonces, unlocks de tokens).
- Attendre les corrections après des pics pour limiter les risques.
- Diversifier son portefeuille pour réduire l’exposition au token ONDO.
- Utiliser des indicateurs techniques (RSI, ATR) pour affiner les points d’entrée/sortie.



### 7. Conclusion & pistes futures
- Le modèle met en évidence des **périodes critiques et des anomalies significatives**, utiles pour orienter les décisions d’investissement.
- Les limites identifiées (volatilité, données limitées, simplicité du modèle) ouvrent des **perspectives d’amélioration** :
  - Ajouter des données macroéconomiques et sociales.
  - Tester des algorithmes plus avancés.
  - Mettre en place un système d’alerte basé sur la détection d’anomalies.



## 👤 À propos de moi

Je suis passionné(e) par la **data analyse**, la **visualisation interactive** et l’**application concrète des outils data à des problématiques métiers**.  
Ce projet illustre ma capacité à **combiner Python, Excel et Power BI** pour produire des analyses actionnables.

**Sébastien PALADIAN** – [sebastien.paladian@gmail.com] – [LinkedIn](https://www.linkedin.com/in/sebastien-paladian/)

Merci pour votre intérêt pour ce projet !
