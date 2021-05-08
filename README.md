# Content Based Movie Recommendation System with Sentiment Analysis

Based on the users search query, content based movie recommendation system will recommend similar movies based on the likes and sentiments on the reviews of the searched movie.

Details of a movie like the title, genere, runtime, rating, poster are extracted from TMDB using the API key generated from TMDB. Based on the IMDB ID of the movie in the API, reviews are scrapped using the `beautifulsoup4` library and sentiment analysis for those reviews are performed.

## How to run the project?

1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the [requirements.txt] (`pip install -r requirements.txt`).
3. Get your unique API key (https://www.themoviedb.org/) and replace the key in two places of the `static/recommend.js` file.
4. Once it's done, open the terminal and run `main.py`. Then open the browser and type `http://127.0.0.1:5000/` in the address bar.

### Dataset Sources 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)
6. [List of movies in 2021](https://en.wikipedia.org/wiki/List_of_American_films_of_2021)

