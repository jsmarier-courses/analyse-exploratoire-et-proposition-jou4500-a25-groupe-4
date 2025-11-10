**11 Novembre 2025**<br>
**JOU4500 et Journalisme Numérique II**<br>
**Nikita Scholz, Dania Maisonneuve, Kelli-Anne Piché**<br>
**Présenté à Jean-Sébastien Marier**<br>

# Analyse exploratoire de données (AED) et proposition

## 1. Introduction

Notre but pour ce travail est d’analyser la réalité du logement selon les différents quartiers d’Ottawa. Nous tenterons de répondre à la question: est-il plus avantageux d’être propriétaire ou locataire à Ottawa selon les prix des logements?
Nous utiliserons le jeu de données collecté par Statistique Canada dans le cadre des initiatives de transparence municipale. Ce jeu de données contient plusieurs types de renseignements : les prix médians des propriétés, les loyers moyens, ainsi que d’autres informations socioéconomiques par quartier. 
L’analyse que nous tenterons de faire sera séparée en 3 étapes. La première sera de nettoyer le jeu de données pour s’assurer de garder seulement l’essentiel pour nos recherches. Ensuite, nous analyserons la position des locataires et celle des propriétaires pour comparer laquelle sont plus avantageuses pour un citoyen. La dernière étape sera alors d'interpréter les résultats pour répondre à notre question de départ.


## 2. Obtenir les données
Expliquer comment importer les données dans google feuilles de calcul
Tout d’abord, nous sommes allés dans les instructions de l’analyse exploratoire et nous avons cliqué double sur Utiliser ce fichier CSV et ensuite on a sélectionné Télécharger le fichier lié. Ensuite, après l’avoir téléchargé dans les téléchargements, nous avons été dans google feuilles de calcul et on a ouvert une nouvelle feuille de calcul. Par la suite, on a sélectionné l’option Fichier et ensuite Importer. On est allé dans téléverser et on a glissé le téléchargement des données. Finalement, nous avons pesé sur l'importation des données. 

