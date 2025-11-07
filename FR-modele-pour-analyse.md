**Date**<br>
**Cote et nom du cours**<br>
**Prénom et nom de l'étudiant(e)**<br>
**Présenté à Jean-Sébastien Marier**<br>

# Analyse exploratoire de données (AED) et proposition

Utilisez un croisillon (`#`) pour créer un intertitre de niveau 1 comme celui-ci.

## Avant-propos

Pour ce travail, vous devez extraire des données d’un site Internet ou d’une base de données. Vous devez ensuite nettoyer et analyser votre jeu de données, trouver une histoire potentielle et créer une visualisation. Votre travail doit clairement expliquer votre processus. Vous devez écrire environ 1500 à 2000 mots et inclure des captures d’écran montrant les différentes étapes de votre analyse. Votre travail doit être rédigé avec le format Markdown et être publié sur GitHub.

J'assigne différentes versions de ce projet à mes étudiants en journalisme numérique et en « data storytelling » depuis déjà quelques années. La structure générale de ce travail est basée sur celle du [*Guide du datajournalisme*](http://jplusplus.github.io/guide-du-datajournalisme/index.html). La présente version est également inspirée du programme [Key Capabilities in Data Science](https://extendedlearning.ubc.ca/programs/key-capabilities-data-science) offert par l'Université de la Colombie-Britannique (UBC).

**Voici quelques ressources utiles pour ce travail :**

