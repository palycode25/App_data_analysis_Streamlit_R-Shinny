# README - Application interactive de Data Analysis

## Description

Application interactive permettant d'explorer un jeu de données (CSV/Excel), de visualiser ses variables et d'entraîner un modèle prédictif simple, sans écrire de code. Deux versions sont disponibles : une en **R (Shiny)** et une en **Python (Streamlit)**.

## Fonctionnalités

- **Import de données** : fichiers CSV ou Excel
- **Aperçu et statistiques descriptives** : variables numériques et catégorielles
- **Visualisations** :
  - Univariées : histogrammes, boxplots, barplots
  - Bivariées : nuages de points, boxplots croisés, heatmaps de contingence
  - Multivariées : heatmap des corrélations
- **Modélisation prédictive** :
  - Détection automatique de la tâche (régression ou classification) selon la variable cible
  - Choix du modèle : régression linéaire / logistique ou Random Forest
  - Séparation train/test paramétrable
  - Affichage des métriques (R², RMSE, MAE pour la régression ; Accuracy, F1 pour la classification)

## Stack technique

**Version R** : Shiny, dplyr, ggplot2, caret, randomForest
**Version Python** : Streamlit, pandas, scikit-learn, matplotlib, seaborn

## Lancer l'application

**R (Shiny)**

\`\`\`r
shiny::runApp("app.R")
\`\`\`

**Python (Streamlit)**

\`\`\`bash
streamlit run app.py
\`\`\`

## Utilisation

1. Charger un fichier CSV ou Excel via la barre latérale
2. Explorer les données dans les onglets Aperçu / Univarié / Bivarié / Multivarié
3. Choisir une variable cible et des variables explicatives
4. Sélectionner un modèle et consulter les métriques de performance
