# Netflix Movie Duration Analysis

## Introduction
Netflix, a powerhouse in the entertainment industry, has evolved from its humble beginnings as a DVD rental service in 1997 to become one of the largest and most influential streaming platforms today. As part of your exploration into the world of data analysis, you have been presented with an intriguing hypothesis: the average duration of movies on Netflix may be declining over time.

To investigate this claim, you are provided with a dataset named `netflix_data.csv`, which contains information about various shows on the platform. Armed with your Python skills, you will conduct exploratory data analysis (EDA) to determine whether movie lengths are indeed getting shorter, and if so, identify potential contributing factors.

## Dataset Description

The dataset (`netflix_data.csv`) includes the following columns:

- `show_id`: The ID of the show
- `type`: Type of show (e.g., Movie, TV Show)
- `title`: Title of the show
- `director`: Director of the show
- `cast`: Cast of the show
- `country`: Country of origin
- `date_added`: Date added to Netflix
- `release_year`: Year of Netflix release
- `duration`: Duration of the show in minutes
- `description`: Description of the show
- `genre`: Show genre

## Initial Code Setup
Before diving into the analysis, the dataset is loaded into a Pandas DataFrame using the following code:

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
dataset = "netflix_data.csv"
netflix_df = pd.read_csv(dataset)
netflix_df.head()

Exploratory Data Analysis (EDA)
I started the analysis by attempting to create a scatter plot of movie duration by release year. The code snippet provided is a part of this effort. Make sure to execute this code to visualize the data.

# Using netflix_df, initialize a figure object called fig with width 12 and height 8
# Create a scatter plot with release_year on the x-axis and movie duration on the y-axis
# Label the plot and axes accordingly
fig = plt.figure(figsize=(12, 8))
plt.scatter(x=netflix_df['release_year'], y=netflix_df['duration'], c=colors)
plt.title("Movie Duration by Year of Release")
plt.xlabel("Release year")
plt.ylabel("Duration (min)")
plt.show()

Analysis Question
Now, the critical question is: "Are we certain that movies are getting shorter?" Evaluate the data and provide your answer as a string assigned to the variable answer. Possible answers are "yes," "no," or "maybe."



# Provide your answer
answer = 'maybe'
print("Are we certain that movies are getting shorter? Answer:", answer)
Feel free to further explore the dataset and add more analysis to support your conclusion. Happy coding!


You can copy and paste this template into your README file and customize it as needed.






