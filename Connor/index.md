## Connor's Page

#### Interest

I am interested in comparing the age ratings of movies or tv shows between different countries from the dataframe. I think it could be interesting seeing what audiences netflix has catered to in different countries.

### Netflix Visualizations


{% include_relative visualizations/netflixUSMovies.html %}


I decided to try and merge the IMDB database into the Netflix one and upon graphing some of the IMDB data something seemed off.


{% include_relative visualizations/IMDBVotes.html %}
This visualzation is using the numVotes column that contains the number of ratings that the movie got to give is score, as you can see no matter how im cutting the data there is a big cluster of movies with a low number of votes.

I thought this was a bit wierd so I took a sample of 5 movies from the dataframe and found that only 1 or 2 of these 5 ever lined up with what the IMDB website had for the rating. Based on my samples, the IMDB dataset must not be updated very frequently or there is some problem with their system. Not being able to look at these ratings is annoying but it was goot practice to check if 
a dataset is correct or not.

### COMING SOON...
I intend on doing a visualization that compares the different countries that netflix provides movies to based on what rating movies and shows they receive.

{% include_relative visualizations/RatingsPieChart.html %}