# Recommendation System
This project uses a database from IBM Watson Studio platform, which is composed of users, articles about data science, and interactions between these two elements. The goal is to make a recommendation system, which recommends an article for a user in the database, based on the interactions with articles of a user.

## Files

Recomendations_with_IBM.ipynb: Main file with the algorithms designed to the solution.
project_tests.py: File with all main needed tests to be executed testing the outputs presented in the file above.

The other four files with extension .p are files used in the test file above.

## Recommendation approaches

### Rank-Based Recommendations

This approach is used to recommend the most popular articles. Popular in this case is a measure of the interaction amount received by the users, since we don't have ratings.

### User-User Based Collaborative Filtering

Given the users and its interactions, it’s possible to calculate the similarity between two users, which will give us the users that interacted with some of the same articles of a given user. 
The difference between the interacted articles by similar users and interacted articles by this first user will give us it's possible articles this user would like to interact with.

### Content Based Recommendations

One of the datasets is all about the articles. This dataset provides information about the name of the article, the body and the summary. From this information it’s possible to use the words of this text as tokens using TF-IDF representation to create this way a matrix with all possible tokens inserted in the article summary for example, to find this way the similarity between each article.

### Matrix Factorization

Using the Single Value Decomposition (SVD), it was possible to decompose the matrix of user-item interactions, which results can be understood as features of the articles required to users to interact with some article or not.

## License

Copyright 2020 Thiago Lima
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
From opensource.org
