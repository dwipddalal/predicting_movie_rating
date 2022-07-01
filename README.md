# Predicting_movie_rating

## Dataset:
Here the dataset used has been obtained from <a href='https://www.kaggle.com/datasets/akshaypawar7/millions-of-movies'>Kaggle</a>.
My train-test split of the dataset can be found <a href = 'https://drive.google.com/drive/folders/1PJTqbzhEhwQyEhVykJh20V0c8tzFsQNs?usp=sharing'>here</a>.

## Logic:
Overall flow:

So here I basically split the data into two parts one will be NLP part and other will be the numertic part.
I have muniplicated dataset on the basis of some assumptions that is:                                     
->id does not have any impact on the rating of the movie  
->production companies does not seem to have much impact on the rating of the movie  the logic behind it is that there are 1.5l prodcution companies and almost 7l entires. So here the categorical encoding will not be of much help. Also there are lots of null values in this columns more than 50% of the values are null.

Here I have made 4 models one taking different columns for different models                      
-> 1st model: using the columns of categorical and numerical values        
-> 2nd model: using the columns that has more than one categorical values in each of their cells
-> 3rd model: using the columns that has text input in each of their cells


And then finally perform intergrated stacking on these 4 models so formed.

## Model Architecture 
![model](https://user-images.githubusercontent.com/91228207/176964676-390de262-2018-4c94-8730-0da94e0974a3.png)



