# 🧠 P6 – Classification automatique de biens de consommation  
**Place de Marché – Marketplace e-commerce**  
Formation Data Scientist – OpenClassrooms  

---

## 🎯 Contexte métier

L’entreprise *Place de Marché* souhaite lancer une marketplace e-commerce anglophone.

Les vendeurs publient leurs articles en ajoutant :
- Une image du produit
- Une description textuelle

Actuellement, l’attribution des catégories produits est réalisée manuellement par les vendeurs, ce qui entraîne :

- Des erreurs de catégorisation
- Une expérience utilisateur dégradée
- Un manque de fiabilité dans la recherche
- Une difficulté à passer à l’échelle

L’objectif est donc d’évaluer la **faisabilité d’un moteur de classification automatique** des produits à partir du texte et de l’image.

---

## 📊 Objectifs du projet

- Prétraiter les données texte et image
- Extraire des features pertinentes
- Réduire la dimensionnalité (projection 2D)
- Visualiser les regroupements produits
- Évaluer la cohérence des clusters
- Mesurer la similarité entre catégories réelles et clusters
- Conclure sur la faisabilité d’un système automatique

---

## 🗃 Données utilisées

Jeu de données comprenant :

- Descriptions textuelles (en anglais)
- Images produits
- Catégories réelles

Aucune contrainte de propriété intellectuelle.

---

# 🔎 Approche 1 : Classification à partir du texte

## 🧹 Prétraitement NLP

- Nettoyage du texte
- Suppression des stopwords
- Lemmatisation
- Normalisation

## 🧠 Extraction de features texte

Plusieurs approches ont été testées :

### 🔹 Bag of Words
- Count Vectorizer
- TF-IDF

### 🔹 Word Embeddings classiques
- Word2Vec / GloVe / FastText

### 🔹 Embeddings avancés
- BERT
- Universal Sentence Encoder (USE)

---

# 🖼 Approche 2 : Classification à partir des images

## 🧹 Prétraitement images

- Redimensionnement
- Normalisation
- Conversion format compatible modèles

## 🧠 Extraction de features image

Deux familles d’approches :

### 🔹 Méthodes classiques
- SIFT / ORB

### 🔹 Deep Learning
- CNN via Transfer Learning
- Extraction des features via modèles pré-entraînés

---

# 📉 Réduction de dimension & Visualisation

- PCA
- Projection 2D
- Visualisation des clusters
- Comparaison avec catégories réelles

---

# 📏 Évaluation

Pour mesurer la similarité entre :

- Catégories réelles
- Clusters obtenus

Utilisation de métriques telles que :

- Score de silhouette
- Indice ARI (Adjusted Rand Index)
- Comparaison visuelle + métrique quantitative

---

# 📊 Résultats

Les analyses montrent que :

- Certaines catégories sont clairement séparables
- Les embeddings avancés (BERT / USE) améliorent la séparation
- Le Transfer Learning CNN améliore la structuration des données images
- Une classification automatique apparaît techniquement faisable

---

# 💡 Conclusion

La faisabilité d’un moteur de classification automatique est démontrée.

Les approches Deep Learning (CNN + embeddings modernes) offrent les meilleures performances.

Ce projet valide la possibilité d’automatiser la catégorisation produits afin :

- D’améliorer l’expérience vendeur
- De fiabiliser la recherche côté acheteur
- De préparer un passage à l’échelle

---

# 📁 Contenu du repository

- Notebook prétraitement et faisabilité texte
- Notebook prétraitement et faisabilité images
- Notebook classification finale
- Notebook script Python
- Présentation projet

---

# 🛠 Technologies utilisées

- Python
- Pandas
- NumPy
- Scikit-Learn
- NLTK / SpaCy
- Word2Vec / BERT / USE
- OpenCV
- CNN (Transfer Learning)
- TensorFlow / Keras
- PCA
- Matplotlib / Seaborn

---

# 👩‍💻 Auteur

Adriana TINT  
Data Scientist – OpenClassrooms  