# tags-generator-nlp

## Description
Projet NLP: prédiction d'une liste de 5 tags pour le site StackOverFlow à partir des questions des utilisateurs. Projet constitué de 4 notebooks: récupération de données, exploration, approche non supervisée, approche supervisée.   

## Récupération des données
Récupération des données avec une requête SQL et via une API. (StackAPI) 

## Analyse exploratoire
Nettoyage des titres et corps des questions. Tokenisation, gestion des stopwords, lemmatisation, filtrage de noms avec nltk POS tagging. 
Bag Of Words: nombre d’occurrences d’un mot avec CountVectorizer, TfidfVectorizer.

## Algorithmes non supervisés
Topic modelling: modélisation de sujets avec Gensim. Visualisation avec PyLDAvis.  
Métriques utilisées: accuracy qui fournit le pourcentage de précisions correctes et d'autres métriques comme le F1 Score...

## Algorithmes supervisés
Préparation des modèles: Entrainement avec OneVsRestClassifier: stratégie qui permet de traiter les problèmes de classification multiclasse. Différents modèles sont envisagés comme LogisticRegression et SGDClassifier qui prédisent la probabilité d'un évènement binaire. Les métriques utilisées sont les mêmes que pour les algorithmes non supervisés.
SGDClassfier est le modèle qui obtient les meilleurs résultats.   
Utilisation de MLFlow pour sauvegarder les hyperparamètres, métriques, artefacts. Analyse de la stabilité sur 6 mois.

