# Recommender-System

We have developed a recommendation system that helps users discover new places of interest in different categories based on similar users’ habits. 

We have utilized a dataset of Foursquare check-ins, which contains check-ins from New York City over ten months, to train this system. 

In generating recommendations, we first use k-means to cluster the users into six broad clusters based on their frequency of visitation across Foursquare venue categories. Then we use a decision tree-based classification model to find the appropriate cluster for our test user. Then we use a cosine distance metric to find three users most similar to our test user and compile a list of venues our test user hasn’t visited yet. 

We give the test user a choice to select a particular category like food places, outdoor & sports activities, etc. for their recommendations. Based on the category selected by the test user, we recommend three venues from our venue list for the user to check out.