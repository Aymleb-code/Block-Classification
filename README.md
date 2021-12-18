# Block-Classification

#### Libraries requises:
pandas
matplotlib.pyplot
seaborn
numpy
tkinter
sklearn
random


# Identification de la problématique:

Développer un modèle de prédiction permettant de détecter très efficacement les zones de textes. 



# Preprocess du dataset:

Equilibrage des différentes classes représentées dans le dataset (la classe text étant largement 
prédominante (89.8%)  ce qui pouvait grandement nuire à la performance du model)



# Data Visualisation:

Étude des corrélations 
Les variables les plus corrélées à la classe sont height, area and P_and.
Nous avons essayé de réstreindre notre futur model à ces 3 variables mais cela affectait grandement l'accuracy, montrant que les autres variables avaient tout de même leur importance.



# Choix et optimisation du model de prédiction de classes:

Test de différents modeles: KNN, RandomForest et Logistic Regression 

### KNN:

Choix du meilleur K par comparaison de leurs accuracies respectives, choix de k=4. 

Résultat: 88.03% d'accuraccy globale, 83.3% de précision dans la détection de texte


### RandomForest:

Choix du meilleur paramètre par comparaison de leurs accuracies respectives, choix de depth=7. 

Resultat: 94.72% d'accuraccy globale, 97.1% de précision dans la détection de texte

### Logistic Regression:

Resultat: 78.17% d'accuraccy globale, 72.2% de précision dans la détection de texte

Le meilleur model est donc bien évidemment le model de RandomForest qui permet d'avoir une précision 
de 97.1% pour la détéction de texte 




# API:

#### Libraries nécessaires: 
xlrd
pandas
flask
numpy
scikitlearn
pickle
matplotlib
