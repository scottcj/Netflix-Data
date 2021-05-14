## Andreas's Page

Interest: I'd be interested in comparing the amount of releases of each genre between different countries. I would also be interested in looking at the frequency of certain key words in the descriptions of the movies and tv shows.

### Netflix visualization

Here is a plotly visualization of the frequency of certain ratings of TV shows and Movies on Netflix.

{% include_relative plotly/netflix-ratings.html %}

Below is a visualization of the average movie/tv show ratings from the countries with the most content on Netflix.

{% include_relative plotly/country-ratings.html %}

This graph was made after merging the Netflix data with the IMDB datasets which included the ratings. The countries shown are those with the most content on Netflix. As we can see, it appears that the UK and South Korea have a slightly better average tv show/movie ratings on their Netflix, followed by USA, India, and Canada. All the average ratings are pretty close.

I had some difficulties merging the Netflix and IMDB datasets, since the merged data set includes many more rows than the Netflix data. This means that there may be duplicates of movies or tv shows or perhaps some of the content in the IMDB was added to the Netflix dataset. I only want to include the movies and tv shows in the Netflix dataset so I will need to clean the data to get rid of any unwanted additions. 

When looking at word frequencies in the descriptions of the movies and tv shows, I had troubles with converting the data type. First the descriptions had to be converted from an object to a string. However, plotting string values brings up complications which I will need to look further into to be able to plot specific word frequencies and to eliminate insignificant words such as prepositions and conjunctions. 


### Comparing descritpions of Netflix movies/tv shows based on release year

Since it was very difficult to accurately merge the IMDB datasets with the Netflix data set, I decided to leave the movie and tv shows ratings out and just focus on the Netflix dataset. Instead, I decided to look at the descriptions of the movies and tv shows on Netflix. I thought it would be interesting to see what the most commonly used words were in the descriptions and compare the most common words based on the release year of the movie or show. 

To accomplish this, I just used the description column from the Netflix dataset and the release year of the movies and tv shows. First I separated the Netflix content by release year, then combined the descriptions of movies and shows by release year. I focused on the last 4 years (2020-2017) since those were the years with the most content on Netflix. Then I converted all capitals to lower case letters so that all the words would read the same. I also removed any punctuation and non-descriptive words, such as prepositions, pronouns, and conjunctions (e.g., what, a, the, his, them, from, etc.). I was mainly interested to see what the most popular nouns and adjectives were. Then I used a function that counted the frequency of each word in the descriptions. After this, I was able to plot the most common word descritors of movies and tv shows based on what year they were released. 

Below is an example of the most common words used in the descriptions of movies and shows released in 2020 that are on Netflix. 

{% include_relative plotly/2020_word_freq.html %}

I wanted to compare what the most common words were in the descritions by release year. I used the last 4 years, 2020-2017, because Netflix had the most content from movies and shows released those years. I plotted them together on the same bar graph and the result is shown below. 

<img width="860" alt="Screen Shot 2021-05-13 at 8 25 57 PM" src="https://user-images.githubusercontent.com/66276355/118217003-74baf380-b429-11eb-873e-f336b40accb7.png">

I was having troubles saving this graph as an html so I had to upload it as a static image instead, as opposed to the live html bar graph shown previously. As we can see from this graph, the most commmon word used the descriptions for most the movies and shows released the past four years is "life". Other commonly used words were "family", "new", and "young". I was also surprised to see that "school" was a common topic in movies and shows released in 2020, perhaps due to the covid pandemic and school experiences changing to such a dramatic extent. I also noticed that "man" was mentioned more in the descriptions compared to "woman" for each release year, indicating that the movie industry is still male dominated. 

As an additional visualization, I created a wordcloud of the most common words used in the descriptions of movies and shows released in 2020 on the United States Netflix. I made the wordcloud into the shape of the Netflix logo. 

<img width="864" alt="Screen Shot 2021-05-13 at 4 40 30 PM" src="https://user-images.githubusercontent.com/66276355/118218046-8604ff80-b42b-11eb-8dbf-99cda159c399.png">
