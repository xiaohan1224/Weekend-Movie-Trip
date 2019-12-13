## Weekend Movie Trip

## MovieLens Dataset Classification

Resource: https://grouplens.org/datasets/movielens/

The dataset contains, comments towards different movies from various users, movie ids, ratings and etc. 
The movie genres in this dataset are:
	- Action
	- Adventure
	- Animation
	- Children's
	- Comedy
	- Crime
	- Documentary
	- Drama
	- Fantasy
	- Film-Noir
	- Horror
	- Musical
	- Mystery
	- Romance
	- Sci-Fi
	- Thriller
	- War
	- Western
	- (no genres listed)

## Purpose:
   To determine similar movies using ratings and tags. 

## Main steps:
   1. Data Prepartion: 
       * a) Genres is transformed as a onehot nuermic array
       * b) Column title is seperated into year and and tile (Movie name)
       * c) Label Encoder is used to transform tag
   2. Visualzie tags to the same movie using WordCloud  
   3. Feature correlation
   4. MeanShift and Kmenas cluser models are applied

## Result:
The result is appealing, based on, genres, tags and few movies that i watched, the movies with similar genres and tags are clustered pretty well, based on the result shown above. Most of the clusters created by these two modeled overlapped pretty well. The difference is caused by the different algorithms of the two models, which makes sense. Overall, using tag and rating as feature is valid for solving this clustering problem.

## Project Structure

```bash

.
├── notebooks 
│     └── Weekend_Movie_Trip.ipyb
├── README.md
└── data
      ├── links.csv
      ├── tags.csv
      ├── movies.csv
      └── README.txt
```
