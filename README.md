# Data_Visualisation_2024
# Projet de Visualisation de Données sur l'insertion proffessionnelle des diplomés de Master en France 
Le jeu de données que nous avons selectionné contient des informations sur l'insertion professionnelle des diplômés de niveau Master en France. Les informations incluses dans le fichier couvrent divers aspects tels que l'année, le type de diplôme, la situation (18 ou 30 mois après le diplôme), le genre, les disciplines d'étude, les indicateurs d'insertion professionnelle tels que les taux d'insertion, les taux d'emploi, les salaires médians, etc.
En ce qui concerne les colonnes vides, il semble y avoir des cellules vides dans le jeu de données. Par exemple, certaines lignes contiennent des valeurs manquantes pour des indicateurs tels que le salaire net mensuel médian, le taux de chômage national, etc. Ces cellules vides devront être prises en compte lors du nettoyage et de la préparation des données pour une analyse ou une visualisation ultérieure.
# présentation des informations présentées dans le jeu de données : 
Le fichier fr-esr-insertion_professionnelle-master.csv contient les champs de données suivants :
Année : L'année à laquelle les données d'insertion professionnelle se rapportent.
Diplôme : Le type de diplôme obtenu (Master LMD, etc.).
Situation : Le statut des diplômés (18 mois après le diplôme, 30 mois après le diplôme, etc.).
Genre : Le genre des diplômés (femmes, hommes, ou les deux).
Domaine d'étude : Le domaine d'étude des diplômés.
Code du domaine : Le code du domaine d'étude.
Discipline : La discipline d'étude des diplômés.
Code de la discipline : Le code de la discipline d'étude.
Nombre de diplômés : Le nombre de diplômés pour chaque catégorie.
Taux d'insertion : Le taux d'insertion professionnelle des diplômés.
Taux d'emploi : Le taux d'emploi des diplômés.
Taux d'emploi salarié en France : Le taux d'emploi salarié en France des diplômés.
Pourcentage d'emplois cadre ou professions intermédiaires : Le pourcentage d'emplois cadre ou professions intermédiaires des diplômés.
Pourcentage d'emplois stables : Le pourcentage d'emplois stables des diplômés.
Pourcentage d'emplois à temps plein : Le pourcentage d'emplois à temps plein des diplômés.
Salaire net médian des emplois à temps plein : Le salaire net médian des emplois à temps plein des diplômés.
Salaire brut annuel estimé : Le salaire brut annuel estimé des diplômés.
Pourcentage de diplômés boursiers : Le pourcentage de diplômés boursiers parmi les diplômés.
Taux de chômage régional : Le taux de chômage régional des diplômés.
Salaire net mensuel médian régional : Le salaire net mensuel médian régional des diplômés.
Il semble y avoir des colonnes vides dans le jeu de données, comme indiqué par la présence de plusieurs points-virgules consécutifs dans les extraits de données fournis. Ces colonnes vides devront être prises en compte lors du nettoyage et de la préparation des données pour une analyse ou une visualisation ultérieure.


# Pour remplir les informations manquantes dans ce jeu de données, vous pouvez envisager les approches suivantes :
# Imputation par la moyenne ou la médiane : 
Pour les variables numériques telles que les salaires, vous pouvez remplir les valeurs manquantes en utilisant la moyenne ou la médiane des salaires pour la catégorie correspondante (par exemple, le domaine d'étude, le genre, etc.).
# Imputation par la valeur la plus fréquente : 
Pour les variables catégorielles, vous pouvez remplir les valeurs manquantes avec la catégorie la plus fréquente dans le jeu de données.
# Utilisation de modèles de prédiction : 
Si les données manquantes représentent une proportion importante du jeu de données, vous pouvez envisager de construire des modèles de prédiction pour estimer les valeurs manquantes en fonction des autres variables disponibles.
# Suppression des lignes ou des colonnes : 
Si les données manquantes sont très répandues et ne peuvent pas être estimées avec précision, vous pouvez envisager de supprimer les lignes ou les colonnes concernées.
Avant d'appliquer l'une de ces méthodes, il est important de comprendre le contexte des données et d'évaluer l'impact potentiel de l'imputation sur toute analyse ou interprétation ultérieure. De plus, il est recommandé de documenter clairement toute méthode d'imputation utilisée dans le cadre d'une analyse de données.
