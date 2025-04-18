📝 Analyse des Avis McDonald's
📌 Description du Projet
Ce projet utilise Python et Machine Learning pour analyser les avis clients de McDonald's. L'objectif est de : ✅ Nettoyer et préparer les données textuelles ✅ Catégoriser les avis en positif, neutre ou négatif ✅ Visualiser la distribution des sentiments ✅ Entraîner un modèle de classification des avis et analyser ses performances

📂 Données utilisées
Le dataset translated_McDonald_s_Reviews.csv contient les avis clients et leurs évaluations sous forme de notation (1 à 5 étoiles).

Les principales étapes du traitement sont : 🔹 Suppression des valeurs manquantes 🔹 Création d'une colonne "feeling" pour catégoriser les avis selon les notes 🔹 Nettoyage et tokenisation des avis textuels

📊 Exploration des données
📌 Distribution des notes
Un graphique en barres permet d'observer la répartition des avis par nombre d'étoiles.

📌 Distribution des sentiments
Les avis sont classés en trois catégories : ✔️ Positif : 4 et 5 étoiles ➖ Neutre : 3 étoiles ❌ Négatif : 1 et 2 étoiles

Un graphique montre cette répartition.

📌 Nuage de mots
Un WordCloud est généré pour visualiser les mots les plus fréquemment utilisés dans les avis.

🛠 Modélisation avec NLP & Machine Learning
🔹 Vectorisation des avis via TfidfVectorizer 🔹 Entraînement d'un modèle Random Forest pour la classification 🔹 Évaluation des performances avec classification_report et roc_auc_score

📌 Résultats du modèle
Sentiment	Précision	Recall	F1-score	Support
Négatif	0.82	0.91	0.86	2543
Neutre	0.80	0.41	0.54	939
Positif	0.85	0.90	0.87	3198
✅ Accuracy : 83% ✅ AUC Score : 0.919

Ces résultats montrent que le modèle est performant pour détecter les avis positifs et négatifs, bien que la classification des avis neutres soit plus difficile.
