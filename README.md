## Music-Genres-Classification-and-Recommendation-System
# Idea
Hello everyone!\
Since I learned Python,It has been 5 months.\
This is kinda my first machine learning project done from zero to finished.\
The idea of our project is from one of my teammates who loves to listen to music on Spotify.\
But unfortunately, The recommendation system on Spotify is made for general users, not for personal.\
Therefore, We decide to build a customized system for ourselves. \
Doesn't it sound exciting?? LoL

# Method
Mostly we used a package called librosa, a useful tool which help us analyze audio files and extract the features we wanted.\
Firstly, We downloaded 100-thousand different audio files from Internet but most of them are belongs to Rock genres. We retrained those audio files with less genres data in order to balance our genres.\
Secondly, We put every song muti-labels(not single label) to classify them more specific.\
Third, after finishing data-preprocessing, We Built a model with three layers NN using BinaryCrossentropy as our loss funtion(click the [CODE LINK](https://colab.research.google.com/drive/19vx7-9ogV0VJdORmiBwPiLuU9AnFkrKx?usp=sharing) to see the model detail) which can classify song's genres.(acc up to 75%)(evalution:AUC)
Last but not least, we build a recommandation system by utilizing cross comparison way to get the optimal songs to our users.

# Result
When users put a song they love into our model, they can get the most similar genres songs eventually.

# Future
Because of unbalance genres data, we retrained the same songs with less genres data. Maybe we can alter song's gamut to a brand_new song but still the smae genres. Therefore, we can avoid overfitting then be able to train deeper.
Because of using NN, there will be more possibilities to be overfitting. Maybe we can try cnn to avoid these situations.
