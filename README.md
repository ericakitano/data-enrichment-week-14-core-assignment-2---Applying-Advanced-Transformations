# data enrichment week 14 core assignment 2 - Applying Advanced Transformations
 
## The Data

You will be working with a heavily modified version of the Superheroes dataset from Kaggle.

The dataset includes two csv's:

- superhero_info.csv:
   - Contains Name, Publisher, Demographic Info, and Body measurements.
   
- superhero_powers.csv:
   - Contains Hero name and list of powers
   
   
## The Task

Your task is two-fold:

**I. Clean the files and combine them into one final DataFrame.**

  - This dataframe should have the following columns:
       - Hero (Just the name of the Hero)
       - Publisher
       - Gender
       - Eye color
       - Race
       - Hair color
       - Height (numeric)
       - Skin color
       - Alignment
       - Weight (numeric)
       - Plus, one-hot-encoded columns for every power that appears in the dataset. E.g.:
             - Agility
             - Flight
             - Superspeed
             - etc.
             
Hint: There is a space in "100 kg" or "52.5 cm"



**II. Use your combined DataFrame to answer the following questions.**

   1. Compare the average weight of super powers who have Super Speed to those who do not.

   2. What is the average height of heroes for each publisher?


[(Source)](https://www.kaggle.com/datasets/claudiodavi/superhero-set)


***

![feedback](feedback.PNG)

Summary of Filenames:

* `Applying Advanced Transformations (Core).ipynb` - Original Submission (before feedback)
* `(Fixed the Problem) Applying Advanced Transformations (Core).ipynb` - Retried for my own learning based on assignment feedback (after feedback)
* `Folder: My Own Experiment` - I tried to switch the order of one-hot-encode vs dataframe merge, but it was not the issue.

In the end, I found that the issue was that I needed to create a separate column "Powers_split" before exploding, in order to make `cols_to_make`.

I needed to differentiate when to use "Powers_split" and when to use "Powers".

By NOT differentiating the exploded "Powers_split" vs original "Powers" in my original assignment submission, when I did the for loop to create new column, it created multiple rows for the same Hero. By differentiating the two, I only have one row per Hero.

