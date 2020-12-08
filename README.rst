Therion Config file
===================================================

Version 3.1 - Apr. 27, 2020

Created by: / Créé par : Xavier Robert

Licence
-------  
Released under a Creative Commons Attribution-ShareAlike-NonCommecial License:
	<http://creativecommons.org/licenses/by-nc-sa/4.0/>

Publié sous la licence Creative Commons Attribution-ShareAlike-NonCommecial:
	<http://creativecommons.org/licenses/by-nc-sa/4.0/>

Langue (fr)
-----------
Le readme en langue française est à la suite de celui en langue anglaise !

Usage (en)
----------

1. Copy the file in the master/parent folder of your caves' surveys database

2. In your *.thconfig file, you need to call this file with: 

	``input <path/to/the/file/>config.thc``

3. and then, in each layout, you need to call the layout(s) of the config.thc you may interested in: 

	ex: ``copy drawingconfig``


Layouts of the config.thc (en)
------------------------------

In the config.thc, there are different parts and layouts:

1. a first part where the legend names can be changed, according to the language called by the Therion keyword ``language XX``

2. layout langue-XX with XX = fr, es or en: Layout to change the language in the header and the legend. It also define the Therion keyword ``language XX``

3. Layout drawconfig: layout that set colors/size of symbols, define new symbols...

4. layout headerl: Redefine the header for the plan view

5. layout header_coupe: Redefine the header for the extended view, with horizontal scale bar

6. layout layoutmapborder: to add a border to the pdf exports

7. layout layouAtlasNorthArrow: redefinition of the atlas definition

8. Layout layoutcontinuation: to write all the texts that go with continuations marks

9. layout northarrowMG: New north arrow definition

10. layout scalebar_horiz: horizontal scale bar definition

11. layout scalebar_vert: vertical scale bar definition

12. header_coupe_vert-auto: Redefine the header for the extended view, with vertical scale bar situated to the right of the header

13. header_coupe_vert-to-place: Redefine the header for the extended view, with vertical scale bar that needs to be placed within the layout in the thconfig file

14. layout test: to test new configurations if needed!

New symbols definitions (en)
----------------------------
Today the layout drawconfig defines new points/lines/areas symbols. To use them, use for each type of symbol (point, line or area) the u definition: u:_NEW_SYMBOL_NAME.
New points are:

1. nest (u:nest)

2. gradient -->	geologic dip

3. danger (u:danger)

4. bats (u:bats)

5. stalactite boss (u:boss)

6. artificial anchor (u:anchor_artificial)

7. natural anchor (u:anchor_natural)

8. shell (u:shell) 

9. masonry (u:masonry)

10. Ex voto/Signature (u:ex_voto)

11. Human bones (u:human_bones)

New lines are:

1. strata (u:strata; option -clip off)

2. coupole (u:coupole; option -clip off)

3. fault (u:fault; option -clip off)

4. doline (u:doline; option -clip off)

5. bats (u:bats)

6. surface (u:surf; option -clip off)

7. rail (u:rail)

8. plan walk (u:planwalk)

9. handrail/rambarde (u:handrail)

10. Dive line/Fil d'Ariane (u:ariane)

11. Deviation/Déviation (u:deviation)

New areas are:

1. mud (u:boue)

2. guano (u:guano)

3. bats (u:bats)

4. tree-trunc (u:tronc; options -clip off -place top)

5. tree-leaves (u:feuilles; option -clip off)

6. tunnel initiation (u:galerie)

Templates for .thconfig and .th files (en)
------------------------------------------
The folder ``Template_cave`` contains an example of a survey-folder structure and of some .th and .thconfig files with all the commands explained in french (<fr>) and english (<en>).
You can use these files if you modify them according to your project.

Folder TEST_THERION (en)
------------------------
This folder contains test cases used for the development of new function for the config.thc. Everything here is in development, and do not really work.
If you have hints, do not hesitate to contact me.

Have fun...

Some example of use (en)
------------------------

You will find some real example based on these files in:

1. Folly's karst area database (France) <https://github.com/robertxa/Topographies-Samoens_Folly>

2. Peruvian caves surveys database <https://github.com/robertxa/Mapas_Cavernas_Peru>

Utilisation (fr)
----------------

1. Copier le fichier dans le dossier master/parent folder de votre cavité ou de votre base de données topographiques

2. Dans votre fichier *.thconfig, vous devez appeller ce fichier avec la ligne : 

	``input <path/to/the/file/>config.thc``

