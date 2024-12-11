# AON_Scraper
## description  
the AON_Scrapper consists of 3 parts.  
### the scraper  
the aonScraper.ipynb file describes the use of pythons response library to scrape html information from the website, [archives of nethys](https://2e.aonprd.com/) and compiles it into a file monsterdeets.txt which links monsterids to a block of pertinant raw html data. 
### the parser  
the dataparser.ipynb file takes that raw html data, and parses it into the corpusData.csv which contains the data we need for our searching.  
## the seacher
the bm25Searcher.ipynb file uses the csv file the parser generated to create a document corpus, which the bm25 algorythm can then use to search for monsters.
## Extra, the Gui
for testing I have created a simple webapp hosted through anvil. using this [link](https://colorful-thorough-auk.anvil.app/) the server in the bm25searcher code needs to be running for the web app to work.  
run the `anvil.server.wait_forever()` line and it should work

