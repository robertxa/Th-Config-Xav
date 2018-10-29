Therion Config file
===================================================

Version 2.0 B1 - Oct 29, 2018

Created by Xavier Robert

Licence
-------  
Released under a Creative Commons Attribution-ShareAlike-NonCommecial License:
	<http://creativecommons.org/licenses/by-nc-sa/3.0/>

Usage
-----

1. Copy the file in the master/parent folder of your caves' surveys database

2. In your *.thconfig file, you need to call this file with: 

	``input <path/to/the/file/>config.thc``

3. and then, in each layout, you need to call the layout(s) of the config.thc you may interested in: 

	ex: ``copy drawingconfig``


Layouts of the config.thc
-------------------------

In the config.thc, there are different parts and layouts :

1. a first part where the legend names can be changed, according to the language called by the Therion keyword ``language XX``

2. layout langue-XX with XX = fr, es or en: Layout to change the language in the header and the legend. it also define the Therion keyword ``language XX``

3. Layout drawconfig: layout that set colors/size of symbols, define new symbols...

4. layout headerl: Redefine the header for the plan view

5. layout header_coupe:  Redefine the header for the extended view

6. layout layoutmapborder: to add a border to the pdf exports

7. layout layouAtlasNorthArrow: redefinition of the atlas definition

8. Layout layoutcontinuation: to write all the texts that go with continuations marks

9. layout northarrowMG: New north arrow definition


Templates for .thconfig and .th files
-------------------------------------
The folder ``Template_cave`` contains an example of a survey-folder structure and of some .th and .thconfig files with all the commands explained in french and english.
You can use these files if you modify them according to your project.

Have fun...


