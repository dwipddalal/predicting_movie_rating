# Predicting_movie_rating

## Dataset:
Here the dataset used has been obtained from <a href='https://www.kaggle.com/datasets/akshaypawar7/millions-of-movies'>Kaggle</a>.
My train-test split of the dataset can be found <a href = 'https://drive.google.com/drive/folders/1PJTqbzhEhwQyEhVykJh20V0c8tzFsQNs?usp=sharing'>here</a>.

## Logic:
Overall flow:

So here, I basically split the data into two parts. One will be the NLP part, and the other will be the numeric part.
I have processed the dataset on the basis of some assumptions that is:                                     
->id does not have any impact on the rating of the movie  
->production companies do not seem to have much impact on the movie's rating; the logic behind it is that there are 1.5l production companies and almost 7l entires. So here, the categorical encoding will not be of much help. Also, there are lots of null values in these columns. More than 50% of the values are null.

Here I have made four models made by taking different columns for different models:                    
-> 1st model: using the columns of categorical and numerical values.        
-> 2nd model: using the columns with more than one categorical value in each of their cells, i.e., using 'genres' and 'credits'.
-> 3rd model: using the 'overview' column.
-> 4th model: using the 'keywords' column.

And then finally perform integrated stacking on these four models so formed.

## Nomenclature of the files:
Analysis.ipynb : contains a through analysis of the dataset
Avg_rating_pred : contains the models written in the above-mentioned order
Integrated stacking: contains the stacked model and the class to perform prediction on the unseen data input
## Model Architecture 
![model](https://user-images.githubusercontent.com/91228207/176964676-390de262-2018-4c94-8730-0da94e0974a3.png)



