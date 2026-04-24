# Approche Semi-Supervisée pour l'Apprentissage sur des IRM

Ce projet implémente une approche d'apprentissage semi-supervisé appliquée à l'analyse d'images par résonance magnétique (IRM). Le pipeline complet couvre l'exploration des données, le prétraitement des images, des méthodes d'apprentissage non supervisé (clustering) et la modélisation semi-supervisée finale en utilisant PyTorch et Scikit-Learn.

## Structure du Projet

Le projet est divisé en plusieurs notebooks séquentiels, documentant chaque étape de la pipeline de traitement et de modélisation :

- **`notebooks/1_EDA.ipynb`** : Analyse Exploratoire des Données (EDA). Visualisation et compréhension de la distribution des données IRM.
- **`notebooks/2_pretraitement.ipynb`** : Prétraitement des images. Nettoyage, normalisation et augmentation des données (utilisant OpenCV et Pillow).
- **`notebooks/3_clustering.ipynb`** : Regroupement (Clustering). Application de techniques d'apprentissage non supervisé pour identifier des structures sous-jacentes dans les données.
- **`notebooks/4_mss.ipynb`** : Modèle Semi-Supervisé (MSS). Entraînement du modèle final en exploitant à la fois les données étiquetées et non étiquetées.

## Prérequis

- Python `>= 3.11` et `< 3.15`
- [Poetry](https://python-poetry.org/) pour la gestion des dépendances.

## Installation

Le projet utilise `pyproject.toml` et `poetry.lock` pour garantir des environnements reproductibles.

1. Cloner le dépôt :

   ```bash
   git clone <https://github.com/EthanChmt/semi-supervised-mri-learning>
   cd semi-supervised-mri-learning
   ```

2. Installer les dépendances avec Poetry :

   ```bash
   poetry install
   ```

3. Activer l'environnement virtuel :

   ```bash
   poetry shell
   ```

## Stack Technique Principale

| Catégorie | Bibliothèques |
|---|---|
| Manipulation de données & Calculs | `numpy`, `pandas` |
| Visualisation | `matplotlib`, `seaborn` |
| Traitement d'images | `pillow`, `opencv-python` |
| Machine Learning & Deep Learning | `scikit-learn`, `torch`, `torchvision` |
| Suivi de progression | `tqdm` |

## Auteurs

- Chaumeret : ethan.chaumeret@gmail.com