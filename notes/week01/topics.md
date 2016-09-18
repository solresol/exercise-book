What we covered, day-by-day
===========================




Monday
------

Shell commands, including:

 - cat, mkdir, rmdir, rm, touch, cd, pwd
 
 - how the shell splits into words
 
 - how * and ~ expand
 
Git

 - add, commit, push, pull

Python programming

 - confirmed that everyone was quite confident about 
 types, functions, dictionaries, lists, and so on
 
Python notebooks

 - string.split
 
Numpy intro

 - what is numpy, why do we use it
 
 - creating arrays with numpy.arange, numpy.array
 
 - statistical functions
 
 - selecting elements and columns
 
 - reshaping
 
 - lab exercises 4.2 and 4.3


Matplotlib intro

 - how to create a simple graph from some numpy data


Tuesday
-------

Git

 - how to create branches
 
 - pull request
 
 - merge branches
 
 - created exercise books
 
 
 
SSH

 - ssh-keygen to create a private key
 
 - ssh user@hostname to log in to another computer
 
 - scp file user@hostname:directory/filename to transfer files around
 
 - putting ```.ssh/id_rsa.pub``` (public key) into
   ```.ssh/authorized_keys``` so that you don't need a password
   
 - upload ssh keys to Github
 
 
 
PGP

 - why you can't trust github unverified commits
 
 - creating a pgp private key



CSV reading

 - Python csv library
 
 - pandas read_csv method
 
 - manipulate pandas DataFrames
 
 - [Notebook link](../../notebooks/reading-csv-files.ipynb)




Wednesday
---------


PGP

 - importing your public key to github
 
 - verified commits
 
 - the kinds of projects where people generally sign their commits
 
 
Crontab

 - how to schedule a job (such as ```git pull```) to run unattended

 - ```crontab -l``` to display the current cron jobs
 
 - ```crontab -e``` to edit the current cron jobs



Markdown

 - Why we have Markdown, and why it gets used instead of MS-Word
 
 - The syntax of Markdown
 
 - Converting Markdown documents to HTML
 
 - Using pandoc convert Markdown documents to all sorts of other formats
 
 
 
Simple pre-processing:

 - Creating an index for a dataframe and series during CSV import 
 
 - Parsing dates
 
 - Checking that imported data types are correct
 
 - Dealing with thousands separators and other annoyances
 
 - Counting the size of categories
 
 - Dealing with null and missing data
 
 - [notebook](simple-preprocessing-examples.ipynb)
 
 
 
Lab
 - Pick a dataset.
 
 - Present it, tell us something about it


Thursday
--------

Seaborn

 - Univariate charts: displot
 
 - Bivariate plots: jointplot (including kde), pairplot
 
 - Categoric plots: boxplot, violinplot, stripplot, countplot, pointplot
 
 - Linear regression plots: lmplot, residplot
 
 - (Students updated their notebook they created yesterday for presenting)



Tableau

 - installed, wrestled with license keys
 
 - watched video
 
 - short lab manipulating some sample datasets
 
 
 
Acquring HTML data

 - pandas.read_html to collect a table of populations from Wikipedia
 
 - [notebook](other-data-sources.ipynb)
 
 
 
Merging data

 - pandas.merge: inner and outer joins, what to merge on
 
 - how to clean up mismatches in datasets
 
 - brief introduction to regular expressions, including [ ] [^ ] * and .
 
 - [notebook](other-data-sources.ipynb)


Friday
------

Reviewed yesterday's final notebook. Detailed all the ways we can 
access a dataframe:

  df.ColumnName  - column as a series: can be assigned to
  df["ColumnName"]  - column as a series: can be assigned to
  df[0]  - first row

Indexing by a list of column names:

  df[["ColumnName"]] - return a 1-column dataframe view
  df[["Col1","Col2"]] - return a 2-column dataframe view
  
Indexing by a list (or array) of booleans:

  df[[True,False,False,True]] - return first and fourth rows
  df[df.Price > 10] - return rows that match the condition
  
How to select a cell so that you can update a value (assign to it):

  df.loc["RowIdx","ColIdx"] - the cell in the column called 
        "ColIdx" in the row which has an index of "RowIdx"
		
  df.loc["Row1":"Row2", "Col1":"Col2"] - cols from col1 through to col2
        of the rows that come after row1 and before row2 (including 
		row1, row2, col1 and col2 themselves)

  df.iloc[3,2] - same as loc, but using integer indexes: column 2 of row 3 


Web scraping:

 - wget
 
 - requests library
 
 - dealing with authenticated pages
 
 - parsing with BeautifulSoup
 
 - handling JSON files
 
 
Project time