3. Et ensuite, dans chaque layout de votre *.thconfig, vous devez appeller le layout(s) du fichier de configuration config.thc qui vous intéresse en rajoutant la ligne : 

	ex: ``copy drawingconfig``


Layouts disponibles dans le config.thc (fr)
-------------------------------------------

Dans le config.thc, il y a différentes parties et layouts :

1. Une première partie où les descriptions de la légende peuvent être modifiées, en fonction de la langue définie par le mot-clef Therion ``language XX``

2. layout langue-XX avec XX = fr, es où en : Layout pour changer la langue du cartouche (header) et de la légende. Cela définit aussi le mot-clef Therion ``language XX``

3. Layout drawconfig : Layout qui permet de définir la couleur, la taille de symboles, ainsi que de nouveaux symboles...

4. layout headerl : Redéfinit le cartouche (header) pour la projection en plan

5. layout header_coupe :  Redéefinit le cartouche (header) pour la coupe développée

6. layout layoutmapborder : Pour ajouter un cadre de bordure aux exports pdf

7. layout layouAtlasNorthArrow : Redéfinition de la flèche du nord pour l'Atlas

8. Layout layoutcontinuation : Pour écrire tous les textes qui sont donnés dans les points de continuations (i.e. avec l'option -attr Code XX -text "C'est ce texte là qui est écrit"

9. layout northarrowMG : Nouvelle définition de la flèche du nord

10. layout scalebar_horiz: Nouvelle définition d'une barre d'échelle horizontale

11. layout scalebar_vert: Nouvelle définition d'une barre d'échelle verticale

12. header_coupe_vert-auto: Redéfinition du header pour les coupes, avec une échelle verticale situé sur la droite du header

13. header_coupe_vert-to-place: Redéfinition du header pour les coupes, avec une échelle verticale à placer par l'utilisateur dans le layout du fichier thconfig

14. layout test : pour tester de nouvelles configurations si besoin !

Nouvelles définitions de symboles (fr)
--------------------------------------
Actuellement, le layout drawconfig définit de nouveaux symboles de points, de lignes et d'aires, qui peuvent être appelés en utilisant pour chaque entité (point, ligne ou aire) la définition u:NOM.
Les nouveaux points sont :

1. nid (u:nest)

2. gradient -->	pendage géologique

3. danger (u:danger)

4. chauves-souris (u:bats)

5. stalactite boss (u:boss)

6. ancrage artificiel (u:anchor_artificial)

7. ancrage naturel (u:anchor_natural)

8. coquille fossile (u:shell) 

9. maçonnerie (u:masonry)

10. Ex voto/Signature (u:ex_voto)

11. ossements humains (u:human_bones)


Les nouvelles lignes sont :

1. strate (u:strata ; option -clip off)

2. coupole (u:coupole ; option -clip off)

3. faille (u:fault ; option -clip off)

4. doline (u:doline ; option -clip off)

5. chauves-souris (u:bats)

6. surface (u:surf ; option -clip off)

7. rail (u:rail)

8. chemin construit (u:planwalk)

9. rambarde (u:handrail)

10. Dive line/Fil d'Ariane (u:ariane)

11. Deviation/Déviation (u:deviation)

Les nouvelles aires sont :

1. boue (u:boue)

2. guano (u:guano)

3. chauves-souris (u:bats)

4. tronc d'arbre (u:tronc ; options -clip off -place top)

5. feuillage d'arbre (u:feuilles ; option -clip off)

6. départ d'une galerie (u:galerie)


Templates pour fichiers .thconfig et .th (fr)
---------------------------------------------
Le dossier ``Template_cave`` contient un exemple de la structure d'un dossier d'une topographie et de quelques fichiers .th et .thconfig avec les commandes principales expliquées/décrites en français (<fr>) et en anglais (<en>).
Vous pouvez utiliser ces fichiers en les adaptant à votre project.

Dossier TEST_THERION (fr)
------------------------
Ce dossier contient des exemples-tests pour le développement de nouvelles fonction du config.thc. Tout ce qui est ici est en développement et ne fonctionne pas correctement.
Si vous avez des idées ou des solutions pour aider à ce développement, n'hésitez pas à me contacter.

Bon courage...

Quelques exemples d'utilisation (fr)
------------------------------------

Vous trouverez des exemples réels basés sur ces fichiers et structure :

1. La base de données topographiques des cavités du massif du Folly (France) <https://github.com/robertxa/Topographies-Samoens_Folly>

2. La base de données topographiques des cavités du Pérou <https://github.com/robertxa/Mapas_Cavernas_Peru>
