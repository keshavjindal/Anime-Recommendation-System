# Anime Recommendation System
In this repository, we have tried to build some **Recommendation Systems** to get **Anime Recommendations**. We have built three Recommendation Systems and applied them on the Dataset given **[here](https://www.kaggle.com/CooperUnion/anime-recommendations-database)**. The Dataset contains two files namely : **anime.csv** and **rating.csv**.

**`anime`** Dataset contains following attributes:
* `anime_id` : ID given to each Anime.
* `name` : Name of the Anime.
* `genre` : List of Genres relating to given anime.
* `type` : Type of Anime i.e whether it is a Movie, TV show etc.
* `episodes` : Number of Episodes produced for a anime.
* `rating` : Average Rating given to the Anime.
* `members` : Number of people that have watched the Anime.

**`rating`** Dataset contains following attributes:
* `user_id` : ID given to each User
* `anime_id` : Same as in anime file
* `rating` : Rating given by user to a particular Anime.

Three *Recommendation Systems* built are:
* **Demographic Filtering**: It is a very elementary recommendation system that provides recommendations based on the popularity and the *wighted rating* of the show.
* **Content-Based Filtering**: It is a decent recommendation system that uses the genres of the input show, and tries to recommend shows with similar genres. This Filtering is implemented using two namely : *CountVectorizer* and *TfidfVectorizer*.
* **Collaborative Filtering**: It is a good recommendation system that considers the rating given by users and the similarity between user-user and show-show to get the recommendations based on the input list of animes and their corresponding ratings. This Filtering is implemented using *Pearson's Correlation*.
