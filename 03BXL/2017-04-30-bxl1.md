# Workshop BXL 
note post workshop1:  
- [ ] Compléter les logiciels utilisés, justification?  
- [ ] Trier les documents en dossier /source, /référence, *...autres?*  
- [ ] Compléter la doc
- [ ] Faire le point sur les matériaux utilisés
- [ ] Scanner les papiers et ordonner chronologiquement
- [ ] Proposer la transcription des notes "prototype step"
- [ ] Comment gérer les traductions?
- [ ] Comment gérer les "issues" càd les bugs, les points à améliorer, les nouvelles pistes à explorer, ...  

## Objectifs 

**Description temporaire en vrac des sujets à questionnement:**  

- 3 types d'outils (point B) = 3 modèles de : 
  - léger: bic, crayon, pointe sèche, feutre, .... 
  - moyen: dremel ou allonge flexible, ... 
  - lourd: makita,....
  
- Structure?
	- rigidité en fonction de l'outil?
	- matériaux? 
	- méthode de fabrication, actuellement découpe laser et print3D + quincaillerie.
  
- Safety kids?    Quels sont les éléments auxquels faire attention?
  - projection copeaux?
  - ~~220V~~ vs 12V
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

- Limiteur Z, pour ajuster la profondeur de gravure de l'outil en fonction du matériau gravé?
- autres?

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
### A - Point Fixe

Le point fixe pourrait s'accrocher à la table avec une pince de type lampe de bureau. Je suis partis de ce modèle:   
http://www.thingiverse.com/thing:1460590

Pourquoi? Parce qu'avec la même pince, on peut y adapter différentes têtes grâce à une encoche en queue d'aronde. 
Print en PET pour plus de solidité. La première version en PLA a cassée sous la pression de serrage.   

Fusion360 file: http://a360.co/2n9jVwL    

![pointA1.1](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/PointA1.1.jpg)   

![pointA1.2](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/pointA1.2.jpg)    

**Matos:**   
- 2x vis M3 12mm,   
- 2x vis M6 16mm, tête fraisée  
- 1x rondelle M6,  
- 1x Ecrou M6,  
- 1x taraud M3 pour le pas de vis M3 dans "MountA"  
- 1x taraud M6 pour le pas de vis M6 dans le connecteur en queue d'aronde. 


### B - Porte outil

##### crayon/pencil
**Version 0.0**  
Simple hack avec un taraud M8 pour fixer un crayon à l'intérieur d'un roulement.   Si ça servira? Je ne sais pas, mais j'étais content de moi. :)

![pointB0.1](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/pointB0.1.jpg)  
![pointB0.2](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/pointB0.2.jpg)    

**Version 1.1**    
L'outil doit se positionner exactement au croisement des axes et pouvoir coulisser. L'idée de départ était d'utiliser un roulement à bille et de trouver le moyen de faire passer l'outil dans son centre puis de fixer les axes dessus.  

Fusion360 file: http://a360.co/2n8FAnX   

![pointB1.1](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/pointB1.1.jpg)  
![pointB1.3](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/pointB1.3.jpg)  

note: pour l'impression 3D de l'écrou "MegaBolt.stl", pour que le pas de vis coulisse bien, il faut agrandir X et Y (scale x1.02) , Z reste inchangé.

**Version 2.1**

Le roulement coute un peu cher, n'est pas standard et il provenait de mon stock.   
Son centre est d'un diamètre de 17mm, ce qui fonctionne bien mais limite cette solution pour utiliser des outils de diamètre supérieur à 10mm. Cette version crée le même principe mais complétement imprimé en 3D, le modèle est paramétrique donc ajustable au diamètre de l'outil.   

Fusion360 file: http://a360.co/2nrWama

![pointB2.1](https://github.com/openfab-lab/chic2.0/blob/master/03BXL/Working%20files/pointB2.1.jpg)


### C - Guide
### Axes?



