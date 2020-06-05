# Recommendation System

Using real data on users and articles from IBM Watson Studio Platform, we build a recommendation system using Rank-based recommendations and Filtering, User-User Collaborative Filtering, and Singular Value Decomposition Matrix Factorization.

Rank-based recommendations and Filtering are useful for users or articles without sufficient data. This problem typically arise for new users. This is referred to as the Cold Start Problem, which occurs when it is difficult to recommend similar users and articles because not much is known about the user or article. Filtering is also particularly useful if a user has a very specific criteria for an article.

User-User Collaborative Filtering are useful if there is an active community of users or selection of articles in which recommendations can be made from the similarity of users activity history, such as the number of times an article is read by similar users. This is particularly useful when paired with a rating system.

Singular Value Decomposition (SVD) Matrix Factorization are useful in recommending based on the some important unknown latent features of articles. The decomposition tends to give good recommendations to users if a few latent features (in a diagonal latent features matrix) can explains most of the variability in user preferences. However, SVD requires that there are no missing data in the user-article interactions matrix. A workaround to circumvent this is FunkSVD, which employs a gradient descent algorithm to approach an optimal latent features matrix.

Further improvements can be made using Content-based recommendations such as Natural Language Processing to categorize Bag-of-Words in the article.

## Installations
```
pip3 install -r requirements.txt
```
* numpy
* pandas
* matplotlib
* seaborn
* pickle

## Licensing, Authors, and Acknowledgements

[MIT License](https://github.com/jasonho0810/recommendation-system/blob/master/LICENSE)