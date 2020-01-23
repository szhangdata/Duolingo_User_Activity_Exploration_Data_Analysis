# Duolingo_User_Activity_Exploration_Data_Analysis

**In this project we will perform EDA and predictive modeling of Duilingo user activities.**

**1. The data used here can be download from the website: https://github.com/duolingo/halflife-regression.**

**2. The training data has 13 million data, but we only take 1 million here.**

**3. The input is a list of users along with their demographics, user activity, web session records, and some summary statistics.**

**4. Performed data anaylsis to discover user patterns in data by visualizing data and by computing the correlation between features.**

## Background
The dataset in this project comes from Duolingo, which is the world's most popular platform to learn a language. They offer free online language courses to different ages of people, with different level of courses. Users can choose a variaty of language course, such as English, Spanish, French, Italy, Portuguese and so on. Their vision is to analyze how millions of people learn online courses so as to create the most effective educational system possible and tailor it to each student. Their ultimate goal is to give everyone access to a private tutor experience through technology.

In this Duolingo user activity dataset, we will use some classical ways to explore data efficiently with different packages so that we can develop intuition about data set:
* Import and briefly check data with python data manipulation tools Pandas
* Get basic description of data, descriptive statistics, checking rows and columns.
* Time series analysis
* Simple predictive modeling
* Discover patterns in data by visualizing data with python data visualization packages sucha as Matplotlib, and Seaborn, or by using functions to compute the correlation between features.

## Data Description
In this project, we are given a list of users along with their demographics, user activity web session records, and some summary statistics. We will perform exploration data analysis to develop intuation about the dataset. The target p_recall is the excercise score after taking courses. The outcome will give us correlation between different featurs and p_recall.

## File descriptions
The columns are as follows:
p_recall - proportion of exercises from this lesson/practice where the word/lexeme was correctly recalled
timestamp - UNIX timestamp of the current lesson/practice
delta - time (in seconds) since the last lesson/practice that included this word/lexeme
user_id - student user ID who did the lesson/practice (anonymized)
learning_language - language being learned
ui_language - user interface language (presumably native to the student)
lexeme_id - system ID for the lexeme tag (i.e., word)
lexeme_string - lexeme tag (see below)
history_seen - total times user has seen the word/lexeme prior to this lesson/practice
history_correct - total times user has been correct for the word/lexeme prior to this lesson/practice
session_seen - times the user saw the word/lexeme during this lesson/practice
session_correct - times the user got the word/lexeme correct during this lesson/practice

The lexeme_string column contains a string representation of the "lexeme tag" used by Duolingo for each lesson/practice (data instance) in our experiments. It has been added for this release to facilitate future research and analysis. Only the lexeme_id column was used in our original experiments. 
