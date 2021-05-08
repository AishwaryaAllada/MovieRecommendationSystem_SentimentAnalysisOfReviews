# Content Based Movie Recommendation System with Sentiment Analysis

Based on the users search query, content based movie recommendation system will recommend similar movies based on the likes and sentiments on the reviews of the searched movie.

Details of a movie like the title, genere, runtime, rating, poster are extracted from TMDB using the API key generated from TMDB. Based on the IMDB ID of the movie in the API, reviews are scrapped using the `beautifulsoup4` library and sentiment analysis for those reviews are performed.

## How to run the project?

1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the [requirements.txt] (`pip install -r requirements.txt`).
3. Get your unique API key (https://www.themoviedb.org/) and replace the key in two places of the `static/recommend.js` file.
4. Once it's done, open the terminal and run `main.py`. Then open the browser and type `http://127.0.0.1:5000/` in the address bar.

## Architecture

![IMG-20210306-WA0012](https://user-images.githubusercontent.com/36665975/110212434-597bb700-7ec1-11eb-9ffa-7ac319e33123.jpg)

## Similarity Score : 

   How does it decide which item is most similar to the item user likes? Here we use the similarity scores.
   
   It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
   
## How Cosine Similarity works?
  Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.
  
  ![image](https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png)

  
More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)

### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

