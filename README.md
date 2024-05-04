# Capstone-Project-Netflix-Movie-Recomender-System

![image](https://github.com/Ankit-770/Netflix-Movie-Recomender-System/assets/90442965/c464b9c0-4fec-4fd9-bae0-750857581755)


Developing an effective and efficient movie recommender system for Netflix is a crucial initiative aimed at enhancing user experience and maximizing user engagement on the platform. The primary objective is to provide personalized movie recommendations to each user, taking into account their preferences, viewing history, and behavior.

The business aim of this project is threefold:
Enhanced User Experience: By providing accurate and personalized movie recommendations, the recommender system aims to improve user satisfaction and engagement, leading to increased platform usage and customer loyalty.
Content Utilization: Optimizing the usage of available content by guiding users to movies that align with their interests, ultimately driving higher viewership of a wider range of movies offered by Netflix.
Business Success: The development of a robust movie recommender system will support informed decision-making, helping Netflix to maximize user retention, customer satisfaction, and overall business performance, thereby ensuring sustained growth and competitiveness in the streaming industry.

Therefore, the successful implementation of an advanced recommender system is imperative for Netflix as it directly impacts user engagement, content consumption, and the overall success and growth of the streaming platform.

## Problem Statement

In the face of an ever-growing library of movies and TV shows, providing tailored and precise movie recommendations has become essential for Netflix to enhance user experience and encourage sustained platform engagement. The challenge at hand is to create an advanced recommendation system capable of accurately predicting user preferences in order to offer personalized movie recommendations to each user. The primary focus of this project is to design and implement a recommendation system that addresses the following core objectives:
Personalized Recommendations: Develop a system capable of producing personalized movie suggestions based on user viewing history, behavior, preferences, and interactions with the platform.
User Engagement: Enhance user satisfaction and engagement by presenting recommendations aligned with individual preferences, increasing the likelihood of continued and regular use of the Netflix platform.
Content Discovery: Enable users to discover a broader range of movies, ensuring optimal utilization of Netflix's extensive library while increasing viewer engagement.

## Data Overview

This dataset contain information about various TV shows and movies available on Netflix, including details like the production country, release year, rating, duration, genre, and a description of each title.

Attribute Information

1. show_id : Unique ID for every Movie / Tv Show
2. type : Identifier - A Movie or TV Show
3. title : Title of the Movie / Tv Show
4. director : Director of the Movie
5. cast : Actors involved in the movie / show
6. country : Country where the movie / show was produced
7. date_added : Date it was added on Netflix
8. release_year : Actual Releaseyear of the movie / show
9. rating : TV Rating of the movie / show
10. duration : Total Duration - in minutes or number of seasons
11. listed_in : Genere
12. description: The Summary description

## Approach
The following steps were followed in the project:

Data Preprocessing: The dataset was preprocessed and cleaned to handle missing values, outliers, and any inconsistencies in the data.

Text data preprocess: Lower Casing, Removing Punctuations, Removing URLs & words contain digits, emoving Stopwords & White spaces, Rephrase Text, Tokenization, Text Normalization, Part of speech tagging, Text Vectorization. Dimesionality Reduction(PCA)

Data Clustring: The preprocessed data was clustered in different groups based on similarity ans group together based on elbow method or silhouette score. By using different clustering algorithem we group similar data together.


Model Deployment: The selected model can deployed using pickle, where it could recommend movies based on similarity created in different clustering algorethms. The model's performance can monitor over time to ensure its usefulness.

## Models Used
For modeling we tried various clustring models such as- 
1)K-Means Clustering

2)Hierarchical Clustering (Agglomerative Clustering)

3)Silhouette Score for Clustering

4)Elbow method for Clustering

## Results
From the Elbow method and Silhouette score we can choose optimal no of clusters to group data based on similarity of the data. in the end i use cosine similarity to buid a recomender system which recommend movies based similarity and clusters.

## Outputs

![image](https://github.com/Ankit-770/Netflix-Movie-Recomender-System/assets/90442965/0eb56c62-a888-45f8-ad5e-e0d808c8cecb)

![image](https://github.com/Ankit-770/Netflix-Movie-Recomender-System/assets/90442965/9aea70a3-5203-485d-b65d-b5809c77e497)

![image](https://github.com/Ankit-770/Netflix-Movie-Recomender-System/assets/90442965/e76f83f3-4733-4949-8f86-6864714444ca)

![image](https://github.com/Ankit-770/Netflix-Movie-Recomender-System/assets/90442965/2dea8987-c398-4c16-9ec1-29fef41f2a3c)

![image](https://github.com/Ankit-770/Netflix-Movie-Recomender-System/assets/90442965/36ff0af7-136f-459c-b580-9845e69e5ecd)

![image](https://github.com/Ankit-770/Netflix-Movie-Recomender-System/assets/90442965/9601502e-bc6b-482c-a279-6713dab76d01)



## Conclusion
During our analysis, Firstly I cleaned the data and conducted an exploratory data analysis (EDA) on all the features in our dataset. Firstly, I analysed my variable applied transformations as per requirement.Then I evaluate categorical variables to impliment clustering algorithms. I have done Monovariate and Bivariate analysis on these variables . I also studied the numerical variables, calculated their correlations, and the their relationships with the dependent variable.

I employed 2 machine learning algorithms including K-Means Clustering, Hierarchical Clustering (Agglomerative Clustering), Silhouette Score and Elbow method to get optimal no of clusters .

Some facts based on analysis:.

1)The analysis revealed that Netflix has a greater number of movies than TV shows, with a rapidly growing collection of shows from the United States.

2)To cluster the shows, i have selected six key attributes: director, cast, country, genre, rating, and description

3)i used K-Means and Agglomerative clustering algorithms to group the shows. The elbow method confirmed that the optimal number of clusters was 6 for K-Means, however for Silhouette score analysis it was 13.

4)In Agglomerative clustering the optimal number of clusters was 9, which we visualized with a dendrogram.

5)69.1% of the data belongs to movies and 30.9% of the data for TV shows.
