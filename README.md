# Music_Genres_Classification_and_Recommendation_System
## Introduction
As the world's musical library continues to expand, offering us an ever-increasing array of choices, it becomes increasingly important to have personalized methods of selecting songs that resonate with our unique tastes. Although modern music streaming platforms like Spotify offer various recommendation systems, these are often tailored for a general audience rather than individual preferences. Recognizing this, we've decided to create a customized music recommendation system that caters specifically to our personal tastes and preferences.     

## Method
We primarily utilized Librosa, a powerful tool for analyzing audio files and extracting desired features. Initially, we downloaded approximately 100,000 audio files from the internet, predominantly from the rock genre. To ensure genre diversity, we performed data augmentation to enlarge the dataset with audio files from underrepresented genres. Additionally, we assigned multiple labels to each song, rather than a single label, to enable more specific genre classification. Finally, we built our model using a three-layer neural network, employing Binary Cross-Entropy as our loss function, to accurately classify songs into their respective genres.     
(click the [CODE LINK](https://colab.research.google.com/drive/19vx7-9ogV0VJdORmiBwPiLuU9AnFkrKx?usp=sharing) to see the model detail)**(accuracy up to 75%)**(evalution:AUC)    

Finally, we developed a recommendation system using a cross-comparison approach. This method involves comparing various features of songs within our dataset to identify those that closely align with the individual preferences of our users. By analyzing the similarities between songs in terms of their musical characteristics and genres, our system is able to suggest the most suitable and enjoyable tracks to each user. This personalized approach ensures that the recommendations are not only based on general popularity or broad genres but are tailored to the specific tastes and listening habits of each individual.     

## Result
When users input a song they enjoy into our model, the system is designed to identify and recommend three songs with similar genres to them.    

## Future
Due to the imbalance in genre representation within our dataset, we retrained our model with a more balanced selection of songs, focusing on genres that were previously underrepresented. One innovative approach we considered was altering the pitch and tempo of existing songs to create new variations, while still maintaining their original genre characteristics. This strategy not only diversifies our dataset but also helps in mitigating the risk of overfitting, thereby enabling us to train our model more comprehensively.   

Given the inherent risk of overfitting associated with neural networks, we are exploring the potential of Convolutional Neural Networks (CNNs) as an alternative. CNNs, renowned for their proficiency in pattern recognition and feature extraction in complex datasets, could offer improved generalization in identifying intricate patterns in music data. This shift in methodology might enhance our system's ability to discern nuanced differences between genres and deliver more accurate recommendations.    
