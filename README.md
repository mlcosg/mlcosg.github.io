# mlcosg.github.io

## About the Project
Hello! My name is Marcia and this website is the *first* website I have ever made! And it was coded "from scratch," 
meaning I coded all of the HTML and CSS myself! This website is in fulfilment of the "Web Design Challenge" requirements 
for the UCD Data Visualization certification course I am currently taken. In other words, this website is my homework assignment!

Additionally, the content for this website is pulled from my first project for the same course, which was a semi-collaborative 
group effort. My group decided to examine publically available data from the National UFO Reporting Center, which we downloaded 
from Kaggle.com. We collaboratively cleaned and transformed most of the data together, then chose our own analytic topics to pursue. 
This website summarizes my analysis of the UFO data!

I was mostly interested in examining trends over time and was curious whether certain sightings of objects might have greater 
reliability over others, and if so, then it's likely we should see some kind of pattern in those sightings over time.

For this analysis I looked at how long objects were sighted for (duration in seconds) by the shape of the object over time. 
I started by looking at the average duration of sightings by shape (i.e. the means and errors) for observations reported between 
2000 and 2014. I also looked at the average duration of sightings by shape for observations by day of week. I was curious to see 
if there were any decernable patterns by day of week. I finish the analysis by looking at some correlations.

## About the Data
The data used in this project is compiled and published by the National UFO Reporting Center (NUFORC) on UFO sightings. The initial dataset was greater than 80k observations and reported on sightings back to the 1960s. After the initial data cleaning and group decisions about the data were made, the dataset the group worked with for our individual analyses was 56k observations. We included only more recent observations (2000-2014), and looked at data on time, location (latitude/longitude), object shape, and duration of sighting.

About the Shapes Category:
During the initial group cleaning of the data, we coded the shape category using the following meta-schema:

"No Shape Provided" = blank, unknown, other <br>
"Geometric" = triangle, delta, circle, sphere, round, dome, rectangle, cylinder, cone, pyramid, hexagon <br>
"Light" = light, fireball, flare, flash <br>
"Changing" = changed, changing <br>
"Disk" = disk, oval, cigar <br>
"Teardrop" - teardrop, egg <br>
"Formation" = formation of multiple objects <br>
"Miscellaneous" = diamond, chevron, cross, crescent <br>

Further Cleaning of the Data for the Analysis:
I further limited the scope of my individual analysis by dropping all observations of durations in sightings greater than 5 hours. (For a discussion on this, see “Comparisons-Outliers” under the Comparisons dropdown menu option.)

Since my analysis was looking at duration of sightings by object shape over time, I further limited the dataset I looked at by excluding the shape categories “changing” and “no shape provided."

Changing Shape Category - The “changing shape” category showed more variation in general (larger errors) than the other shape categories, and because the notes field provided for that category show more variation in general in how people described what they saw, I decided it would be better to examine the other categories in more detail since they were more consistent in what the observer claimed to be seeing.

No Shape Provided Category - In line with this logic, I also decided to further narrow the dataset and exclude "no shape provided" as well. However, I decided to keep the "miscellaneous" category since that category was compiled of a subset of shapes (chevron, diamond, cross) where observers were more certain about what they saw.

Observations in 2014 - I also dropped the observations for the year 2014 since this was an incomplete year in the dataset. The only observations included in my analysis have occurred between 1/1/2000 and 12/31/2013.

* Group Dataset was 56,739 observations (starting point for this analysis)
* Number reduced 288 observations after dropping sightings greater than 5 hours long
* Number reduced 1,482 observations after dropping the "changing" category
* Number reduced 7,947 observations after dropping the "no shape provided" category
* Number reduced 1,693 observations after dropping observations made in 2014
* Total Observations = 45,329

