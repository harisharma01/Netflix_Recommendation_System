# Netflix Recommendation System
You may have noticed that YouTube suggests videos related to topics you have recently viewed. Similarly, e-commerce platforms suggest products based on your browsing and purchasing history. For instance, if you recently bought a mobile phone, you may be recommended phone accessories such as earphones and back covers. Online streaming services like Netflix, Amazon Prime Video, and Disney+ Hotstar also make recommendations based on your viewing history. For example, if you watched the comedy movie "Dumb and Dumber," you may be recommended "Dumb and Dumber 2" and other comedy movies or movies featuring Jim Carrey.

Customer Behaviour and it's prediction lies at the core of every Business Model. From Stock Exchange, e-Commerce and Automobile to even Presidential Elections, predictions serve a great purpose. Most of these predictions are based on the data available about a person's activity either online or in-person.

In today’s world OTT platform and Streaming Services have taken up a big chunk in the Retail and Entertainment industry. Organizations like Netflix, Amazon etc. analyse User Activity Pattern’s and suggest products that better suit the user needs and choices.

## Problem Statement
For the purpose of this Project we will be creating one such Recommendation Engine from the ground-up, where every single user, based on there area of interest and ratings, would be recommended a list of movies that are best suited for them using collaborative filtering.

Collaborative filtering employs the principle of identifying shared interests among similar users to make recommendations for new items. By analyzing the patterns of choices and preferences of like-minded individuals, it determines what suggestions to offer.

## Project Objective
Find out the list of most popular and liked genre
Create Model that finds the best suited Movie for one
user in every genre. 3. Find what Genre Movies have received the best and worst ratings based on User Rating

## Algorithm Used:SVD
Singular Value Decomposition (SVD) is a technique for factorizing a matrix into the product of three matrices: a unitary matrix, a diagonal matrix, and another unitary matrix. It is a generalization of the eigen decomposition of a normal matrix (for example, a symmetric matrix) to any matrix via an extension of eigen vectors and eigen values to singular vectors and singular values.

### Surprise library
The Surprise library is a Python library for building and analyzing recommender systems. It was developed by Nicolas Hug and is built on top of the scikit-learn library. The library provides a set of powerful and easy-to-use tools for building and evaluating recommender systems, including algorithms for collaborative filtering, matrix factorization, and neighborhood-based methods. The library provides several built-in datasets, as well as a way to easily load your own data. It also provide a variety of evaluation measures and cross-validation methods to evaluate the performance of the recommenders.

## Pearson correlation Method
The Pearson correlation method is a statistical technique used to measure the linear relationship between two continuous variables.

The Pearson correlation coefficient measures the linear association between two variables. It takes a value between -1 and 1, with -1 indicating a perfect negative linear relationship, 0 indicating no linear relationship, and 1 indicating a perfect positive linear relationship.

The Pearson correlation coefficient is calculated as the covariance of the two variables divided by the product of their standard deviations. The covariance is a measure of the degree to which two variables vary together, and the standard deviation is a measure of the dispersion of the data around the mean.

The Pearson correlation method is widely used in a variety of fields, including psychology, economics, and the social sciences, to quantify the linear relationship between variables. It is particularly useful when the relationship between the variables is expected to be linear, and can provide insights into the strength and direction of the relationship between the variables.

### Utility Matrix
A utility matrix, also known as a user-item matrix, is a matrix used in recommendation systems to represent the preferences or ratings of users for a set of items. Each row in the matrix represents a user, and each column represents an item. The entries in the matrix are the ratings that users have assigned to items.

For example, consider a movie recommendation system, where the items are movies and the users are people who have watched and rated the movies. The utility matrix would be a matrix with one row for each user, and one column for each movie. The entries in the matrix would be the ratings that each user has given to each movie.

The utility matrix is an important component of many recommendation systems, as it provides a compact representation of the preferences of users for a large number of items. Based on the entries in the matrix, recommendation algorithms can be applied to generate recommendations for individual users. For example, collaborative filtering algorithms use the similarities between users' ratings to generate recommendations, while matrix factorization algorithms factorize the utility matrix into lower-dimensional representations to identify latent features in the data that are predictive of users' ratings.

The utility matrix is also useful for evaluating the performance of recommendation algorithms, as it provides a ground truth for comparison with the recommendations generated by the algorithms.

## Data Description

Rating Dataset:

User_ID – Contains the separate keys for customer.
Rating – A section contains the user ratings for all the movies.
Movie_ID – Id given to each movie.

Movies Dataset:

Movie_ID – Contains the separate keys for each movie.
Year – Year in which movie was released.
Name – Name of the movie corresponding to the movie_ID
