# Workshop BXL 
## Objectifs 
## Contenu du workshop
### Les bases mathématique
*référence:*  
http://bidouillesetmathscollege.blogspot.be/2012/02/pantographes.html  

Après un premier proto très basique, les conclusions mathématiques sont:   
Soit les points **A**, **B** et **C** avec A fixe, B le porte outils et C le guide.   
Soit **R** = le ratio   
ET les segments tel que:  

![Math00](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/Math00.png)

Le calcul de ratio se fait en fonction de la longueur totale du segment AD divisé par la longueur de AE.    
**R = AD/AE**

![MathRatio](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/MathRatio%20low.jpg)

Fusion360 File: http://a360.co/2ne4I0O  

##### Proto 1.0
Découpe laser 4x dans MDF 3mm de [test01Pantographe.svg](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/test01Pantographe.svg)  
L'assemblage suivant a permis de valider par la pratique les théories mathématique.

![Proto 1.0](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/Proto1.0.jpg)

##### Proto 1.1

L'update se focalise sur l'automatisation du calcul de ratio ainsi que la validation des distances à atteindre. 
Ici, l'objectif est de partir d'un dessin de taille A4 vers une réduction 1/5ème au maximum.  

![Proto 1.1](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/Proto1.1.jpg)

Fusion360 file: http://a360.co/2mwILFR

### Liste matériels (BOM)

Liste temporaire d'achat pour le workshop de MARS  
https://github.com/openfab-lab/chic2.0/blob/master/03BXL/AchatWRKShop.md

### Liste Logiciels

Logiciel utilisé:
- Autodesk Fusion360 pour la 3D.  
http://www.autodesk.com/products/fusion-360/overview  
Logiciel propriétaire mais très accessible, comprenant à la fois les outils de modélisation, les outils CAM pour le controle machine ainsi qu'un système de version similaire à GIT pour le travail collaboratif.  
- Inkscape pour la 2D.   
https://inkscape.org/


## Composantes du montage

**Description temporaire en vrac des sujets à questionnement:**  

- 3 types d'outils (point B): 
  - léger: bic, crayon, pointe sèche, feutre, .... 
  - moyen: dremel ou allonge flexible, ... 
  - lourd: makita,....
- Safety kids?    Quels sont les éléments auxquels faire attention?
  - projection copeaux?
  - poids? 
  - Mise en action? Que se passe t'il si l'enfant lache le guide? Arrêt automatique, balance de l'outil, séparation physique entre outil et guide avec plexi?
- Les matériaux?
  - Lino
  - Bois
  - Caoutchouc
  - métal, cuivre, laiton?
  Est-ce qu'il y a des risques de projections, d'usage, d'usinage? Quels sont les méthodes de travail?
- Les guides? (point C)
  - échelles visuelles de référence adpatée au ratio de réduction et à l'outil utilisé.
  - visibilité? (élément en plexi)
- Structure?
	- rigidité en fonction de l'outil?
	- matériaux? 
	- méthode de fabrication, actuellement découpe laser et print3D + quincaillerie.
- Limiteur Z, pour ajuster la profondeur de gravure de l'outil en fonction du matériau gravé?
- autres?


### A - Point Fixe
### B - Porte outil

##### crayon/pencil
Simple hack avec un taraud M8 pour fixer un crayon à l'intérieur d'un roulement.   Si ça servira? Je ne sais pas, mais j'étais content de moi. :)

![pointB1](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/pointB0.1.jpg)
![pointB2](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/pointB0.2.jpg)    


### C - Guide
### Axes?



