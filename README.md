# Hang-Tags

What it does
------------

This software is designed to help you make hang tags for beer; the code is set up predominantly for lambic beer, but can be modified to include other producers as well.  After you create a database of information (see below), you can compile the code (see below) to generate a PDF.  The PDF is sized 8.5 inches by 11 inches.

What's here
------------


**tags.csv**

This is a sample file which showcases how one enters data that will be used to create the tags.  It is a comma separated list, with each line giving the information of the producer, color, date, name, and size of a given bottle.  More on how to format this file below.

**An assorthment of PNG files**

These include files for producers and for "color swatches".  You'll only need files for the producers/colors you use. 
	
**tags.tex**

This is the code which merges your data from the tags.csv file with the various image files to create the tags. 
 
Getting started -- if you don't already have a LaTeX compiler
---------------------------------------------------------------

Export the files in this project; this should be downloaded to your computer as 'tags.zip'.  Go to Overleaf and create a new personal account; it's free!  Once you've logged into your account, click the "New Project" button in the upper left.  This will give you the chance to upload a zip file, so give it the 'tags.zip' file you exported a moment before. It will take a second to process, but soon you'll see it show up.  You can expand the file structure by clicking on the arrow next to the folder called 'tags'.  Unfortunately Overleaf doesn't allow you to edit the file 'tags.csv' directly in its editor, so you'll need to download it to your computer, enter your data locally (using a plain text editor), and then re-upload.  (See 'Setting up the tags.csv file' below for information about how to format this file.)

Getting started -- if you already have a LaTeX compiler
-------------------------------------------------------

To generate the tags you need to (1) update the tags.csv file with the data for the tags you want to create, and (2) compile the tags.tex code in a LaTeX compiler.  The tags.csv file and tags.tex file need to be in the same directory; a folder called tag_graphics should also be in this same directly, and all image files for producers and colors go into the tag_graphics folder.

Setting up the tags.csv file
----------------------------

When inputting your entries into the tags.csv file, be sure to not disturb the first line; your entries will start on the second line. Each entry in the tags.csv file takes the following form

    producer,color,bottledate,beername,size
    
The allowable entries for producer are: 
 		Ca = Cantillon;
		DF = Drie Fonteinen (new silkscreen bottle);
		DF_old  = Drie Fonteinen (old silkscreen bottle);
		OB = Oud Beersel;
		B = Boon;
		G = Girardin;
		DC = De Cam;
		T = Tilquin;
		BFM = Brasserie Franches-Montagnes;
		Ch = Chimay;
		L = Lindemans;
    Bo = Bokkereyder
    LF = Lambiek Fabriek

The allowable entries for color are:
		yellow
		purple
		blue
		red
		orange
		orangered
		green
		pinkred
		clear
		lightorange
		cream
		darkpurple

If your size entry is one of 375, 750 or 1500, a corresponding circle to the left of the cutout will be shaded.  Obviously you can use these numbers as proxies for "small", "medium" and "large" bottles.


Tips
----

It's quite hard to get a printer to print the 8.5x11 content of the resultant PDF perfectly onto an 8.5x11 sheet of paper (even if your printer has "borderless" printing capabilities).  You might need to experiment to find your best option for maximizing the size of the printed product without losing content off the side of the printed page. In my case, I have an option to scale to print the entire image (which means: scale by 97%), and this works fairly well.
