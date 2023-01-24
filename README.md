## Web Scraping.
The goal was to perform collection of data (textual data deprived from email links, the links itself and date).
The emails are organized by date. Each link under “Scam emails by date:” points to another page with many links. Most of these links are references to an email page. The script returns a table of links (link text, url, day ) for 3 months of data (I chose the volume). The links are collected that lead to a list of emails and ignore the others. The script gatheres and processes all the email links from each of the pages.

Web Scraping was performed based on the https://www.419scam.org site by using diverse libriries and packages such as: BeautifulSoup, Urllib , Requests, Pandas. 

Web scraping is the process of collecting and parsing raw data from the Web.
There are several steps that should be considered before performing the Web Scrapping.

## Scrutinizing the Website
To reach a web server we send an HTTP request (query) to the server of the page we want to scrape. The server responds by sending the HTML content of the web page. Since we use Python for our requests, we need a third-party HTTP library, and we will use Requests.
## Decipher the Information in URLs
The base URL represents the path to the search functionality of the website. We have parameters that are in the format of a key-value pair.
Query parameters are defined set of parameters attached to the end of a url. They are expansions of the URL that are used to aid figure out specific content or actions based on the data being passed.
Origin: The beginning of the query parameters is denoted by a question mark (?). 
Content: The pieces of information of a query parameter are enclosed in key-value pairs, keys and values are joined together by an equal sign (key=value).
Divider: Every URL might have multiple query parameters, which are separated from each other by an ampersand (&) in between each. These can be created by any variation of object types or lengths such as String, Arrays and Numbers.

## Pandas -
This library is for keeping the records of our  scrapped  in the form of tables (CSV)
## BeautifulSoup - The link for installation - https://beautiful-soup-4.readthedocs.io/en/latest/
This library is for searching through the HTML  in  code  an organized and  simple way.
## Requests - 
This library is for sending HTTP requests and  the HTML data from the target web
pages to obtain the information we are looking for.
