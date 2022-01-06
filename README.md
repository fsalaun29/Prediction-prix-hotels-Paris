# Projet de Python pour l'économiste - ENSAE 2A

Florian SALAUN, Yao Pacome KOUAME, Zeena SOW

## Problématique : Quels facteurs déterminent les tarifs des hôtels parisiens ? 

## Introduction 
...

## Partie 1 : Scraping des données à partir du site booking.com

Les notebook "Partie1" et "Partie1 bis" sont relatifs au scraping des données des hôtels parisiens sur booking.com :
"Partie1" correspond au code réellement utilisé pour obtenir les bases de données ; "Partie1 bis" en est une version réduite plus rapide à exécuter. 
- Dans un premier temps (Partie 1.1), nous avons scrapé l'évolution des tarifs au cours du temps 
- Dans un second temps (Partie 1.2), nous avons scrapé les caractéristiques des hôtels 

Pour pouvoir être exécuté correctement, le fichier "chromedriver.exe" (disponible dans la branche main) doit être placé dans le même répertoire que le code Python. 
Ce dernier aboutit à la création de plusieurs data-frame, regroupant un ensemble d'informations exploitables (nom de l'hôtel, prix, note moyenne des clients, détail des notes, nombre d'avis, arrondissement). Ces data-frame sont enfin sauvegardés au format xlsx et disponibles dans la branche main de ce projet. 

## Partie 2 : Analyse de l'évolution temporelle des prix

Le notebook "Partie2.ipynb" est relatif à l'analyse des effets de temporalité sur les tarifs des hôtels : 
- Dans un premier temps (Partie 2.1), le jeu de données est nettoyé afin d'être exploitable 
- Dans un second temps (Partie 2.2), nous avons analysé descriptivement l'évolution des prix en fonction des hôtels
- Enfin (Partie 2.3), nous avons cherché les facteurs temporels à l'origine des fluctuations globales des prix

## Partie 3 :  Modélisation des déterminants des prix 

Le notebook "Partie3.ipynb" regroupe une interrogation sur la représentativité des données utilisées dans ce projet ainsi qu'une analyse descriptive puis une modélisation : 
- Dans un premier temps (Partie 3.1) nous avons étudié la représentativité des données scrapées en les comparant à des données officielles disponibles sur statista.fr, en utilisant notamment un test du chi2
- Dans un second temps (Partie 3.2), nous avons réalisé une analyse descriptive du jeu de données
- Ensuite (Partie 3.3), nous avons construit un modèle de régression linéaire multiple afin d'analyser plus finement les effets des caractéristiques des hôtels sur leurs tarifs
- Enfin (Partie 3.4), nous effectuons des tests sur notre modèle de régression afin d'évaluer sa pertinence et sa robustesse.

## Conclusion : 
...