Inclure une capture d’écran de votre jeu de données dans google après l’importation
faut voir les titres de colonnes (première ligne) et les 20 à 30 lignes dessous. (Et n'oubliez pas de mettre l'image dans le même dossier que vos fichiers .md.)
![alt text](<Capture d'ecran.png>)

Veuillez inclure un lien public vers votre document Google Feuilles de calcul.
https://docs.google.com/spreadsheets/d/1lzWKCiK3wRbvcReweSwHE6eMn_tIX7ZD1PHe1a8lKak/edit?usp=sharing 


Faites des observations générales concernant le jeu de données :

Dans le jeu de données, il y a 26 colonnes et 2503 lignes. À première vue, les données n’étaient pas propres et n’étaient pas très bien organisées. Nous avons aussi remarqué qu’il y beaucoup de données qui nous étaient peu utiles ou même absentes. Ensuite, notre équipe à fait comme observation qu’il y a beaucoup de données quant aux âges, aux langues, aux immigrants, aux types de voitures, des types de logements et aux types de revenus. Finalement, nous avons aussi remarqué et on a été très déçu du fait qu’il n'y a pas de données par rapport au Québec, tandis que le texte discutait de la relation entre travailler en Ontario et habiter au Québec et vis versa.

 Dans notre jeu de données, nous avons affaire avec différents types de variables. Tout d’abord, dans notre jeu de donnés utile pour notre histoire, les frais de logement de la colonne A (1-5) représentent des variables quantitatives continues. Ensuite,  les % des ménages propriétaires ou locataires, de la colonne A (7-8) représentent aussi des variables continues. Pour ajouter, le restant de nos données ce sont aussi des variables quantitatives continues. Les titres des colonnes B à Z sont plutôt des variables qualitatives nominales.

Formulez au moins une question ou une hypothèse qui vous vient à l’esprit lorsque vous examinez les données brutes.

Est-ce que ça vaut plus la peine d'être locataire plutôt que propriétaire dans la ville d’ottawa?



Utilisez deux croisillons (`##`) pour créer un intertitre de niveau 2 comme celui-ci.

**Voici quelques exemples de fonctions et de lignes de code mises dans des boîtes grises :**

1. Si vous nommez une fonction, mettez là à l'intérieur de guillemets « inclinés » comme ceci : `IMPORTHTML`.
1. Si vous voulez inclure une ligne de code complète, faites la même chose, mais avec tout le code : `=IMPORTHTML("https://en.wikipedia.org/wiki/China"; "table", 5)`.
1. Alternativement, vous pouvez mettre le code dans une boîte indépendante en utilisant le modèle de code ci-dessous :

``` r
=IMPORTHTML("https://en.wikipedia.org/wiki/China"; "table", 5)
```
C'est aussi comme ça qu'on crée une liste ordonnée. Il suffit de mettre `1.` devant chaque item.

## 3. Comprendre les données

### 3.1. Analyse VIMA

Nous avons réalisé notre analyse VIMA sur les données des lignes 757, 759, 760, 761, 762, 765, 767, 768 ainsi que les lignes 1951 à 1956. De façon générale, il s’agit des données que nous pensons qui pourraient nous être utiles dans nos recherches. 

Avant même d’avoir recours à diverses méthodes pour analyser nos données, nous avons remarqué quelques détails. 

Plusieurs données présentaient des erreurs de formatage. À titre d’exemple, les valeurs dans la colonne 757 n'étaient pas formatées de la même façon. Certaines de ces données étaient des chiffres alors que d’autres étaient en fait des dates. De plus, nous avons remarqué que les colonnes M et N présentaient souvent des erreurs de formatage majeures, qui rendaient parfois les valeurs aberrantes et, ainsi, invalides. Par exemple, toujours dans la ligne 757 qui est censée afficher un pourcentage, la valeur de la cellule à la colonne M affiche le chiffre 45 994. Comparativement aux autres données qui ensemble font une moyenne de 10,15%, la valeur de 45 000% ressort du lot et est impossible dans ce contexte.

Une fois les données nettoyées et ces détails réglés, nous avons eu la chance de procéder à des méthodes plus poussées pour faire notre analyse VIMA détaillée. 

À premier coup d'œil, les données des lignes que nous avons ciblées semblent toutes être valides. Il n’y a pas de données manquantes, et il ne semble pas y avoir de données invalides ou aberrantes.

Afin de confirmer ce constat, nous avons produit un premier graphique à l’aide des données des colonnes 7 et 8 de notre nouveau tableau nettoyé. Ce graphique, ci-dessous, nous a permis de confirmer qu’il n’a évidemment pas de valeur aberrante. De plus, il n’y a pas de valeurs invalides qui furent soulevées. 

Ensuite, afin de vérifier l’exactitude des données, nous avons procédé à divers calculs afin de voir si les chiffres de l’ensemble des quartiers coordonnaient avec les données pour l’ensemble de la Ville d’Ottawa. Nos résultats furent assez intéressants. La plupart des sommes, des moyennes ou des médianes de l’ensemble des quartiers ne correspondent pas aux données pour l’ensemble de la Ville d’Ottawa, mais la différence est parfois minime. 

Autrement, les données semblent valides et exactes. 

______________________________________________________________________
______________________________________________________________________

Utilisez trois croisillons (`###`) pour créer un intertitre de niveau 3 comme celui-ci. Je vous prie de suivre ce modèle en ce qui a trait aux intertitres de niveaux 1 et 2. Toutefois, je vous laisse le loisir d'utiliser les intertitres de niveau 3 comme bon vous semble.

Insérez votre texte ici.

Appuyez vos affirmations en citant les sources appropriées. Veuillez suivre les [normes APA en matière d'attribution dans le corps du texte](https://apastyle.apa.org/style-grammar-guidelines/citations).

**Par exemple :**

Comme l'affirme Cairo (2016), une visualisation de données doit être véridique...

### 3.2. Nettoyage des données

Insérez votre texte ici.

### 3.3. Analyse exploratoire des données (AED)

Nous avons concentré notre analyse exploratoire sur les deux variables suivantes : 
* % de ménages locataires consacrant 30% ou plus de leur revenu aux frais de logement
* % de ménages propriétaires consacrant 30% ou plus de leur revenu au frais de logement

À notre avis, il s’agit des meilleures variables pour nous aider à comprendre s’il est plus plus avantageux d’être propriétaire ou locataire à Ottawa. C’est une chose que les prix des logements soient élevés ou non, mais il en est tout autre si les individus doivent dépenser plus de 30% de leur salaire en frais de logement, ce qui leur laisse moins d’argent pour d’autres dépenses essentielles. 

Le fil conducteur de notre récit nous est apparu comme une évidence. Dès notre analyse VIMA, nous avons remarqué la différence marquante entre les locataires qui dépensent plus de 30% de leur revenu en frais de logement et les propriétaires, et ce, dans chaque quartier (AED - Graphique 1). Ces statistiques ont suscité en nous plusieurs questions. Nous tenterons donc de mieux comprendre ce phénomène lors de notre récit. 

![alt text](<AED - Graphique 1.png>)

Nous nous sommes donc servis de cette analyse exploratoire pour essayer de mieux comprendre la situation au sein de chaque quartier afin de nous guider dans nos recherches. Pour y arriver, nous avons modifié notre tableau nettoyé afin de pouvoir y réaliser de nouvelles opérations, comme des filtres (voir la capture d’écran ci-dessous). L’usage d’un tableau croisé ne semblait pas pertinent avec nos types de données. 

![alt text](<AED - Jeu de données modifié.png>)

Nous avons d’abord utilisé la formule suivante afin de connaître la différence exacte entre les ménages propriétaires et locataires au sein de chaque quartier. 

```
=H_-G_
```

À l’aide de l’outil filtre, nous avons été en mesure de déterminer les 5 quartiers où les différences sont les plus grandes : 
1. Quartier 4 - Kanata-Nord (34,70)
1. Quartier 6 - Stittsville (29,80)
1. Quartier 1 - Orléans Est-Cumberland (29,40)
1. Quartier 20 - Osgoode (28)
1. Quartier 2 - Orléans-Ouest-Innes (27,80)

Nous avons également filtré les colonnes G et H afin de connaître les quartiers où les locataires et les propriétaires sont plus nombreux à dépenser 30% de leur revenu en frais de logement. Les résultats que nous avons obtenus sont les suivants : 

Locataires dépensant plus de 30% de leur revenu aux frais de logement
1. Quartier 4 - Kanata-Nord
1. Quartier 6 - Stitsville
1. Quartier 1 - Orléans Est-Cumberland
1. Quartier 12 - Rideau-Vanier
1. Quartier 17 - Capitale

Propriétaires dépensant plus de 30% de leur revenu aux frais de logement
1. Quartier 12 - Rideau-Vanier
1. Quartier 14 - Somerset
1. Quarter 13 - Rideau-Rockcliffe
1. Quartier 10 - Gloucester-Southgate
1. Quartier 22 - Riverside Sud-Findlay Creek

De plus, afin de voir la relation entre les propriétaires et les locataires dépensant plus de 30% de leur revenu en frais de logement au sein d’un même quartier, nous avons produit les graphiques circulaires ci-dessous (AED - Graphique 2). Cependant, ces statistiques font ressortir les mêmes quartiers vus plus haut, seulement dans des ordres différents.

![alt text](<AED - Graphique 2.png>)

Une fois ces statistiques obtenues, nous avons produit la map suivante (AED - Map) afin de voir si la dimension géographique pouvait révéler quelque chose.

Celui-ci semble indiquer que les plus grandes différences entre les locataires dépensant plus de 30% de leur revenu en frais de logement et les propriétaires ont principalement lieu dans les extrémités est et ouest de la ville. Bref, un autre angle intéressant sur lequel on pourra se tourner.

C’est ce qui conclut notre analyse exploratoire. De toute évidence, une analyse plus poussée des données afin de voir si d’autres variables, comme le revenu d’emploi moyen ou le pourcentage de gens travaillant à temps plein ou à temps partiel, pourrait expliquer cette différence. 

______________________________________________________________________
______________________________________________________________________
## 4. Récit potentiel

Les articles suivants vont nous permettre de comprendre la situation des logements au Canada mais plus spécifiquement à Ottawa. Afin de vraiment raconter une histoire et bien comprendre nos données, on doit comprendre la situation de logement afin d'avoir des informations précises sur plusieurs aspects qui peuvent influencer les choix des locataires ou propriétaires. Nous avons trouvé principalement des articles de journaux et des articles sur des sites de logements. Dans notre cas, ce sont des sources assez pertinentes, car elles viennent de journalistes et de professionnels dans le domaine du logement. Pour notre projet, nous examinons s’il est plus avantageux d’être propriétaire ou locataire à Ottawa selon les prix des logements, donc toutes ces sources seront des informations qui vont nous permettre de bâtir une conclusion concise et bien soutenue.  

Desjardins, S. (2025, February 11). Louer ou acheter: devenir propriétaire n’est pas un choix logique. Le Journal De Montréal. https://www.journaldemontreal.com/2025/02/09/louer-ou-acheter-devenir-proprietaire-nest-pas-un-choix-logique 

Du Canada Statistique Canada, G. (2021, September 2). Les statistiques : le pouvoir des données! https://www150.statcan.gc.ca/n1/edu/power-pouvoir/toc-tdm/5214718-fra.htm 

Eads, D. (2016, October 15). How to “interview” a big pile of data. NPR. https://www.npr.org/sections/npr-training/2025/05/29/g-s1-67278/how-to-interview-a-big-pile-of-data 

Info, R. (2025, February 25). Élections en Ontario : la crise du logement vue par les candidats de la région d’Ottawa. Radio-Canada. https://ici.radio-canada.ca/nouvelle/2143463/logement-ontario-ottawa-crise-election   

Malone, K. (2025, April 15). Are Ottawa condos a good investment in 2025? Here’s what you need to know — Matt Richling - Ottawa Condos and Lofts - Ottawa Real estate for sale. Matt Richling - Ottawa Condos and Lofts - Ottawa Real Estate for Sale. https://www.mattrichling.com/blog/are-ottawa-condos-a-good-investment-in-2025-heres-what-you-need-to-know 

Ottawa, J. P.-. R. I. K., & Polonski. (2023, November 14). Meet Jason Polonski – Kanata & Ottawa’s trusted real estate agent. Jason Polonski- Realtor in Kanata, Ottawa. https://ottawarealtyman.com/renting-vs-buying-in-ottawa/?srsltid=AfmBOopRTPe0wguJu-6BidNu77JeIqpCF0Rhsw_c5KqrPSvv65isi5a4 

https://www.cpacanada.ca/fr/nouvelles/analyse/acheter-louer 


De quoi avez-vous besoin pour raconter cette histoire?

Afin que notre analyse soit complète et solide, nous avons quelques aspects à explorer;
Témoignage de citoyens
Nous pourrions aller chercher des témoignages pour avoir des expériences vécues de locataires et propriétaires. Avoir des témoignages de différents quartiers pourrait aussi nous aider à comparer les écarts de réalités.
Politiques locales
Qu’est-ce que la ville fait pour aider ses citoyens? Quelles sont les mesures mises en place? Nous pourrions aussi creuser davantage dans les règlements de zonage ou même de projet récent, comme la densification près des stations O-Train.
Visualisation des données
Pour mieux comprendre notre analyse, nous allons créer des cartes interactives des prix médians et des loyers moyens, des graphiques qui vont comparer l’évolution du coût du logement et le revenu médian. De plus, nous allons pouvoir utiliser le graphique split bar pour voir clairement les différences entre locataire et propriétaire.


Qui pourriez-vous interviewer à ce sujet?

Nous pourrions interview:
Citoyens 
Des locataires et propriétaire dans différents secteurs d’Ottawa
Agent de terrain
Des courtiers immobiliers ou gestionnaire d’immeubles pour discuter du marché
Experts ou chercheur
Professeur en urbanisme à l’université d’Ottawa: Carolyn Whitzman
Analystes de la SCHL: encore à trouver…


## 5. Conclusion

Insérez votre texte ici.

## 6. Références

Veuillez inclure une liste de vos références ici. Assurez-vous de suivre les [normes APA pour les références](https://apastyle.apa.org/style-grammar-guidelines/references). Les retraits négatifs (*hanging paragraphs*) ne sont pas nécessaires. Le [guide sur l'adaptation APA](https://arts.uottawa.ca/lettres/sites/arts.uottawa.ca.lettres/files/cartu-outils-de-redaction-adaptation-apa.pdf) de l'Université d'Ottawa pourrait également vous être utile.

**Voici un exemple :**

Bounegru, L., & Gray, J. (Eds.). (2021). *The Data Journalism Handbook 2: Towards A Critical Data Practice*. Amsterdam University Press. [https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153](https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153)
