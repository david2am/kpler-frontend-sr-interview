## Feature Specs

We propose you to write a simple app to render a list of
countries location and some vessel tracks and show them on a map.

The layout of this application is expected to be divided in 3 parts:

```
+------------------------------+
|   Controls: search, buttons  |
+------------------------------+
|                 |            |
|  Countries      |            |
|    List         |   Maps     |
|                 |            |
+------------------------------+
```

* one block wrapping controls (search, sort, ...)
* one block displaying filtered countries list
* one block wrapping the map

### List of countries

* As a user, I want to see a list of countries, each country should be 
  represented as a card
* Each country card should contain following information: country name, capital, 
  population, borders list
* Each country card should have a button to quickly focus the country on the 
   map

###  Maps

* A marker should be visible for each country on the maps
* When focusing on a country / marker, url must be updated
* vessels tracks should be displayed on the map

### Controls

* As a user, I want to be able to search/filter countries
* As a user, I want to be able to sort countries by alphabetical order or by 
  population
* As a user, I want to be able to compute average population of all the 
  countries of the filtered list
* Average population and markers displayed on the map must be updated when list 
  of countries is updated

## Data

You can fetch data from this [REST Countries API](https://restcountries.com/).  
Use the [vessel positions dataset][1] (vessel_id, latitude, longitude, position_time) to create the tracks.

[1]: https://kpler.github.io/kp-recruitment/e0e0648191289bb0cf43090d052121c58f0af8f5/data-fs-exercise.csv
