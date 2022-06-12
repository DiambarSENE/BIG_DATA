# Description de l’application

* Préparation des données :

	* Nous utilisons le jeu de données « Cancer du sein Coimbra » pour effectuer la classification et il peut être facilement chargé à partir du module de jeu de données avec l’API PySpark.
	* Pour combiner toutes les données d'entités et séparer les données "d'étiquettes" dans un jeu de données, nous utilisons VectorAssembler.
	* Ensuite, nous diviserons les données en parties d'entraînement et de test.
* Vérification de la prédiction et de la précision :

	* Ensuite, nous allons définir le modèle de classificateur d'arbre de décision en utilisant la classe DecisionTreeClassifier et ajuster le modèle sur les données de train. Nous pouvons prédire les données de test en utilisant la méthode trasnform ().
	* Après avoir formé le modèle, nous allons prédire les données de test et vérifier les mesures de précision. Ici, nous pouvons utiliser MulticlassClassificationEvaluator pour vérifier l'exactitude. 
	* Enfin, nous arrêterons la session de contexte Spark.
# Installations et configurations

	1. Installation de Java 1.8 ; 
	2. Installation de Spark ; 
	3. Modification des variables d’environnement ; 
	4. Vérification de la bonne exécution de Spark (spark-shell).

## Install PySpark in Anaconda & Jupyter Notebook - Spark by {Examples} (sparkbyexamples.com) 
	1. Installation de Anaconda 
	2. Création et activation d’un nouvel environnement 
	3. Installations des packages ci-dessous dans ce nouvel environnement : 
		* conda install -y -c conda-forge pyspark 
		* conda install -c conda-forge findspark 
		* conda install -y -c anaconda pandas 
	4. Ajout du nouvel environnement à jupyter notebook 
		* pip install --user ipykernel 
		* python -m ipykernel install --user --name=%EnvironmentName%



