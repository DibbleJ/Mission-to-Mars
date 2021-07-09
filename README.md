# Mission-to-Mars

# Overview
  The purpose of this analysis is to collect information about Mars, store it in a mongo database, and display it for other in a Flask app. The information is collected from a number of different sites listed below:
  - Mars News is from https://redplanetscience.com/.
  - The Featured Image is from https://spaceimages-mars.com.
  - The Mars Facts are from https://galaxyfacts-mars.com.
  - The Hemisphere pictures and names are from https://marshemispheres.com/.
# Results
  The webpage that has been put together incorporates html, python, mongo, and Flask to create a site that can update information from multiple sources at the click of a button. The html is styled using Bootstrap to allow for simple, clean design.
# Summary
  The button initiates the Flask /scrape route, which in turn executes scraping.py. The scraping.py program uses BeautifulSoup and Splinter to travel to each website and collect the necessary information by parsing through the html tags and classes. Once all of the data has been collected in the scraping.py program, it is returned to the Flask app, and the mars mongo db is updated.
