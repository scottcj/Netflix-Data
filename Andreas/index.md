## Andreas's Page

Interest: I'd be interested in comparing the amount of releases of each genre between different countries. I would also be interested in looking at the frequency of certain key words in the descriptions of the movies and tv shows.

### Netflix visualization

Here is a plotly visualization of the frequency of certain ratings of TV shows and Movies on Netflix.

{% include_relative plotly/netflix-ratings.html %}

Below is a visualization of the average movie/tv show ratings from the countries with the most content on Netflix.

{% include_relative plotly/country-ratings.html %}

This graph was made after merging the Netflix data with the IMDB datasets which included the ratings. As we can see, it appears that the UK and South Korea have a slightly better average tv show/movie ratings on their Netflix, followed by USA, India, and Canada. All the average ratings are pretty close, so the range on the y-axis was changed to show the differences better. 

I had some difficulties merging the Netflix and IMDB datasets, since the merged data set includes many more rows than the Netflix data. This means that there may be duplicates of movies or tv shows or perhaps some of the content in the IMDB was added to the Netflix dataset. I only want to include the movies and tv shows in the Netflix dataset so I will need to clean the data to get rid of any unwanted additions. 

When looking at word frequencies in the descriptions of the movies and tv shows, I had troubles with converting the data type. First the descriptions had to be converted from an object to a string. However, plotting string values brings up complications which I will need to look further into to be able to plot specific word frequencies and to eliminate insignificant words such as prepositions and conjunctions. 


### Next up...
Next I would like to create a word map of the descriptions of the tv shows and movies to see which key terms are used most often. From there, I would like to compare the ratings of movies/tv shows that contain the given key words in their description to see whether some topics/themes are generally rated higher than others. 
