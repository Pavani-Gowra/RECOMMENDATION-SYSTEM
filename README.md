# RECOMMENDATION-SYSTEM

COMPANY : CODTECH IT SOLUTIONS

NAME : G PAVANI

INTERN ID : CT08DK681

DOMAIN : MACHINE LEARNING

DURATION : 8 WEEKS

MENTOR : NEELA SANTHOSH

DESCRIPTION OF THE TASK :

 Building a Recommendation System using Collaborative Filtering :
 
As part of the fourth and final task of my Machine Learning Internship at CodTech IT Solutions, I was assigned the task of building a Recommendation System using Collaborative Filtering techniques. The aim was to understand how recommendation engines work and implement a model capable of suggesting items (e.g., movies) to users based on historical interaction data. This task gave me hands-on experience with one of the most practical applications of machine learning in real-world platforms like Netflix, Amazon, and Spotify.

**Tools and Technologies Used:

Programming Language: Python

Development Environment: Jupyter Notebook

**Libraries Used:

->pandas – for data manipulation and preprocessing

->NumPy – for mathematical computations

->scikit-learn – for splitting the dataset

->surprise (Scikit-Surprise) – a specialized library for building and analyzing recommender systems

->matplotlib – for basic visualization

**Dataset
I used the MovieLens dataset, a popular dataset for benchmarking recommender systems. It contains:

*User IDs

*Movie IDs

*Ratings (given by users to movies)

This data reflects real-world user preferences and is ideal for implementing collaborative filtering algorithms.

Task Workflow:

1. Data Loading and Exploration :
The dataset was loaded using pandas. I explored the structure of the dataset, checking for null values, rating distribution, and unique user-item interactions. I ensured the data was clean and ready for modeling.

2. Understanding Collaborative Filtering :
Collaborative Filtering is based on the idea that users with similar preferences in the past will have similar preferences in the future. It doesn’t require explicit features of the items or users—just their interaction data (ratings).

I implemented User-Based Collaborative Filtering, which recommends items to a user based on items liked by similar users.

3. Model Building using Surprise Library :
To implement collaborative filtering effectively, I used the surprise library, which is specifically designed for building recommendation systems.

**Steps included:

*Loading the dataset into Surprise format using Dataset.load_from_df()

*Defining a similarity measure (cosine similarity)

*Creating the model using the KNNBasic algorithm

*Training the model using a trainset created from the full dataset


4. Making Predictions and Evaluation :
The model was tested on the 20% test dataset to check how well it predicted unseen ratings. I used Root Mean Square Error (RMSE) as the primary evaluation metric, which measures the average magnitude of prediction error.

5. Generating Recommendations :
After training and testing the model, I implemented a function to recommend top N movies to a specific user based on the highest predicted ratings. This function filtered out movies the user had already rated to ensure only new recommendations were made.

**Challenges and Learnings:

Initially, understanding the theoretical difference between content-based and collaborative filtering was a challenge. With more research, I realized collaborative filtering is powerful when you have ample interaction data. The task also taught me how similarity metrics (like cosine similarity) play a crucial role in finding user neighborhoods.

Another challenge was handling the sparsity of user-item matrices. Since not every user rates every item, the data is highly sparse. The Surprise library helped mitigate these challenges by abstracting much of the matrix handling.

**Conclusion :

This task significantly enhanced my understanding of recommendation systems, especially user-user collaborative filtering. I learned how to preprocess data for recommender models, use dedicated libraries like Surprise, calculate similarities, and evaluate predictions effectively.

By completing this task, I acquired practical skills that can be applied in building recommendation engines for e-commerce, streaming platforms, or social networks. This task also wrapped up the internship with a strong application of machine learning to personalization and user experience enhancement.

