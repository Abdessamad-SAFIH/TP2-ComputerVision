# 📘 TP2 - Computer Vision

## 🎯 Objectif du projet
Ce projet a pour objectif d’appliquer un **classifieur K-Nearest Neighbors (KNN)**  
à une tâche de **classification d’images** sur le dataset **CIFAR-10**,  
en utilisant une **validation croisée 5-Fold** afin d’analyser l’impact du nombre
de voisins *k* sur les performances du modèle.

L’ensemble du travail est implémenté dans un **notebook Google Colab** en Python,
en s’appuyant sur la bibliothèque **Scikit-learn**.

---

## 🗂 Structure du projet

```text
TP2-ComputerVision/
│
├── README.md
├── TP2-KNN-CIFAR10.ipynb
```
---
## 🧪 Contenu du notebook
1. Présentation du dataset CIFAR-10

- Description du dataset CIFAR-10
- Structure des données (images 32×32×3, 10 classes)
- Chargement des données à l’aide de TensorFlow / Keras
---
## 2. Prétraitement des données
- Réduction du nombre d’images pour accélérer l’exécution
- Aplatissement des images (32×32×3 → 3072 caractéristiques)
- Normalisation des données avec `StandardScaler`
---
## 3. Implémentation du KNN
- Utilisation du classifieur `KNeighborsClassifier` de Scikit-learn
-Construction d’un Pipeline combinant normalisation et KNN
- Test de plusieurs valeurs du paramètre k
---
## 4. Validation croisée 5-Fold
- Application de la validation croisée avec `cross_val_score`
- Calcul de l’accuracy moyenne pour chaque valeur de k
- Analyse de la robustesse des performances
---
## 5. Analyse des résultats
- Tracé de la courbe **Accuracy vs Nombre de voisins (k)**
- Étude de l’effet du sur-apprentissage et du sous-apprentissage
- Identification de la valeur de k offrant le meilleur compromis
---
## 6. Conclusion
- Discussion sur les limites du KNN pour la classification d’images
- Importance du choix des hyperparamètres
- Intérêt de la validation croisée pour l’évaluation des modèles
---
## Clone
Clonez le projet :
```
git clone https://github.com/Abdessamad-SAFIH/TP2-ComputerVision.git
```
---
## Auteur

🧠 Author: Abdessamad

📅 Year: 2025-2026