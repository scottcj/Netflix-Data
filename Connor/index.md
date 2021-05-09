## Connor's Page

#### Interest

I am interested in comparing the age ratings of movies or tv shows between different countries from the dataframe. I think it could be interesting seeing what audiences netflix has catered to in different countries.

### Netflix Visualizations


{% include_relative visualizations/netflixUSMovies.html %}

### Deciphering the IMDB dataset

I decided to try and merge the IMDB database into the Netflix one and upon graphing some of the IMDB data something seemed off.


{% include_relative visualizations/IMDBVotes.html %}

This visualzation is using the numVotes column that contains the number of ratings that the movie got to give is score, as you can see no matter how im cutting the data there is a big cluster of movies with a low number of votes.

I thought this was a bit wierd so I took a sample of 5 movies from the dataframe and found that only 1 or 2 of these 5 ever lined up with what the IMDB website had for the rating. Based on my samples, the IMDB dataset must not be updated very frequently or there is some problem with their system. Not being able to look at these ratings is annoying but it was good practice to check if 
a dataset is correct or not.

### Comparing Different countires rating distributions

As stated in my interest section I wanted to compare the ratings of movies and tv shows released in different countries to allow a conclusion to be drawn about what demographic netflix caters to and if it changes depending on what country you watch from.
The first step was to create a pie chart based on the entire dataframe so that you can compare the pie charts for individual contries with a baseline. Then I was able to plot the rest of the individual countries that I want to look at and compare between them and the baseline.

### Baseline
{% include_relative visualizations/BaselinePieChart.html %}
### By Country
{% include_relative visualizations/RatingsPieChart.html %}