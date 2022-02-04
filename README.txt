README: GCMS Plotter

Hi, these instructions are wirtten for someone who is quite new to this world, apologise if
I am teaching you to suck eggs :) 

This code is best run (by that I mean tested) through Anaconda and Spyder. 
	- Download Anaconda (selecting your operating system):
	https://www.anaconda.com/products/individual

	- Install Spyder (looks scary, but isn't too bad)

The code works by utilizing a few packages (pre-written code that is called upon at various points)
The following packages are needed:

	- tkinter (handles some little error messages)
	- numpy (suite for maths based operations)
	- pandas (a generally useful module for handling files)
	- matplotlib (graph plotting module)
	- glob (computer-geekery)

To install these packages we will use a tool provided by Anaconda called "Anaconda prompt"
Search for this application once Anaconda is installed and open it. You will be presented with 
a black screen called a "Terminal". Through this terminal we will install the relevant packages:
Type (or copy/paste) the following commands into the terminal (one at a time):

	conda install -c anaconda tk

	conda install -c anaconda numpy

	conda install -c anaconda pandas
	
	conda install -c conda-forge matplotlib

	conda install -c conda-forge glob2

After typing each command into the terminal you will normally be presented with an option to install
the desired package that requires you to enter "yes" or "no" (y/n) in the terminal. Type "y" at this point
to continue to install. Once finished move on to the next package. The code runs a quick package check before
running the actual graph plotting code, so it should tell you if you haven't done this correctly and highlight 
which modules need installing. 

You might want to download the example dataset to help see how the code works/play around with a dataset. 
Available at the following link:

	https://drive.google.com/drive/folders/1Y_R7cTnjjOjI_rhV2P5Z9CadzrU7vuQM?usp=sharing

The actual code (Python script) is broken into segments denoted as follows:

////////////////////////////////////////////////
//                Segment Name                //
////////////////////////////////////////////////


Each segment has a breif overview and comments of what it trying to achieve. You can collapse these 
segments by pressing the small arrow next the line number at the top of a segment (appears when you
mouse over it), this makes for easier viewing!

Place your Agilent files into a folder and move that folder to the Data_Dump folder in the parent 
directory. You will need to tell the code what this folder is called (see "User Input" and "data" 
variable).

Choose a mode of operation (see variable "mode") and choose either relative or absolute abundances. 

You can run the code now and a graph/graphs will be produced. See "Graph Styling" segment for styling
options. Unless you really care, you can ignore the "Housekeeping and Code" segment. 

I'm sure bugs/issues will be thrown up by people using this code, contact me if you need help:
	mxa415@student.bham.ac.uk (Matt)

Outputs will be saved into Image_Dump as both Jpegs and SVG's. Have fun.