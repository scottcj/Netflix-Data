## Tyler's Page
Interest: I am interested in comparing the rating between genres of shows and movies on netflix

Data issues encountered: Our current dataset of netflix shows and movies currently contains a lot of information about the shows and movies on netflix however, it doesn't include the ratings the show/movies recieved. To attempt to gain access to the ratings I tried to use another dataset from IMDB and try and merge the data onto our current dataset to add ratings. However after furthur manipulation with the different datasets on IMDB I quickly came to the conclusion that the datasets were not only very impractical to use but the data doesn't seem to be accurate. Another issue with our datasets is that many of the foreign titles in our datasets seem to have their titles mistaken and their titles were entered using the wrong syntax. Another problem I came across is that the movies and tv-shows overlap on a lot of the rating when they shouldn't be overlapping. I think this is due to netflix having innconsistent identification on what's a tv show and wha't a movie.

### Netflix visualization
{% include_relative Visualization/test.html %}
{% include_relative Visualization/tvshows.html %}
{% include_relative Visualization/movies.html %}



