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
 
Lab
 - Pick a dataset.
 - Present it, tell us something about it


