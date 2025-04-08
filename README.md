# RecSysTermPrj
This is the repository for recommend system term project
## Topic
Steam game recommendation system that enables customization according to the user's input value using ensemble techniques

## Why Do We Need?
  People's preferences for items change over time. There are ways to combine static and dynamic preferences to solve this problem, but it is difficult to reflect people's preferences that change every day because they reflect the results of the user's sequential behavior.
  In addition, the fixed recommendation system has limitations in reflecting the preferences that change according to the user's mood and time. When a user wants to be recommended items that focus on a specific criterion, I think that the user's satisfaction can be improved by receiving the user's input to the feature standard and presenting the appropriate item tailored to it.

## Model Architecture
![image](https://github.com/user-attachments/assets/8416c20e-f0fe-4fc8-bcd2-a69c1ec68b81)

- Model focusing on i: Models learned from data with greater weight on features
- $W_i$ : parameters to give greater weight to features
- $z_i$ : Results of scoring by focusing on features
- $\hat{y}$: score for each piece of music (the result of multiplying the results of each model by weights and adding them)
  - $w_i$ : Weight to be multiplied by the result of focusing on features
    - It will be inputted about features that are important to the user and set based on them
   

  After experimenting with several models focusing on a specific feature (feature weighting-enabled models e.g. FM-based model, DL-based model, AutoML-based model etc..), the optimal model will be selected and used

## Train Dataset
### User Dataset
- https://www.kaggle.com/datasets/tamber/steam-video-games/data?select=steam-200k.csv
### Item Dataset
- https://www.kaggle.com/datasets/fronkongames/steam-games-dataset
- https://www.kaggle.com/datasets/trolukovich/steam-games-complete-dataset

## Test Dataset
- https://cseweb.ucsd.edu/~jmcauley/datasets.html#steam_data
