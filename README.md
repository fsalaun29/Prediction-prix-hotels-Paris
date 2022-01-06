# Projet de Python pour l'économiste - ENSAE 2A

Florian SALAUN, Yao Pacome KOUAME, Zeena SOW

## Problématique : Quels facteurs déterminent les tarifs des hôtels parisiens ? 

## Introduction 
Dans ce projet, nous avions réellement envie de ne pas utiliser des données "toutes prêtes" et de s'essayer au webscraping. Nous avons donc naturellement pensé aux comparateurs de vols, de restaurants ou encore d'hôtels qui donnent accés à des données statistiquement et économétriquement analysables. Nous avons essayé de scraper plusieurs site et avons finnalement réussi avec booking.com, qui est un comparateur d'hôtels. 

Nous avons ensuite choisi de s'intérresser aux facteurs d'influence des tarifs des hôtels parisien uniquement, afin de restreindre le panel de critères et éviter les explications trop évidentes basées sur la ville où est situé l'hôtel. 

Notre travail est sceindé en trois grandes parties, dont voici la descrition :

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

L’objectif général de cette étude était d'analyser les facteurs déterminants des tarifs des hôtels parisiens. Pour atteindre cet objectif, nous avons scrapé les données du site booking.com concernant l'évolution des tarifs des hôtels et certaines de leurs caractéristiques. A partir de ces données, deux approches principales ont été adoptées : 
d'abord une analyse de l'evolution des prix ; ensuite, à l'aide d'une régression linéaire multiple, une modélisation du prix par les facteurs susceptibles de l'influencer.

L'analyse de l'évolution des prix nous a permis de mettre en exergue, d'une part, l'existence d'une disparité des prix entre les hôtels (certains hôtels pratiquent des prix plus élevés que d'autres), d'autre part, la présence d'un effet saisonnier sur les prix (plus élévés pendant le weekend).
Quant aux déterminants des prix, il ressort que ces derniers croissent avec le nombre d'étoiles de l'hôtel. On note par ailleurs que certaines caractéristiques telles que la richesse et la sûreté de l'arrondissement ainsi que la bonne qualité du service du personel influencent positivement les prix.
