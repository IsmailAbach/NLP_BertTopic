# BERTopic – Topic Modeling Project

Ce projet consiste à appliquer **BERTopic** pour réaliser du **topic modeling** sur des données textuelles, en combinant des techniques modernes de **NLP**, de **clustering non supervisé** et de **visualisation**.

Le projet a été développé et exécuté sur **Google Colab**.

---

## Objectif du projet
- Extraire automatiquement des **thèmes (topics)** à partir d’un corpus de textes  
- Regrouper les documents sémantiquement similaires  
- Analyser et interpréter la structure thématique des données textuelles  

---

## Méthodologie

Le pipeline BERTopic utilisé suit les étapes suivantes :

1. **Embedding**
   - Transformation des textes en vecteurs numériques à l’aide de modèles **Transformer** afin de capturer le sens sémantique des documents.

2. **Réduction de dimension**
   - Utilisation de **UMAP** pour réduire la dimension des embeddings tout en conservant la structure sémantique globale.

3. **Clustering**
   - Regroupement des documents similaires à l’aide de **HDBSCAN**, sans fixer à l’avance le nombre de clusters.

4. **Vectorisation avec c-TF-IDF**
   - Application de la méthode **Class-based TF-IDF (c-TF-IDF)** pour identifier les mots les plus représentatifs de chaque topic.

5. **Modélisation des topics**
   - Génération des topics finaux à partir des clusters et des scores c-TF-IDF, chaque topic étant représenté par un ensemble de mots clés.

6. **Visualisation**
   - Visualisation de la distribution des topics et de leurs relations afin de faciliter l’analyse et l’interprétation des résultats.

---

## Technologies utilisées
- Python  
- BERTopic  
- Sentence Transformers  
- UMAP  
- HDBSCAN  
- c-TF-IDF  
