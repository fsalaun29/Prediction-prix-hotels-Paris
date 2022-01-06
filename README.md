# Projet de Python pour l'économiste - ENSAE 2A

Florian SALAUN, Yao Pacome KOUAME, Zeena SOW

## Problématique : Quels facteurs déterminent les tarifs des hôtels parisiens ? 

## Introduction 
Dans ce projet, nous avions réellement envie de ne pas utiliser des données "toutes prêtes" et de nous essayer au webscraping. Nous avons donc naturellement pensé aux comparateurs de vols, de restaurants ou encore d'hôtels qui donnent accés à des données statistiquement et économétriquement analysables. Nous avons essayé de scraper plusieurs sites et avons finalement réussi avec Booking.com, qui est un comparateur d'hôtels. 

Nous avons ensuite choisi de nous intéresser aux facteurs d'influence des tarifs des hôtels parisiens uniquement, afin de restreindre le panel de critères et éviter les explications trop évidentes basées sur la ville où est situé l'hôtel.

Notre travail est scindé en trois grandes parties, dont voici la description :

## Partie 1 : Scraping des données à partir du site booking.com

Les notebook "Partie1" et "Partie1 bis" sont relatifs au scraping des données des hôtels parisiens sur booking.com :
"Partie1" correspond au code réellement utilisé pour obtenir les bases de données ; "Partie1 bis" en est une version réduite plus rapide à exécuter. 
** Attention : utiliser le notebook "Partie1 bis" et pas "Partie1" **

- Dans un premier temps (Partie 1.1), nous avons scrapé l'évolution des tarifs au cours du temps 
- Dans un second temps (Partie 1.2), nous avons scrapé les caractéristiques des hôtels 

Pour pouvoir exécuter le code correctement, le fichier "chromedriver.exe" (disponible dans la branche main) doit être placé dans le même répertoire que le code Python. 
Ce dernier aboutit à la création de plusieurs data-frame, regroupant un ensemble d'informations exploitables (nom de l'hôtel, prix, note moyenne des clients, détail des notes, nombre d'avis, arrondissement). Ces data-frame sont enfin sauvegardés au format xlsx et disponibles dans la branche main de ce projet. 

## Partie 2 : Analyse de l'évolution temporelle des prix

Le notebook "Partie2" est relatif à l'analyse des effets de temporalité sur les tarifs des hôtels : 
- Dans un premier temps (Partie 2.1), le jeu de données est nettoyé afin d'être exploitable 
- Dans un second temps (Partie 2.2), nous avons analysé descriptivement l'évolution des prix en fonction des hôtels
- Enfin (Partie 2.3), nous avons cherché les facteurs temporels à l'origine des fluctuations globales des prix

## Partie 3 :  Modélisation des déterminants des prix 

Le notebook "Partie3" regroupe une interrogation sur la représentativité des données utilisées dans ce projet ainsi qu'une analyse descriptive puis une modélisation : 
- Dans un premier temps (Partie 3.1) nous avons étudié la représentativité des données scrapées en les comparant à des données officielles disponibles sur statista.fr, en utilisant notamment un test du chi2
- Dans un second temps (Partie 3.2), nous avons réalisé une analyse descriptive du jeu de données
- Ensuite (Partie 3.3), nous avons construit un modèle de régression linéaire multiple afin d'analyser plus finement les effets des caractéristiques des hôtels sur leurs tarifs
- Enfin (Partie 3.4), nous avons effecté des tests sur notre modèle de régression afin d'évaluer sa pertinence et sa robustesse

## Conclusion :

L’objectif de ce projet était d'analyser les facteurs déterminants des tarifs des hôtels parisiens. Pour atteindre cet objectif, nous avons scrapé les données du site Booking.com concernant l'évolution des tarifs des hôtels et certaines de leurs caractéristiques. À partir de ces données, deux approches principales ont été adoptées : 
d'abord une analyse de l'évolution des prix sur une période d'un mois et demi ; ensuite, à l'aide d'une régression linéaire multiple, une modélisation du prix par les facteurs susceptibles de l'influencer.

L'analyse de l'évolution des prix nous a permis de mettre en exergue, d'une part, l'existence d'une disparité des prix entre les hôtels (certains hôtels, notamment les plus étoilés, affichent des prix plus élevés et qui fluctuent davantage dans le temps), et d'autre part, la présence d'un effet saisonnier sur les prix (qui sont plus élévés pendant le week-end et les périodes de fêtes). L'étude des déterminants des prix et la création d'un modèle de régression linéaire nous a permis de déceler certains facteurs qui semblent pousser les prix à la hausse, comme le fait d'avoir un grand nombre d'étoiles, de bonnes notes données par les clients ou le fait d'être dans un quartier ayant une bonne réputation. Nous avons enfin effectué quelques tests de validité de notre modèle, qui nous incitent à la prudence quant à l'interprétation des résultats qu'il fournit.
