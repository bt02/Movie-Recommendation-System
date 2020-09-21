# Movie-Recommendation-System
## Objective and data:
Creation of movie recommendation system while also modifying it to hand the cold start problem. The data used for building the system comes from MovieLens utilizing their small data set containing 100,000 ratings and 3,600 tag applications applied to 9,000 movies by 600 users. 

## Recommendation system: 
![Imgur](https://i.imgur.com/U2HsYnL.png)

The recommendation system uses collaborative filtering to match similar users together . 11 different models were tested to find the best fit. The Baseline Only algorithm was chosen due to it relatively low root mean squared error (RMSE) and low run times. With any recommendation system the problem of the cold start is an issue: How to handle new users with no data. Two solutions are proposed as to how this system will handle it.


### Cold Start: Solution 1:
![Imgur](https://i.imgur.com/byHSSzM.png)

The first solution to the cold start problems is to have new users answer a questionnaire about movies that they have seen. The user ranks the presented movies to allow for the system to have a basis to build off initially
* Ex: “How do you rate this movie on a scales of 1-5”
The result of the questions would output the top 5 recommendation based on the users input 

### Cold Start Solution 2:
![Imgur](https://i.imgur.com/yDhlKFq.png)

The second solution is to display a general list of movies that have a high number of ratings along with a high average movie rating. This will act as a general list of most liked movies. A variation of this option is to adjust the general recommendation with any user data present. 
*	Ex: Gender and or Age

Once this data is received the model would output recommendations that a typical male or female would like would simultaneously adjusting the release dates of the movies so that only title made in the users lifespan are shown for more familiarity.

## Best decade for movies: 
![Imgur](https://i.imgur.com/UdyoCfc.png)

The best decade for movies was from the 1920’s to the 1960’s with and average movie rating of a 3.7. This come with surprise as the top 5 best movies of all time made in the 90’s. Relative to the other decades the 90’s was a particularly low time for movies comparative to the other decades. The overall change in ratings is not significant, but it raises curiosity if the 90’s managed to produce successful movies but not consistently enough to be a high performing decade.

## Distribution of Reviews:
![Imgur](https://i.imgur.com/76CV4vu.png)

16.9% of movies have 1 review for them while 70.3% of movies having less than 10 reviews. The recommendation system runs into the issue of not enough users consistently rating movies. This can play a role in how the movies are displayed to the user if not enough data on the movies is present. It can allow for the bias of a single individual to skew the opinion of the movie.

##  Ratings and Reviews:
![Imgur](https://i.imgur.com/D1Q68mo.png)

Most movies are rated between 3 & 4 on average. Movies that have achieved an average rating of 5 typically only have 1-5 reviews. Many of the movies cannot maintain a 5-star rating as their view count goes up. There is a cycle were movies with low ratings don’t get any new viewers, so their ratings stay low, while highly rated moves get more reviews because of their rating. 

## Recommendations:
1. Try and increase the number of reviews users give
2. Don’t display the rating of the movie until it has at least 10 reviews to try and remove user bias
3. Collect as much data about the user as possible to personalize recommendations

## Future Work
1. Use the large data set for an improved model
2. Update the files with movies and ratings of the current year
3. Have an outside source like Rotten Tomatoes ratings available as a comparison against the individual opinion

