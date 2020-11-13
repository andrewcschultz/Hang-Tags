# Hang-Tags

What it does
------------

This code is designed to help you make hang tags for beer; the code is set up predominantly for lambic beer, but can be modified to include other producers as well.  After you create a database of information (see below), you can compile the code (see below) to generate a PDF.  The PDF is sized 8.5 inches by 11 inches.

What's here
------------


**tags.csv**

This is a sample file which showcases how one enters data that will be used to create the tags.  It is a comma separated list, with each line giving the information of the producer, color, date, name, size, cap/cork, and inventory number (if desired) of a given bottle.  More on how to format this file below.

**An assorthment of PNG files**

These include files for producers and for "color swatches".  You'll only need files for the producers/colors you use. 
	
**tags.tex**

This is the code which merges your data from the tags.csv file with the various image files to create the tags. 
 
Getting started -- if you don't already have a LaTeX compiler
---------------------------------------------------------------

Export the files in this project by clicking the green "Clone or Download" button; this should be downloaded to your computer as 'Hang-Tags-master.zip' (or something equally inspiring).  Go to Overleaf.com and create a new personal account; it's a free online LaTeX compiler.  Once you've logged into your account, click the "New Project" button in the upper left, and then select "Upload Project."  This will give you the chance to upload a zip file, so give it the 'Hang-Tags-master.zip' file you exported a moment before. It will take a second to process, but soon you'll see it show up.  You can expand the file structure by clicking on the arrow next to the folder called 'tags'.  Unfortunately Overleaf doesn't allow you to edit the file 'tags.csv' directly in its editor, so you'll need to download it to your computer, enter your data locally (using a plain text editor), and then re-upload.  (See 'Setting up the tags.csv file' below for information about how to format this file.)

Getting started -- if you already have a LaTeX compiler
-------------------------------------------------------

Export the files in this project by clicking the green "Clone or Download" button; this should be downloaded to your computer as 'Hang-Tags-master.zip' (or something equally inspiring).  Unzip the folder.  The correct file structure should be in place, and you only have to edit the 'tags.csv' file with your data.  When you're ready (don't forget to save the changes to 'tags.csv'!), compile the 'tags.tex' file. You'll have to compile twice in a row for the document to display correctly.

Setting up the tags.csv file
----------------------------

When inputting your entries into the tags.csv file, be sure to not disturb the first line; your entries will start on the second line. Each entry in the tags.csv file takes the following form

    producer,color,bottledate,note,size,cap/cork,ID
    
