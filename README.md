# À l'Assaut du Monde Professionnel : Embarquez pour l'Aventure avec Nous !
# Analyse de l'insertion professionnelle des diplômés de l'enseignement supérieur en France : Tendances, disparités et perspectives
# Table des matières

- [Introduction](#introduction)
- [Collecte et filtrage des Données](#collecte-et-filtrage-des-données)
- [Analyse Comparative du Taux d'Insertion Professionnelle Selon les Domaines d'Études](#analyse-comparative-du-taux-dinsertion-professionnelle-selon-les-domaines-détudes)
- [Comparaison des Salaires Médians Annuels Estimés par Discipline](#comparaison-des-salaires-médians-annuels-estimés-par-discipline)
- [Comparer les Salaires Médians par Genre](#comparer-les-salaires-médians-par-genre)
- [Analyse Temporelle du Taux de Chômage National par Domaine d'Études](#analyse-temporelle-du-taux-de-chômage-national-par-domaine-détudes)
- [Analyse de la Répartition des Opportunités Professionnelles](#analyse-de-la-répartition-des-opportunités-professionnelles)

# Introduction : 
  Dans le paysage éducatif contemporain, l'obtention d'un diplôme de master est souvent perçue comme une étape cruciale dans le cheminement académique, ouvrant les portes à des opportunités professionnelles diverses. Toutefois, le succès de cette transition du monde académique au marché du travail demeure une préoccupation pour les nouveaux diplômés. Ce projet de datavisualisation s'attache à explorer et à analyser l'insertion professionnelle des diplômés de master des universités françaises.

!["Passage vers l'avenir réussi."](https://alumni.ut-capitole.fr/medias/image/16329001225db15e48bfa0f.jpg)

La question de l'insertion professionnelle va au-delà des simples statistiques d'emploi. Elle englobe la diversité des parcours professionnels, les secteurs d'activité privilégiés, les rémunérations, et les défis rencontrés par les diplômés. En examinant de près ces aspects, nous aspirons à apporter une compréhension approfondie des dynamiques de l'emploi post-master, fournissant ainsi des informations cruciales pour les étudiants, les universités, et les acteurs du marché du travail.

À travers une datavisualisation, nous visons à mettre en lumière les tendances, les disparités et les opportunités qui émergent de l'analyse des données sur l'insertion professionnelle. Cette exploration ne se contente pas de quantifier les résultats, mais vise également à susciter des réflexions sur les politiques éducatives, les programmes de formation, et les perspectives d'amélioration pour optimiser l'alignement entre l'éducation supérieure et les besoins du marché du travail.

En nous plongeant dans l'univers des diplômés de master en France, cette datavisualisation aspire à être un outil informatif et révélateur, contribuant ainsi à la discussion continue sur l'efficacité des programmes de master et à la préparation des étudiants aux défis de la vie professionnelle.

# Collecte et filtrage des données : 

Le jeu de données que nous avons selectionné provient du site https://data.enseignementsup-recherche.gouv.fr/pages/home qui est la plateforme de données ouvertes du ministère de l'Enseignement supérieur, de la Recherche et de l'Innovation en France. Cette plateforme fournit un accès à un large éventail de données relatives à l'enseignement supérieur, à la recherche et à l'innovation. Le jeu de données selectionné contient des informations sur l'insertion professionnelle des diplômés de niveau Master en France. Les informations incluses dans le fichier couvrent divers aspects tels que l'année, le type de diplôme, la situation (18 ou 30 mois après le diplôme), le genre, les disciplines d'étude, les indicateurs d'insertion professionnelle tels que les taux d'insertion, les taux d'emploi, les salaires médians, etc.

Afin de garantir la qualité et la fiabilité de nos données, nous avons fait le choix d'utiliser OpenRefine, un outil puissant qui nous a permis d'effectuer des opérations de nettoyage, d'enrichissement et de transformation avec une grande précision.
Nous avons réalisé un processus de filtrage des données à l'aide d'OpenRefine, en mettant en œuvre plusieurs étapes visant à améliorer la qualité et l'utilité de nos données. En premier lieu, nous avons éliminé les colonnes superflues telles que "Salaire net mensuel national 3ème quartile" et "Salaire net mensuel national 1er quartile" qui ne contribuaient pas à notre analyse. Ensuite, pour assurer une meilleure clarté, nous avons renommé la colonne "% emplois extérieurs à la région de l’université" en "pourcentage emplois extérieurs à la région de l’université".

Dans le souci d'éliminer les données inutiles et d'alléger notre jeu, nous avons entrepris des modifications significatives avec OpenRefine. Pour garantir la cohérence des informations, nous avons supprimé les lignes présentant des valeurs vides ou égales à "0" dans la colonne "Taux d’insertion". Nous avons également remplacé les occurrences de "ns" par "0" dans plusieurs colonnes, notamment "Taux d’insertion", "Part des emplois de niveau cadre", "pourcentage emplois extérieurs à la région de l’université", "Part des emplois à temps plein", et "Salaire brut annuel estimé". Ces ajustements ont non seulement éliminé toute ambiguïté, mais aussi amélioré considérablement la qualité de nos données en préparation d'une analyse approfondie, étant donné que les informations manquantes dans les lignes ne sont pas disponibles ailleurs.

Voici le lien vers l'historique des changements apportés au jeu de données : 

[Historique des changements](https://raw.githubusercontent.com/Bouaziz-Souhila/Data_Visualisation_2024/main/history%20(2).json)

Voici le résultat de notre jeu de donnés après l'orération de filtrage : 

<iframe title="[ Insertion Professionnelle des diplômés de Master en France : ]" aria-label="Table" id="datawrapper-chart-rDYbw" src="https://datawrapper.dwcdn.net/rDYbw/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="1173" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r=0;r<e.length;r++)if(e[r].contentWindow===a.source){var i=a.data["datawrapper-height"][t]+"px";e[r].style.height=i}}}))}();</script>

# Analyse Comparative du Taux d'Insertion Professionnelle Selon les Domaines d'Études :
Afin d'illustrer la répartition des diplômés par dicsipline d'études et de mettre en évidence la proportion de diplômés dans chaque discipline, nous avons choisi d'utiliser un diagramme circulaire. Cette approche nous permettra de visualiser de manière succincte et esthétique la répartition globale des diplômés au sein des différentes disciplines académiques.

Le choix du diagramme circulaire repose sur notre intention de créer une représentation visuelle claire de la distribution des diplômés au fil du temps. En attribuant à chaque secteur académique une portion du cercle en fonction de sa part relative, nous faciliterons la perception immédiate des proportions et des tendances majeures. Cette visualisation se révèle particulièrement efficace pour communiquer la diversité des domaines d'études parmi les diplômés, offrant ainsi une perspective globale des orientations académiques.

<iframe src='https://flo.uri.sh/visualisation/16601595/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:900px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/16601595/?utm_source=embed&utm_campaign=visualisation/16601595' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>



# Comparaison des Salaires Médians Annuels Estimés par Discipline  :
Pour examiner de près l'évolution du salaire annuel de 2015 à 2020, nous avons créé un diagramme en lignes. Cette représentation graphique permet une analyse chronologique des variations du salaire estimé au fil du temps, offrant ainsi un aperçu succinct mais précis de la situation sur cette période.

!["titre"](https://raw.githubusercontent.com/Bouaziz-Souhila/Data_Visualisation_2024/main/SALAIREparannee.svg)

Ensuite, nous avons voulu comparer les salaires médians des diplômés en fonction de leur discipline d'études, nous avons opté pour l'utilisation d'un diagramme en barres. Cette approche va nous permettre de visualiser de manière efficace les différences de rémunération entre les différents groupes.

Notre objectif premier avec cette datavisualisation est d'offrir une compréhension visuelle immédiate des écarts salariaux, favorisant ainsi une réflexion approfondie sur les aspects liés à l'équité et à la diversité au sein des parcours professionnels post-diplôme. Le diagramme en barres se présente ainsi comme un outil graphique puissant pour illustrer et communiquer de manière concise ces différences salariales significatives.

<iframe src='https://flo.uri.sh/visualisation/16601641/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/16601641/?utm_source=embed&utm_campaign=visualisation/16601641' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

# Comparer les Salaires Médians par Genre : 

Pour comparer les salaires médians des diplômés en fonction de leur genre et mettre en évidence les différences de rémunération entre les femmes et les hommes au fil des années, nous avons choisi de créer un diagramme en lignes. Cette approche de datavisualisation permet une comparaison claire et directe des salaires médians par genre, organisée par année. En utilisant ce format, notre objectif est de fournir une perspective temporelle sur les tendances salariales, mettant en lumière les variations significatives dans les parcours professionnels post-diplôme sans se focaliser sur des domaines d'études spécifiques.
!["Titre"](https://raw.githubusercontent.com/Bouaziz-Souhila/Data_Visualisation_2024/main/SALAIREparanneeETGENRE.svg)


# Analyse Temporelle du Taux de Chômage National par Domaine d'Études et par Genre: 

Nous avons choisi d'utiliser un diagramme en lignes pour représenter le taux de chômage dans différents domaines d'études au fil du temps. Chaque ligne illustre le taux de chômage, permettant une comparaison directe entre les domaines. Cette visualisation offre une perspective détaillée du chômage dans chaque secteur, avec des couleurs distinctes pour faciliter la distinction. L'analyse de cette représentation graphique permettra d'évaluer les variations du taux de chômage et d'identifier les domaines nécessitant d'éventuels ajustements pour favoriser l'égalité professionnelle.
!["titre"](https://raw.githubusercontent.com/Bouaziz-Souhila/Data_Visualisation_2024/main/Salaire_par_domaine.svg)

Ensuite, nous avons aussi chsoisi une autre visualisation dite, hiérarchique (Hierarchy), pour représenter le taux de chômage en fonction du genre. Cette approche de datavisualisation, basée sur un modèle de regroupement des données et de représentation hiérarchique, offre une perspective structurée du taux de chômage. 
Pour utiliser cette template, vous pouvez sélectionner le taux de chômage dans le menu déroulant, puis cliquer sur les cercles pour afficher d'éventuelles informations.

<iframe src='https://flo.uri.sh/visualisation/16606237/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/16606237/?utm_source=embed&utm_campaign=visualisation/16606237' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

# Analyse de la Répartition des Opportunités Professionnelles : Diagramme de Voronoï selon les Domaines d'Étude et les Emplacements Géographiques 
Nous avons choisi de mettre en œuvre un Diagramme de Voronoï pour analyser la répartition du pourcentage d'emplois externes à la région de l'université, en tenant compte également de la répartition selon le domaine d'étude. Ce type de diagramme offre une représentation graphique distincte en divisant l'espace en zones délimitées, chacune correspondant à une zone géographique spécifique. Dans ce contexte, les zones représentent non seulement les emplacements géographiques des emplois, mais aussi les domaines d'étude associés. Ainsi, cette visualisation permet d'observer de manière claire et détaillée comment les opportunités professionnelles sont réparties spatialement en fonction des différents domaines d'étude, offrant une perspective approfondie sur la dynamique de l'emploi dans cette région universitaire particulière.

!["titre"](https://raw.githubusercontent.com/Bouaziz-Souhila/Data_Visualisation_2024/main/viz_en_dehors_region_univ%20(1).svg)

Ensuite nous avons aussi une autre visualisation qui montre le prourcentage d'insertion extérieur à la région de l'université filtré par domaine d'étude et par année.

<iframe src='https://flo.uri.sh/visualisation/16641350/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/16641350/?utm_source=embed&utm_campaign=visualisation/16641350' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

