# ⚽ Prédiction de la Position des Joueurs avec Machine Learning et Deep Learning

---

## 📝 Description du Projet

Ce projet a pour objectif de prédire la position des joueurs de football en fonction de leurs caractéristiques techniques et physiques, telles que la vitesse, l'agilité, la précision, et bien plus. Pour cela, plusieurs techniques de machine learning, y compris un réseau de neurones profonds (deep learning), ont été mises en œuvre. L'objectif est de créer un modèle capable de classifier les joueurs en différentes positions sur le terrain (défenseurs, milieux, attaquants) en se basant sur leurs performances et attributs.

---

## 📂 Organisation du Notebook

### 1. Importation des Bibliothèques

Utilisation de bibliothèques standards telles que :
- **NumPy** : Pour la manipulation des matrices et des tableaux de données.
- **Pandas** : Pour le nettoyage et la préparation des données.
- **Seaborn & Matplotlib** : Pour la visualisation des données.
- **Scikit-learn** : Pour les modèles de machine learning classiques et les métriques d’évaluation.
- **Keras & TensorFlow** : Pour l'implémentation des modèles de deep learning.

### 2. Préparation des Données

- **Nettoyage des Données** : Suppression des colonnes non pertinentes (logos, photos, etc.) et traitement des valeurs manquantes.
- **Encodage des Variables** : Conversion des variables catégorielles (telles que la position et le pied préféré) en variables numériques.
- **Exploration Descriptive** : Visualisation des relations entre différentes variables pour mieux comprendre les données.

### 3. Analyse Exploratoire

- **Corrélations** : Utilisation de `seaborn` et `matplotlib` pour comprendre les liens entre les variables. Par exemple, les relations entre l'âge, la vitesse et les performances des joueurs.
- **Visualisations** : Création de graphes (scatter plots, heatmaps) pour observer les tendances générales et les corrélations.

### 4. Modélisation

Deux modèles principaux ont été construits :
- **Régression Linéaire** : Un modèle simple utilisé pour une estimation rapide et des comparaisons initiales.
- **Modèle de Deep Learning** : Un réseau de neurones multi-couches construit avec Keras, qui permet de mieux capturer les relations non linéaires entre les caractéristiques des joueurs.

### 5. Entraînement des Modèles

- Le modèle de deep learning a été entraîné sur **10 epochs**, avec l'optimiseur **Adam** et la fonction de perte `categorical_crossentropy`.
- Des techniques de **régularisation** ont été appliquées pour éviter l'overfitting.
- Suivi de l'évolution de la **précision** et de la **perte** pendant l'entraînement.

### 6. Évaluation des Modèles

- **Matrice de Confusion** : Utilisée pour évaluer la capacité du modèle à bien classer les joueurs dans leurs positions respectives.
- **Rapport de Classification** : Calcul des scores de **précision**, de **rappel** et des **F1-scores** pour chaque classe (position sur le terrain).
- **Précision Globale** : Le modèle de deep learning a atteint une précision de **88 %** sur le jeu de test.
- **Visualisation des Prédictions** : Une régression linéaire a été utilisée pour observer la relation entre les prédictions et les valeurs réelles.

---

## 🤖 Choix des Modèles et Justifications

- **Modèle de Deep Learning** : Sélectionné pour sa capacité à capturer des relations complexes entre les caractéristiques des joueurs.
- **Régression Linéaire** : Utilisée comme base pour comparer la performance avec les réseaux de neurones.

---

## 📊 Interprétation des Résultats

- **Analyse des Échecs** : Le modèle a eu du mal à différencier certaines positions proches, comme les milieux offensifs et les attaquants, en raison de leurs similitudes en termes de caractéristiques.
- **Interprétation des Métriques** : Bien que la précision globale soit satisfaisante, certaines classes sous-représentées pourraient être améliorées.

---

## 📈 Conclusion

Ce projet a permis de développer un modèle performant pour prédire les positions des joueurs de football à partir de leurs caractéristiques techniques et physiques. Le modèle de deep learning a bien différencié les joueurs, mais des améliorations futures pourraient se concentrer sur les classes sous-représentées pour encore mieux capturer les distinctions entre les positions.

---

## 🚀 Comment Exécuter le Projet

1. **Cloner le dépôt Git** :
   ```bash
   git clone <url_du_projet>
2. **Installer les dépendances** :
   ```bash
   pip install -r requirements.txt
3. **Exécuter le notebook** : 
Ouvrir le notebook dans Jupyter ou Google Colab pour explorer les résultats et répliquer l'entraînement des modèles.