* [Page *Syntaxe de base pour l’écriture et la mise en forme* de GitHub](https://docs.github.com/fr/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
* [Le répertoire modèle pour ce projet au cas où vous effaceriez quelque chose par accident](https://github.com/jsmarier/jou4100_jou4500_mpad2003_project2_template)

Avez-vous remarqué comment créer un hyperlien? En langage Markdown, on met le texte cliquable entre une paire de crochets et l'adresse URL entre parenthèses.

Pour créer une liste non ordonnée, il suffit de mettre une étoile (`*`) devant chaque item.

## 1. Introduction

Insérez votre texte ici.

## 2. Obtenir les données
Expliquer comment importer les données dans google feuilles de calcul
Tout d’abord, nous sommes allés dans les instructions de l’analyse exploratoire et nous avons cliqué double sur Utiliser ce fichier CSV et ensuite on a sélectionné Télécharger le fichier lié. Ensuite, après l’avoir téléchargé dans les téléchargements, nous avons été dans google feuilles de calcul et on a ouvert une nouvelle feuille de calcul. Par la suite, on a sélectionné l’option Fichier et ensuite Importer. On est allé dans téléverser et on a glissé le téléchargement des données. Finalement, nous avons pesé sur l'importation des données. 

Inclure une capture d’écran de votre jeu de données dans google après l’importation
faut voir les titres de colonnes (première ligne) et les 20 à 30 lignes dessous. (Et n'oubliez pas de mettre l'image dans le même dossier que vos fichiers .md.)

Veuillez inclure un lien public vers votre document Google Feuilles de calcul.
https://docs.google.com/spreadsheets/d/1lzWKCiK3wRbvcReweSwHE6eMn_tIX7ZD1PHe1a8lKak/edit?usp=sharing 


Faites des observations générales concernant le jeu de données :
Combien y a-t-il de colonnes et de lignes?
Colonnes: 26
Lignes: 2603
Les données semblent-elles propres?
Non les données ne sont pas propres, et ne sont pas très bien organisés 
Nous avons remarqué que les donnés sont des fois un peu inutiles ou même qu’elles sont absentes
Nous avons aussi remarqué qu’il y a beaucoup de données quant aux âges, aux langues, aux immigrants, aux types de voitures, types de logements, types de revenues
Nous avons aussi remarqué et on a ete tres decu du fait qu’il n'y a pas de données par rapport au québec, tandis que le texte discutais de la relation entre travailler en ontario et habiter au québec et vis versa


Faites des observations spécifiques sur au moins trois colonnes : ????
À quels types de variables avons-nous affaire? Soyez spécifique. Par exemple : « La colonne A comporte des variables nominales avec les noms de tous les participants à l’étude. La colonne B inclut les âges des participants en tant que variables discrètes. »
Est-ce que quelque chose est manquant, extraordinaire, surprenant?


Formulez au moins une question ou une hypothèse qui vous vient à l’esprit lorsque vous examinez les données brutes.
Est-ce que ça vaut plus la peine d'être locataire plutôt que propriétaire dans la ville d’ottawa?



Utilisez deux croisillons (`##`) pour créer un intertitre de niveau 2 comme celui-ci.

Utilisez le modèle de code ci-dessous pour insérer une capture d'écran. Vos images doivent être sauvegardées dans le même dossier que votre fichier `.md`.

![](import-screen-capture.png)<br>
*Figure 1 : La fenêtre d'importation d'un fichier de Google Feuilles de calcul.*

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

Ceci est un test afin de voir si Git Hub fonctionne. BLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA BLABLABLABLA 

Nous avons réalisé notre analyse VIMA sur les données des lignes 757, 759, 760, 761, 762, 765, 767, 768 ainsi que les lignes 1951 à 1956. De façon générale, il s’agit des données que nous pensons qui pourraient nous être utiles dans nos recherches. 

Avant même d’avoir recours à diverses méthodes pour analyser nos données, nous avons remarqué quelques détails. 

Plusieurs données présentaient des erreurs de formatage. À titre d’exemple, les valeurs dans la colonne 757 n'étaient pas formatées de la même façon. Certaines de ces données étaient des chiffres alors que d’autres étaient en fait des dates. De plus, nous avons remarqué que les colonnes M et N présentaient souvent des erreurs de formatage majeures, qui rendaient parfois les valeurs aberrantes et, ainsi, invalides. Par exemple, toujours dans la ligne 757 qui est censée afficher un pourcentage, la valeur de la cellule à la colonne M affiche le chiffre 45 994. Comparativement aux autres données qui ensemble font une moyenne de 10,15%, la valeur de 45 000% ressort du lot et est impossible dans ce contexte.

Une fois les données nettoyées et ces détails réglés, nous avons eu la chance de procéder à des méthodes plus poussées pour faire notre analyse VIMA détaillée. 

À premier coup d'œil, les données des lignes que nous avons ciblées semblent toutes être valides. Il n’y a pas de données manquantes, et il ne semble pas y avoir de données invalides ou aberrantes.

Afin de confirmer ce constat, nous avons produit un premier graphique à l’aide des données des colonnes 7 et 8 de notre nouveau tableau nettoyé. Ce graphique, ci-dessous, nous a permis de confirmer qu’il n’a évidemment pas de valeur aberrante. De plus, il n’y a pas de valeurs invalides qui furent soulevées. 



Ensuite, afin de vérifier l’exactitude des données, nous avons procédé à divers calculs afin de voir si les chiffres de l’ensemble des quartiers coordonnaient avec les données pour l’ensemble de la Ville d’Ottawa. Nos résultats furent assez intéressants. La plupart des sommes, des moyennes ou des médianes de l’ensemble des quartiers ne correspondent pas aux données pour l’ensemble de la Ville d’Ottawa, mais la différence est parfois minime. 

Autrement, les données semblent valides et exactes. 

Utilisez trois croisillons (`###`) pour créer un intertitre de niveau 3 comme celui-ci. Je vous prie de suivre ce modèle en ce qui a trait aux intertitres de niveaux 1 et 2. Toutefois, je vous laisse le loisir d'utiliser les intertitres de niveau 3 comme bon vous semble.

Insérez votre texte ici.

Appuyez vos affirmations en citant les sources appropriées. Veuillez suivre les [normes APA en matière d'attribution dans le corps du texte](https://apastyle.apa.org/style-grammar-guidelines/citations).

**Par exemple :**

Comme l'affirme Cairo (2016), une visualisation de données doit être véridique...

### 3.2. Nettoyage des données

Insérez votre texte ici.

### 3.3. Analyse exploratoire des données (AED)

Insérez votre texte ici.

**Cette section doit inclure une capture d'écran de votre tableau croisé dynamique, comme ceci :**

![](pivot-table-screen-capture.png)<br>
*Figure 2 : Ce tableau croisé dynamique montre...*

**Cette section doit aussi inclure une capture d'écran de votre graphique exploratoire, comme ceci :**

![](chart-screen-capture.png)<br>
*Figure 3 : Ce graphique exploratoire montre...*

## 4. Récit potentiel

Les articles suivants vont nous permettre de comprendre la situation des logements au Canada mais plus spécifiquement à Ottawa. Afin de vraiment raconter une histoire et bien comprendre nos données, on doit comprendre la situation de logement afin d'avoir des informations précises sur plusieurs aspects qui peuvent influencer les choix des locataires ou propriétaires. Nous avons trouvé principalement des articles de journaux et des articles sur des sites de logements. Dans notre cas, ce sont des sources assez pertinentes, car elles viennent de journalistes et de professionnels dans le domaine du logement. Pour notre projet, nous examinons s’il est plus avantageux d’être propriétaire ou locataire à Ottawa selon les prix des logements, donc toutes ces sources seront des informations qui vont nous permettre de bâtir une conclusion concise et bien soutenue.  

Desjardins, S. (2025, February 11). Louer ou acheter: devenir propriétaire n’est pas un choix logique. Le Journal De Montréal. https://www.journaldemontreal.com/2025/02/09/louer-ou-acheter-devenir-proprietaire-nest-pas-un-choix-logique 

Du Canada Statistique Canada, G. (2021, September 2). Les statistiques : le pouvoir des données! https://www150.statcan.gc.ca/n1/edu/power-pouvoir/toc-tdm/5214718-fra.htm 

Eads, D. (2016, October 15). How to “interview” a big pile of data. NPR. https://www.npr.org/sections/npr-training/2025/05/29/g-s1-67278/how-to-interview-a-big-pile-of-data 

Info, R. (2025, February 25). Élections en Ontario : la crise du logement vue par les candidats de la région d’Ottawa. Radio-Canada. https://ici.radio-canada.ca/nouvelle/2143463/logement-ontario-ottawa-crise-election   

Malone, K. (2025, April 15). Are Ottawa condos a good investment in 2025? Here’s what you need to know — Matt Richling - Ottawa Condos and Lofts - Ottawa Real estate for sale. Matt Richling - Ottawa Condos and Lofts - Ottawa Real Estate for Sale. https://www.mattrichling.com/blog/are-ottawa-condos-a-good-investment-in-2025-heres-what-you-need-to-know 

Ottawa, J. P.-. R. I. K., & Polonski. (2023, November 14). Meet Jason Polonski – Kanata & Ottawa’s trusted real estate agent. Jason Polonski- Realtor in Kanata, Ottawa. https://ottawarealtyman.com/renting-vs-buying-in-ottawa/?srsltid=AfmBOopRTPe0wguJu-6BidNu77JeIqpCF0Rhsw_c5KqrPSvv65isi5a4 

https://www.cpacanada.ca/fr/nouvelles/analyse/acheter-louer 



## 5. Conclusion

Insérez votre texte ici.

## 6. Références

Veuillez inclure une liste de vos références ici. Assurez-vous de suivre les [normes APA pour les références](https://apastyle.apa.org/style-grammar-guidelines/references). Les retraits négatifs (*hanging paragraphs*) ne sont pas nécessaires. Le [guide sur l'adaptation APA](https://arts.uottawa.ca/lettres/sites/arts.uottawa.ca.lettres/files/cartu-outils-de-redaction-adaptation-apa.pdf) de l'Université d'Ottawa pourrait également vous être utile.

**Voici un exemple :**

Bounegru, L., & Gray, J. (Eds.). (2021). *The Data Journalism Handbook 2: Towards A Critical Data Practice*. Amsterdam University Press. [https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153](https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153)
