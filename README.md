# ADSCSegmentingClusteringNeighborhoodsToronto


## Coursera Data Science Capstone Final Project"

### Introduction/Business Problem:

1.1 Background Metro Vancouver is a Canadian political subdivision and corporate entity representing the metropolitan area of Greater Vancouver. It consists of 21 municipalities. In the 2016 Census of Population conducted by Statistics Canada, the Metro Vancouver Regional District recorded a population of 2,463,431, making it the regional district in British Columbia with the greatest population and population density.

1.2 Problem The aim of this project is to investigate the features of different cities in Metro Vancouver Area. Also, the project clusters the area into 5 clusters and explore the rank of popular venues in each cluster.

1.3 Interest Since different cities in Metro Vancouver area has its unique characteristics, the project would be interesting to people who are potential travellers or residents. Since they are able to make a decision on which ares to explore based on their own preferences.

###Data

The postal codes for all British Columbian cities are scraped from wiki page (title: List of postal codes of Canada: V, website: https:// en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_V.)

The data was filtered based on the scope of cities included under Metro Vancouver Area umbrella. The city list can be found at Metro Vancouver official website.

The latitude and longitude of each city is retrieved using Python pgeocode library.

The venues explored within each city is implemented using foursquare API.

