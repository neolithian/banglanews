# banglanews

This is a python package to get the textual content from online Bengali newspapers. The objective of this package is to get Bengali text mainly for the data scientists who need Bengali textual content for research purpose. This package was created for academic AND non-commercial use ONLY. The author of this package does not encourage OR suggest to use this application for anything other than academic research or experimental works.

# How to install<br>

The easiest way to install it from a Python 3 environment using the following command:<br>

<code>pip install banglanews</code><br>

Alternatively, you can download the package <b><a href=https://github.com/neolithian/banglanews/blob/main/banglanews-0.0.2.tar.gz>banglanews-0.0.2.tar.gz</a></b> and put it in a directory. From any Python 3 environment open a terminal, go to that directory where you put the package and install the package using the following command:<br>

<code>pip install banglanews-0.0.1.tar.gz</code><br>

# How to use it in the code

Right now the package only supports the leading Bengali newspaper 'Prothom Alo'. Include the module in your code like below:<br>

<code>from banglanews import prothomalo</code><br>

# Initializing the class

The package contains one single class named <code>scraper</code>. This is how you need to initialize it:<br>

<code>objScraper = prothomalo.scraper('2021-12-01','2021-12-05','D:\\\Content')</code><br>

1st argument: <code>start_date</code> = The date you want the scraper to start with.<br> 
2nd argument: <code>end_date</code> = the end date of getting the content.<br> 
3rd argument: <code>output_dir</code> = The file system location where you want to dump the content.<br><br>

Please note, all three arguments are mandatory. Also note, the dates must be in the YYYY-MM-DD format.

# Important methods:<br>

<code>PrintContents</code> :   Prints individual articles in text files in the file system<br>
<code>PrintURLs</code> :       Prints the Headlines and URLs in a single <i>pipe delimitted</i> csv file in the file system<br>
<code>PrintComments</code> :   Prints the Headlines, URLS and Comments in a single <i>pipe delimitted</i> csv file in the file system<br>

# A sample call<br>

1st argument (optional): <code>search_text</code> = The text that you want to be searched. If you do not pass any value, all the URLs in between <code>start_date</code> and <code>end_date</code> will be searched.<br>

<code>objScraper.PrintURLs('করোনা')</code><br>

The above call will create a .csv file in the <code>output_dir</code> location provided in the class initialization. 

# Version information<br>

Latest version: 0.0.2<br>
Previous versions:




