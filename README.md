# 🎬 Recommandation de Films avec Machine Learning

## 📌 Présentation du projet  
Ce projet implémente un **système de recommandation de films** basé sur l’apprentissage automatique. Il utilise un modèle de **filtrage collaboratif** pour prédire les films susceptibles d’intéresser un utilisateur en fonction des évaluations passées.  

✅ **Objectifs :**  
- Recommander des films personnalisés aux utilisateurs  
- Explorer différentes techniques de recommandation  
- Comparer les performances des modèles et optimiser les recommandations  

🔍 **Technologies utilisées :**  
- 🐍 **Python**  
- 📊 **Pandas, NumPy** (manipulation des données)  
- 🎭 **Surprise** ou **Scikit-Learn** (algorithmes de recommandation)  
- 📈 **Matplotlib, Seaborn** (visualisation)  
- 🚀 **Streamlit / FastAPI** (si mise en production)  

---

## 📂 Structure du projet  
```
📁 Films_recommandations
│── 📄 Films_recommandations.ipynb  # Notebook principal avec le code du projet  
│── 📄 requirements.txt  # Dépendances du projet  
│── 📄 README.md  # Documentation
│── 📄 LICENCE 
```

---

## 🛠️ Installation et exécution  
### 1️⃣ **Cloner le projet**  
```bash
git clone https://github.com/arnaudstdr/films_reco.git
cd films-recommandation
```

### 2️⃣ **Créer un environnement virtuel et installer les dépendances**  
```bash
python -m venv env
source env/bin/activate  # Sur macOS/Linux
env\Scripts\activate  # Sur Windows

pip install -r requirements.txt
```

### 3️⃣ **Lancer le notebook**  
Ouvrir Jupyter Notebook et exécuter `Films_recommandations.ipynb`  
```bash
jupyter notebook
```
---

## 📊 Exploration des données  
Les données utilisées proviennent d’un dataset contenant :  
- **Users** : ID utilisateur  
- **Movies** : ID des films et métadonnées (titre, genre…)  
- **Ratings** : Notes attribuées par les utilisateurs aux films (ex. : 1 à 5 étoiles)  

#### 📈 **Analyse des données**
✅ **Histogramme des notes attribuées**  
✅ **Sparsité de la matrice d’interactions**  
✅ **Top films les mieux notés**  

---

## 🏆 Modèles de recommandation  
Trois approches ont été explorées :  

| Modèle | Type | Avantages | Inconvénients |
|--------|------|-----------|--------------|
| Moyenne des notes | Baseline | Simple, rapide | Pas personnalisé |
| Filtrage collaboratif (SVD, KNN) | ML | Personnalisation, performance correcte | Cold start problem |
| Hybridation (collaboratif + contenu) | ML | Meilleure précision | Plus complexe, plus de données nécessaires |

---

## 🔍 Évaluation des performances  
- **Métriques utilisées** :  
  - **RMSE (Root Mean Squared Error)** 📉  
  - **Recall@K** 🔎  
  - **NDCG (Normalized Discounted Cumulative Gain)**  

- **Résultats obtenus :**  
  - Modèle SVD : **RMSE = 0.95**  
  - Modèle KNN : **RMSE = 1.02**  

---

## 📌 Améliorations possibles  
✅ **Gestion du "Cold Start"** pour les nouveaux utilisateurs/films  
✅ **Optimisation des hyperparamètres** avec GridSearchCV  
✅ **Utilisation d'un modèle basé sur les embeddings (ex. : Autoencoder)**  
✅ **Déploiement via Streamlit pour une démo interactive**  

---

## 📜 Licence  
Ce projet est sous licence MIT. Vous êtes libre de l’utiliser et de le modifier.  

---

## 👨‍💻 Auteur  
🎯 **[arnaudstdr](https://github.com/arnaudstdr)** – Machine Learning Developer Junior 🎬  
