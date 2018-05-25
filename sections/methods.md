### NLTK Methods with the NLTK Corpus

*All of the code for this section is in a Jupyter Notebook in the GitHub Repository. I encourage you to follow along by retyping all of the code, but if you get lost, or want another reference, the code is there as well. To open it in a Jupyter Notebook, Launch the Notebook and then through the file list that appears in your browser, navigate to where you saved the file.*

Return to the Jupyter Home Tab in your Browser (or Launch the Jupyter Notebook again), and start a New Python3 Notebook using the 'New' button in the upper right corner. 

Start by importing the NLTK library by typing:

	import nltk

**Libraries** are sets of instructions that Python can use to perform specialist functions. The Python programming language is very simple by design, and can be used for a wide variety of functions. It allows users to customize it to their needs by importing packages. Packages are written by individuals and groups who see the need for a simple set of commands to do routine functions. The Natural Language ToolKit (NLTK) is one such library. As the name suggests, its focus is on language processing. 

We will also need the matplotlib library later on, so import it now:

	import matplotlib
	
Matplotlib is a library for making graphs. In the middle of this tutorial, we are going to make a dispersion plot of words in our texts. To see 

Finally, because of a quirk of Jupyter notebooks, we need to specify that matplotlib should display its graphs in the notebook (as opposed to in a separate window), so we type this command (this is technically a Jupyter command, not Python):

	%matplotlib inline

All three of these commands can be written in the same cell and run all at once (**Shift** + **Enter**) or in different cells. 

![Image showing that the three lines given above should be written in a single cell in the JuPyther notebook, one after another](https://github.com/DHRI-Curriculum/text-analysis/blob/incorporate-feedback/images/jupyter4.png)

If you don't see an error when you run the notebook—that is, if nothing happens—you can move on to the next step.

Next we need to load all of the NLTK corpora into our program. Even though we downloaded them to our computer, we need to tell Python we want to use them.

	from nltk.book import *

The pre-loaded NLTK texts should appear again. These are pre-formatted data sets. We will still have to do some minor processing, but having the data in this format saves us a few steps. At the end of this tutorial, we will make our own corpus. This is a special type of python object specific to NLTK (it isn't a string, list, or dictionary). Sometimes it will behave like a string, and sometimes like a list of words. How it is behaving is noted for each function below.

![Image showing a second cell with the "from nltk.book import *" line and another line defining some text data](https://github.com/DHRI-Curriculum/text-analysis/blob/incorporate-feedback/images/jupyter5.png)

Let's start by analyzing **Moby Dick**, which is text1 for NLTK.
