# [Investigating-Netflix-Movies-and-Guest-Stars-in-The-Office](https://app.datacamp.com/learn/projects/entertainment-data)
Apply the foundational Python skills by manipulating and visualizing movie and TV data.


--------

## 📌 Project Description
In this project, you’ll apply the skills you learned in [Introduction to Python](https://app.datacamp.com/learn/courses/intro-to-python-for-data-science) and [Intermediate Python](https://app.datacamp.com/learn/courses/intermediate-python) to solve a real-world data science problem. You’ll press “watch next episode” to discover if Netflix’s movies are getting shorter over time and which guest stars appear in the most popular episode of "The Office", using everything from lists and loops to pandas and matplotlib.

You’ll also gain experience in an essential data science skill — exploratory data analysis. This will allow you to perform critical tasks such as manipulating raw data and drawing conclusions from plots you create of the data. 

--------



||🎯 Project Tasks|:memo: Instructions|
|--|--|--|
|1.| Loading your friend's data into a dictionary|🔶Create a list of years from 2011 to 2020 and a list durations of the average movie lengths our friend provided (103, 101, 99, 100, 100, 95, 95, 96, 93, and 90).<br>🔶Create a dictionary movie_dict, with the keys "years" and "durations" and the values set to your lists years and durations.<br>🔶Print and inspect the dictionary to ensure it was created correctly.|
|2.| Creating a DataFrame from a dictionary|🔶Import pandas using its usual alias, pd.<br>🔶Create a DataFrame durations_df using your movie_dict dictionary you created in the previous step.<br>🔶Print the entire DataFrame.|
|3.| A visual inspection of our data|🔶Import matplotlib.pyplot under the alias plt.<br>🔶Create a line plot of the data with the years column of durations_df on the x-axis, and the durations column on the y-axis.<br>🔶Add the title "Netflix Movie Durations 2011-2020" to your plot.|
|4.| Loading the rest of the data from a CSV|🔶Create another DataFrame, netflix_df, this time using the CSV file our friend provided us with, available at the path "datasets/netflix_data.csv".<br>🔶Print the first five rows of the DataFrame to inspect the data and ensure it was created successfully.|
|5.|Filtering for movies!|🔶Subset the netflix_df DataFrame such that only rows where the type is a "Movie" are preserved.Assign the result to netflix_df_movies_only.<br>Subset the netflix_df_movies_only DataFrame to preserve only the columns title, country, genre, release_year, and duration. Assign the result to netflix_movies_col_subset.<br>🔶Print the first five rows of netflix_movies_col_subset.|
|6.| Creating a scatter plot|🔶Using your netflix_movies_col_subset DataFrame, create a scatter plot, placing the release_year on the x-axis and the movie duration on the y-axis.<br>🔶Add a title to your plot: "Movie Duration by Year of Release".<br>🔶Show the plot.|
|7.| Digging deeper|🔶Subset netflix_movies_col_subset to create a new DataFrame short_movies containing only movies that have a duration fewer than 60 minutes.<br>🔶Print the first 20 rows of short_movies to get a good overview of the types of films with a short duration.|
|8.| Marking non-feature films|🔶Initialize an empty list called colors to store our different color values.<br>🔶Use a for loop to iterate through the netflix_movies_col_subset DataFrame's rows and append colors to your colors list based on the following conditions:<br>- If the genre is "Children", append "red".<br>- If the genre is "Documentaries", append "blue".<br>- If the genre is "Stand-Up", append "green".<br>- If the genre is any other genre, append "black".<br>🔶Print the first 10 values of your colors list to inspect the results.|
|9.| Plotting with color!|🔶Using the data contained in netflix_movies_col_subset, plot the same scatter plot as you did in Task 6, but with a few modifications:<br>- Color the points on the scatter plot using your colors list you defined in the previous step.<br>- Add a title "Movie duration by year of release", an x-axis label "Release year", and a y-axis label "Duration (min)".<br>🔶Show the plot.|
|10.| What next?|🔶Provide your answer to the question "Are we certain that movies are getting shorter?" in the form of a string.|


------
