The following instructions are for installing and running the project on Ubuntu

Prerequisites

	1. TeX Live 2012
	2. ConTeXt
	3. TeXworks
	
	Installation: 
		1. Install TeX Live 2012
			a. sudo add-apt-repository ppa:texlive-backports/ppa
			b. sudo apt-get update
			c. sudo apt-get install texlive
			d. sudo apt-get upgrade

		2. Install ConTeXt
			a. sudo apt-get install context

		3. Install TeXworks
			a. sudo apt-get install texworks
	

Using the API

	Directory structure:

		|-- base
		|   |-- java-imp-fld.mkiv
		|-- Project
		|   |-- Algorithms
		|   |   |-- arrayAlgos.tex
		|   |   |-- graphAlgos.tex
		|   |   |-- listAlgos.tex
		|   |   |-- treeAlgos.tex
		|   |-- API
		|   |   |-- arrayAPI.tex
		|   |   |-- baseAPI.tex
		|   |   |-- graphAPI.tex
		|   |   |-- listAPI.tex
		|   |   |-- treeAPI.tex
		|   |-- Examples
		|   |   |-- arrayExample.tex
		|   |   |-- endnext.png
		|   |   |-- graphExample.tex
		|   |   |-- listExample.tex
		|   |   |-- minus.png
		|   |   |-- nextbreak.png
		|   |   |-- next.png
		|   |   |-- playpause.png
		|   |   |-- plus.png
		|   |   |-- prevbreak.png
		|   |   |-- prevend.png
		|   |   |-- prev.png
		|   |   |-- togglepause.png
		|   |   |-- toggleskip.png
		|   |   |-- treeExample.tex
		|-- t-animation
		|   |-- animation
		|   |	|-- t-animation.mkvi
		
	Structure Explanation :
		
		1. API folder has the low level API files.  
		2. Algorithms folder contains the high level API files.
		3. Examples folder contains the samples to create animations using the high level API.

	Instructions for using the project :
	
		1. Copy the 'animation' directory from the 't-animation' directory to the following directory
			/usr/share/texmf/tex/context/third/

		2. Repalce the 'java-imp-fld.mkiv' in 
			/usr/share/texmf/tex/context/base/
			with 'java-imp-fld.mkiv' file from the 'base' directory
			
		3. Copy the 'Project' directory to a preferred location

		4. Compile the tex files from the 'Example' directory using Texworks having ConTeXt as the Typesetting engine.
