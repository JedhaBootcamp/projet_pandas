1)	Téléchargez les trois fichiers “superficie.csv” / “nombre_de_sdb.csv” / “nombre_de_chambres.csv”
2)	Importez les trois datasets
3)	Donnez un nom de colonne à ces trois datasets
4)	Fusionner ces trois datasets un seul dataframe (on fera une fusion simplement par index) qu’on nommera dataset
5)	Quelle est la superficie moyenne des maisons de notre dataset ?
6)	Quelle est le nombre de chambre médian et moyenne ?
7)	Nous un nouveau dataset “house_price.csv” que nous voudrions intégrer à notre dataset 
a)	Cette fois nous voudrions fusionner les index avec les id du dataset.
i)	Importez house_price.csv dans une variable qu’on nommera house_price
ii)	Créez un id pour dataset qui sera égal à l’index de dataset
iii)	Fusionnez house_price à dataset 
8)	Quel est le coût moyen d’une maison ?
9)	Quel est le coût moyen par chambre ?
10)	 Le coût moyen par chambre ne nous apprend pas grand chose.
a)	Tentons de faire des catégories de superficie
i)	Créez une nouvelle colonne dans votre dataset qu’on appellera taille_maison
ii)	Créez trois catégories “très grande” / “grande” / “moyenne” / “petite” / “très petite” qui respectivement correspondront à :
(1)	 “une maison dont la taille est supérieure à 25 000 sqrt_feet”
(2)	 “une maison dont la taille est comprise entre 20 000 et 25 000 sqrt_feet”
(3)	“une maison dont la taille est comprise entre 15 000 et 20 000 sqrt_feet”
(4)	 “une maison dont la taille est comprise entre 10 000 et 15 000 sqrt_feet” 
(5)	“une maison dont la taille est inférieure à 10 000 sqrt_feet”
iii)	Remplissez les lignes correspondantes dans la colonne taille_maison
11)	Quel est le coût moyen d’une maison en fonction de sa catégorie de superficie ?
12)	 Appliquez le code ci-dessous pour visualiser votre résultat. Que pouvez vous conclure ?

import seaborn as sns
sns.lmplot(x = "sqrt_meters", y="house_price", data = dataset)

