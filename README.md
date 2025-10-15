🎬 IMDb Movie Dataset – Exploratory Data Analysis (EDA)

📘 Project Overview

This project performs Exploratory Data Analysis (EDA) on the IMDb Movie Dataset to uncover insights about movie performance, ratings, revenues, and other important attributes.

The goal is to understand patterns and relationships between various movie features such as ratings, votes, metascores, and revenues, and visualize key findings using Python data visualization libraries.

📂 Dataset Information

Dataset Name: IMDB-Movie-Data.csv
Source: IMDb Movie Dataset (Kaggle or similar public source)

Key Columns:

🎞 Rank: Movie rank based on IMDb rating.

🗓 Year: Year of release.

⏱ Runtime (Minutes): Duration of the movie.

⭐ Rating: IMDb rating of the movie.

💵 Revenue (Millions): Box office revenue.

🗳 Votes: Number of audience votes.

🧠 Metascore: Average critic rating.

🧍‍♂️ Director, Actors, Genre – categorical information.

🧠 Project Objectives

Perform data cleaning and quality checks (missing values, duplicates, etc.)

Conduct univariate and bivariate analysis to explore relationships.

Visualize distributions, correlations, and patterns across variables.

Derive insights about factors influencing movie success (ratings, votes, and revenue).

🧹 Data Preprocessing

Checked for null values using df.isnull().sum().

Detected and handled duplicates using df.duplicated().

Converted numeric columns and calculated basic statistics using df.describe().

📊 Exploratory Data Analysis

🔸 Univariate Analysis

Explored single-column distributions:

Rank, Year, Runtime, Rating, Revenue, Votes — analyzed using sns.histplot() and plt.hist().

Observed general trends in movie ratings, runtime, and revenue distribution.

🔸 Bivariate Analysis

Examined relationships between two variables:

Rating vs Votes – higher votes tend to correspond to higher ratings.

Rank vs Year – visualized trends in ranking across different years.

Metascore vs Rating – explored correlation between critic score and user rating.

🔸 Correlation Heatmap

Used sns.heatmap(df.corr(), annot=True) to visualize numeric relationships between variables.

Found positive correlation between Votes, Revenue, and Rating.

Weak correlation observed between Runtime and Revenue.

📈 Key Visualizations

Heatmap of correlations.

Histograms for each numeric column.

Scatterplots: Rating vs Votes, Rank vs Year, etc.

Count plot showing movie frequency by year.

Revenue and rating distributions.

💡 Insights & Observations

Movies with higher votes generally have better IMDb ratings.

Revenue is often higher for movies with good ratings and metascores.

Number of movies produced has increased over the years.

Some missing or zero revenue data might affect interpretation.

🧰 Tools & Libraries Used

Python

NumPy → numerical computations

Pandas → data manipulation

Matplotlib & Seaborn → data visualization

🏁 Conclusion

This analysis provides insights into how ratings, votes, metascores, and revenues interact within IMDb movie data.

Visual exploration helps identify patterns that explain what makes a movie popular and successful.
