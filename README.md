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