The allowable entries for `producer` are: 
*	3Floyds					====		Generic 3 Floyds logo
*	BFM					====		Generic Brasserie des Franches-Montagnes logo
*	Bokke					====		Generic Bokke/Bokkeryder logo
*	Boon					====    	Generic Boon logo
* 	BoonBlackLabel				====		Generic Boon Black Label logo (no edition number)
*	BoonMariageParfait
*	BoonMikkellerCalvadosOG		
*	BoonOG						
*	BoonVAT					====		Generic Boon VAT (no VAT number)
*	Cantillon				====		Generic Cantillon logo
*	Cantillon50n4e
*	CantillonBlabaer
*	CantillonBrabantiae
*	CantillonCG				====		Non-US label for Cantillon classic gueuze
*	CantillonCGus				====		US label for Cantillon classic gueuze
*	CantillonCSG				====		Cuvee Saint-Gilloise
*	CantillonFF				====		Fou Foune
*	CantillonGCB				====		Non-US Grand Cru Bruocsella (no date)
*	CantillonIris				
*	CantillonKriek
*	CantillonLouPepe
*	CantillonNath2018
*	CantillonRDG
*	CantillonStLamvinus
*	CantillonVigneronne
*	Chimay					====		Generic Chimay logo
*	Cycle					====		Generic Cycle logo
*	DeCam					====		Generic De Cam logo
*	Drie					====		Generic Drie Fonteinen logo (fountains)
*	DrieAG					====		sublogo on silkscreen bottles
*	DrieAGHoning				====		sublogo on silkscreen bottles
*	DrieAGPaper				====		Paper label for Armand & Gaston (75cl on label)
*	DrieAGV2015				====		sublogo on silkscreen bottles
*	DrieBraambes				====		sublogo on silkscreen bottles
*	DrieDoesjelPaper			====		Paper label (12.7oz on label)
*	DrieFramboos				====		sublogo on silkscreen bottles
*	DrieFrambozenlambik			====		sublogo on silkscreen bottles
*	DrieFramboosOogst2017			====		sublogo on silkscreen bottles
*	DrieGoldenBlend				====		sublogo on silkscreen bottles
*	DrieHommage				====		sublogo on silkscreen bottles
*	DrieHommageBioFrambozen			====		sublogo on silkscreen bottles
*	DrieHommageBioFrambozenBarrel		====		sublogo on silkscreen bottles
*	DrieHommageBioFrambozenHoning		====		sublogo on silkscreen bottles
*	DrieAardbei				====		sublogo on silkscreen bottles
*	DrieAardbeiKriek			====		sublogo on silkscreen bottles
*	DrieIntenseRed				====		sublogo on silkscreen bottles
*	DrieKriek				====		sublogo on silkscreen bottles
*	DrieKriekBarrel				====		sublogo on silkscreen bottles
*	DrieKriekenlambik			====		sublogo on silkscreen bottles
*	DrieKriekHoning				====		sublogo on silkscreen bottles
*	DrieKriekPaper				====		Paper label (37.5cl on label)
*	DrieRobijn				====		sublogo on silkscreen bottles
*	DriePerzik				====		sublogo on silkscreen bottles
*	DrieOG					====		sublogo on silkscreen bottles
*	DrieOGHoning				====		sublogo on silkscreen bottles
*	DrieOGPaper				====		Paper label (37.5cl on label)
*	DrieOGPaperus				====		US Paper label (12.7oz on label)
*	DrieOGV2014				====		Paper label	Nachtlichten artwork
*	DrieOGV2016				====		Paper label	Nachtlichten artwork
*	DrieOld					====		Generic Drie Fonteinen logo (Papyrus-typeset "3")
*	DrieSchaarbeekseKriek			====		sublogo on silkscreen bottles
*	DriePlatinum				====		sublogo on silkscreen bottles
*	DrieRodeBosbes				====		sublogo on silkscreen bottles
*	DrieBlauweBosbes			====		sublogo on silkscreen bottles
* 	DrieSpelingVIIIiii			====		sublogo on silkscreen bottles
* 	DrieZenne92				====		sublogo on silkscreen bottles
* 	DrieZenne93				====		sublogo on silkscreen bottles
* 	DrieZenne94				====		sublogo on silkscreen bottles
*	Girardin				====		Generic Girardin logo
*	GirardinBlackLabel				
*	HanssensHandgeplukte			====		Hanssens Oude Kriek Handgeplukte Schaarbeekse Krieken
*	HORAL2017
*	LambickX				====		Generic LambickX logo
*	LambiekFabriek				====		Generic Lambiek Fabriek logo
*	Lindemans				====		Generic Lindemans logo
*	LindemansBlossomGueuze
*	LindemansCuveeRene
*	LindemansCuveeReneKriek
*	LindemansCuveeReneSB			====		2010 special blend
*	LindemansGingerGueuze
*	MikkellerSpontanCherryFred		====		Frederiksdal version of SpontanCherry
*	MoriauGeuze
*	OudBeersel
*	OudBeerselGreenWalnut
*	OudBeerselKriek
*	OudBeerselPijpenGeuze			====		Barrel Selection Oude Pijpen Geuze Vieille
*	OudBeerselSchaarbeekseKriek
*	OudBeerselVandervelden135
*	SideProject				====		Generic SideProject logo
*	Struise					====		Generic Struise logo
*	TommieSjef				====		Generic Tommie Sjef logo
*	Tilquin					====		Generic Tilquin logo
*	TilquinCassis
*	TilquinMure
*	TilquinOG
*	TilquinPinotGris
*	TilquinPinotNoir
*	TilquinQuetsche

