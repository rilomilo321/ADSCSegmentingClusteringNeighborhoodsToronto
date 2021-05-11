# ADSCSegmentingClusteringNeighborhoodsToronto


{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Coursera Data Science Capstone Final Project"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    " ### Introduction/Business Problem: \n",
    " \n",
    " 1.1 Background\n",
    "Metro Vancouver is a Canadian political subdivision and corporate entity representing the metropolitan area of Greater Vancouver. It consists of 21 municipalities. In the 2016 Census of Population conducted by Statistics Canada, the Metro Vancouver Regional District recorded a population of 2,463,431, making it the regional district in British Columbia with the greatest population and population density.\n",
    "\n",
    "\n",
    "1.2 Problem\n",
    "The aim of this project is to investigate the features of different cities in Metro Vancouver Area. Also, the project clusters the area into 5 clusters and explore the rank of popular venues in each cluster.\n",
    "\n",
    "\n",
    "1.3 Interest\n",
    "Since different cities in Metro Vancouver area has its unique characteristics, the project would be interesting to people who are potential travellers or residents. Since they are able to make a decision on which ares to explore based on their own preferences.\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Data\n",
    "\n",
    "The postal codes for all British Columbian cities are scraped from wiki page (title: List of postal codes of Canada: V, website: https:// en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_V.) \n",
    "\n",
    "The data was filtered based on the scope of cities included under Metro Vancouver Area umbrella. The city list can be found at Metro Vancouver official website. \n",
    "\n",
    "The latitude and longitude of each city is retrieved using Python pgeocode\n",
    "library. \n",
    "\n",
    "The venues explored within each city is implemented using foursquare API."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "#### Analyzing the features of each city in Metro Vancouver Area\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 391,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Requirement already satisfied: beautifulsoup4 in ./opt/anaconda3/lib/python3.8/site-packages (4.9.3)\n",
      "Requirement already satisfied: soupsieve>1.2; python_version >= \"3.0\" in ./opt/anaconda3/lib/python3.8/site-packages (from beautifulsoup4) (2.0.1)\n",
      "Requirement already satisfied: lxml in ./opt/anaconda3/lib/python3.8/site-packages (4.6.1)\n",
      "Requirement already satisfied: geopy in ./opt/anaconda3/lib/python3.8/site-packages (2.1.0)\n",
      "Requirement already satisfied: geographiclib<2,>=1.49 in ./opt/anaconda3/lib/python3.8/site-packages (from geopy) (1.50)\n",
      "Folium installed\n",
      "Libraries imported.\n"
     ]
    }
   ]
