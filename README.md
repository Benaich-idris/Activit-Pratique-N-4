# Architecture Transformer — Atelier n°4

## Présentation

Ce projet constitue une étude pratique des architectures de Deep Learning appliquées aux séries temporelles et au traitement automatique du langage naturel (TALN).

Il repose sur l'utilisation de PyTorch et de Hugging Face Transformers pour comprendre, implémenter, entraîner et comparer différentes architectures neuronales.

## Objectifs

- Comprendre les architectures RNN, LSTM et Transformer.
- Étudier les mécanismes de Self-Attention et Multi-Head Attention.
- Comprendre les embeddings et l'encodage positionnel.
- Comparer l'attention causale et bidirectionnelle.
- Expérimenter les modèles pré-entraînés GPT-2 et BERT.
- Implémenter des modèles Transformer à partir de zéro.

## Modèles implémentés

| Modèle | Application |
|---|---|
| RNN | Prédiction d'une série temporelle |
| LSTM | Prédiction d'une série temporelle |
| MiniTransformer | Prédiction temporelle par attention |
| GPT-2 | Génération de texte |
| BERT | Prédiction de tokens masqués |
| EnergyTransformer | Prévision de la consommation électrique |
| Mini-GPT | Génération de texte par caractères |
| Mini-BERT | Reconstruction de mots masqués |

## Exercices complémentaires

### Energy Transformer

Prévision de la puissance électrique de l'heure suivante à partir des 24 dernières heures.

- Agrégation horaire des données.
- Normalisation sans fuite de données.
- Entraînement et validation du Transformer.
- Évaluation avec MAE et RMSE.
- Comparaison avec deux méthodes de référence.

### Mini-GPT

Implémentation d'un modèle de langage autorégressif à partir de zéro.

- Tokenisation par caractères.
- Embeddings de tokens et de positions.
- Attention multi-têtes causale.
- Vérification du masque causal.
- Génération de texte.
- Comparaison de différentes températures.

### Mini-BERT

Implémentation d'un Transformer bidirectionnel à partir de zéro.

- Tokenisation par mots.
- Masked Language Modeling.
- Stratégie de masquage 80/10/10.
- Vérification du masque de padding.
- Évaluation de l'accuracy.
- Prédiction de mots masqués.

## Technologies utilisées

- Python 3.12
- PyTorch
- Hugging Face Transformers
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- Git et GitHub

## Installation

Créer un environnement dédié :

```bash
conda create -n transformer python=3.12 -y
conda activate transformer
pip install -r requirements.txt
```

Enregistrer le kernel Jupyter :

```bash
python -m ipykernel install --user --name transformer --display-name "Python (Transformer)"
```

## Sources des données

- Série temporelle sinusoïdale générée avec PyTorch.
- Individual Household Electric Power Consumption — UCI Machine Learning Repository : https://doi.org/10.24432/C58K54
- Le Tour du monde en quatre-vingts jours — Jules Verne, Project Gutenberg.

Les fichiers de données doivent être placés dans le dossier `data/`, conformément aux chemins utilisés dans le notebook.

## Contexte académique

- Établissement : ENSET Mohammedia
- Encadrant : Pr. Mohamed Youssfi
- Activité pratique n°4 : Architecture Transformer

## Statut

Atelier terminé.