The allowable entries for `color` are:
		yellow;
		purple;
		blue;
		red;
		orange;
		orangered;
		green;
		pinkred;
		clear;
		lightorange;
		cream;
		darkpurple;
		black;
		3f_green 	(3 Fonteinen Oude Gueuze);
		3f_darkgreen	(3 Fonteinen Armand & Gaston);
		3f_purple	(3 Fonteinen Schaarbeekse Kriek);
		3f_darkpurple	(3 Fonteinen Braambes);
		3f_red		(3 Fonteinen Kriek);
		3f_red_robijn	(3 Fonteinen Robijn);
		3f_red_bosbes	(3 Fonteinen Rode Bosbes);
		3f_darkblue	(3 Fonteinen Blauwe Bosbes);
		3f_pink		(3 Fonteinen Framboos & Hommage);
		3f_pink_perzik	(3 Fonteinen Perzik);
		3f_pink_aardbei	(3 Fonteinen Aardbei & Aardbei Kriek);
		3f_silver	(3 Fonteinen Platinum);
		3f_yellow	(3 Fonteinen Golden Blend);
		3f_zenne92	(3 Fonteinen Zenne Y Frontera Blend 92);
		3f_zenne93	(3 Fonteinen Zenne Y Frontera Blend 93);
		3f_zenne94	(3 Fonteinen Zenne Y Frontera Blend 94).
		
		
You may enter any string of text you like for `bottledate`.  It will be displayed at the top of the tag (within the color swath, assuming you choose a color other than 'clear'.

You may enter any string of text for  `note` that you like.  Leaving this entry blank will mean no string is printed.

If your `size` entry is one of 375, 750 or 1500, three circles to the left of the cutout will be drawn, and one of the circles will be shaded to indicated the size (375 is the top circle, 750 is the middle circle, and 1500 is the bottom circle).  If you enter any size that is not one of these three numbers, those circles on the left will not display.

In the `cap/cork` entry, if you write 'cap' then the cutout will be a circle of diameter 1.25in.  This is sufficient to fit around the cap of all (of my) capped bottles, but won't go past the neck.  (The cap seems to provide sufficient barrier to tags falling off easily.)  If you write 'cork' (or really, anything else besides cap), then the cutout will be a circle of diameter 1.5in.  This is sufficient to fit around the cork/cage of all (of my) cork and caged bottles.  These tags go further down the neck than their capped counterparts.

If you have an inventory number for your bottles, you can type the inventory number in the `ID` entry.  If you put an entry in this slot, it's printed to the right of the cutout in a small rectangular box.  If you enter nothing, the box is not drawn.


Tips
----

You can purchase circular die cutters of size 1.25in and 1.5in.  These result in perfectly cut circles and make life much easier.

I print my tags on thick cardstock paper so they don't bend or crease as easily.

It's quite hard to get a printer to print the 8.5x11 content of the resultant PDF perfectly onto an 8.5x11 sheet of paper (even if your printer has "borderless" printing capabilities).  You might need to experiment to find your best option for maximizing the size of the printed product without losing content off the side of the printed page. In my case, I have an option to scale to print the entire image (which means: scale by 97%), and this works fairly well.

Finally, what I've set up for myself might not be precisely what you want for yourself; feel free to change the code as you see fit.  If you don't have experience in coding LaTeX, feel free to reach out to me with questions.  If you have other labels you'd like to see included, feel free to give it a whirl yourself or send me an email.

# Note

I do not own the rights to the logos or labels printed on these tags, and this program is not intended for the commericial use of these images. It is shared only for private use. If any producer wishes me to remove their images from this program, please contact me and I will remove them immediately.
