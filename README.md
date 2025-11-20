# Recherche Semantique et Classification de Livres
Dans ce projet j'implémente un système de recherche sémantique et de classification automatique de livres utilisant l'IA d'**OpenAI** ainsi que **HuggingFace** et le traitement du langage naturel.
## Objectifs Principaux:
Exploration et nettoyage d'un dataset de livres importé depuis kaggle  
Classification automatique des livres en Fiction/Non-fiction  
Recherche sémantique basée sur la similarité des descriptions  
## Technologies:
NLP: Transformers (Hugging Face)  
Embeddings: OpenAI  
Base vectorielle: ChromaDB  
Classification: Modèle BART-large-mnli de facebook  
Data Processing: Pandas, NumPy  
## Fonctionnalités principales
1.Exploration & Nettoyage (**exploration.py**):
-Télécharge automatiquement le dataset Kaggle (7k livres)
-Nettoie les données et filtre les descriptions courtes
-Crée des variables dérivées et analyse les corrélations
**livres_nettoyes.csv** comme sortie
2.Classification Automatique (**classification_texte.py**)
-Utilise BART-large-mnli pour classification zero-shot
-Catégorise les livres en Fiction/Non-fiction
-Évalue la performance
-Complète automatiquement les catégories manquantes
**livres_avec_categories.csv** comme sortie
3.Recherche Sémantique (**recherche_semantique.py**)
-Embeddings OpenAI + base vectorielle ChromaDB
-Recherche par similarité sémantique
-Interface interactive pour requêtes naturelles
Retourne livres pertinents avec métadonnées complètes
Pour la realisation de ce projet, je me suis inspiré en appliquant les concepts de machine learning appris à travers diverses ressources éducatives dont aussi freecodecamp
