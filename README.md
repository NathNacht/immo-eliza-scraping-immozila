# immozilla
[![forthebadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

##  Description
This Python project employs web scraping techniques to compile a dataset of real estate properties in Belgium. Specifically, we utilized Immoweb to gather information on 10,000 houses and apartments available for sale across the country.

The outcome of this project provides us with the following headers in our files:

* Property ID
* Locality name
* Postal code
* Price
* Type of property (house or apartment)
* Subtype of property (bungalow, chalet, mansion, ...)
* Type of sale (note: exclude life sales)
* Number of rooms
* Living area (area in m²)
* Equipped kitchen (0/1)
* Furnished (0/1)
* Open fire (0/1)
* Terrace (area in m² or null if no terrace)
* Garden (area in m² or null if no garden)
* Surface of good
* Number of facades
* Swimming pool (0/1)
* State of building (new, to be renovated, ...)


##  Installation

* clone the repo
* Install all the libraries in requirements.txt

```bash
$ python3 main.py
```

* everything wil be stored in ./data/csvdump.csv. 

##  Workflow

### main
```mermaid
graph TD;
    A["multiWeblinks()"]-->B[Will be stored in weblinks];
    B-->C["PropertyScraper(url)"]-->D[Will be stored in scrape_url];
    D-->E["scrape_url.scrape_property_info()"];
    E-->F["to_csv() "];
```

##  Usage

## Visuals

##  Contributors

##  Timeline