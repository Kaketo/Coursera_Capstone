# Data
To answer to the business question: *Where is the best spot to open new restaurant/bar/... in Warsaw, Poland?*, I will use followoing data:
- List of neighborhoods in Warsaw, Poland with their geolocation (*geojson file*).
- Venue data, data related to any gastroniomic businesses in Warsaw, Poland.
- Data about number of residents in each neighborhood in Warsaw, Poland.

### Sources of data and methods to extract them
At the begining, I will use various methods for web scrapping to collect list of neighborhoods with multiple informations.
Very good dataset containing all polygons of Warsaw neighborhood could be found here:
https://github.com/andilabs/warszawa-dzielnice-geojson/blob/master/warszawa-dzielnice.geojson
I download the *geojson* file and transform it into wanted format. Then I will use the Wikipedia website:
https://pl.wikipedia.org/wiki/Podzia%C5%82_administracyjny_Warszawy
To get all necessary information about residents.

After that, I will use Foursquare API to get venues data for whole city. Foursquare has one of the largest database of 105+ milion places and its use worldwide by multiple companies. Foursquare API will probide information about latitute and longtitude of venues, but also category and name.