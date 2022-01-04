# Projet de Python pour l'économiste - ENSAE 2A

Florian SALAUN, Yao Pacome KOUAME, Zeena SOW

## Problématique : Quels facteurs déterminent les tarifs des hôtels parisiens ? 

## Partie 1 : Scraping des données à partir du site Booking.com

Le notebook "Partie 1.ipynb" est relatif au scraping des données des hôtels parisiens sur Booking.com : 
- Dans un premier temps (Partie 1.1) nous avons scrapé l'évolution des tarifs au cours du temps 
- Dans un second temps (Partie 1.2) nous avons scrapé les caractéristiques des hôtels 

Pour pouvoir être exécuté correctement, le fichier "chromedriver.exe" (disponible dans la branche main) doit être placé dans le même répertoire que le code Python. 
Ce dernier aboutit à la création de plusieurs data-frame, regroupant un ensemble d'informations exploitables (nom de l'hôtel, prix, note moyenne des clients, détail des notes, nombre d'avis, arrondissement). Ces data-frame sont enfin sauvegardés au format xlsx et disponibles dans la branche main de ce projet. 

## Partie 2 : Analyse de l'évolution temporelle des prix

Le notebook "Partie 2.ipynb" est relatif à l'analyse des effets de temporalité sur les tarifs des hôtels : 
- Dans un premier temps (Partie 2.1) le jeu de données est nettoyé afin d'être exploitable 
- Dans un second temps (Partie 2.2) nous avons analysé descriptivement l'évolution des prix en fonction des hôtels
- Enfin (Partie 2.3) nous avons cherché les facteurs temporels à l'origine des fluctuations de prix

## Partie 3 :  Modélisation des déterminants des prix 

Le notebook "Partie 3.ipynb" regroupe une interrogation sur la représentativité des données utilisées dans ce projet ainsi qu'une analyse descriptive puis une modélisation : 
- Dans un premier temps (Partie 3.1) nous avons étudié la représentativité des données scrapées en les comparant à des données officielles disponibles sur statista.fr, en utilisant nottament un test du chi2
- Ensuite (Partie 3.2) nous avons réalisé une analyse descriptive du jeu de données
- Enfin (Partie 3.3) nous avons construit un modèle de régréssion afin d'analyser plus finnement les effets des caractéristiques des hôtels sur leurs tarifs 


