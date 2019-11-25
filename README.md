# Secrets Behind Recipes

# Abstract
Cooking is an important skill for everyone, no matter where they live. After evolving for centuries, what people eat everyday has grown into systems. Every country has their own style of eating and the styles diverge from region to region. Through the recipes, we can know what is frequently eaten by the people of one country and how they usually cook. We can even go further, find the relationships between what people eat and how their health conditions are, and dig out all the secrets behind the recipes.

In this project, we want to show the different cooking choices of ingredients, seasoning, etc. among countries. Then we will try to link the recipe features with people's health condition to find out if there is something in eating habits that influences people's health. Besides, using the instructions of cooking steps of each recipe, we will map the recipes to vector space so that we can measure the difference of recipes among countries. To go even further, we want to train a model to predict the flavors of a dish, given its recipe, so that we know the flavor preference of people in different countries. In the end, after all these analysis of people's preference, we hope to make a recommendation system so that we can recommend dishes to people if we know their nationality.

# Research questions
How do eating habits vary in different countries?
- the most frequently used seasoning
- the most common cooking methods(boil, stir, fry, etc)
- the most frequently used ingredients (except seasoning) in general and specifically for main dish, dessert, beverage, etc.

How are the different eating habits related to health?
- the life span( developed/developing)
- some common food-related disease: cancer, obesity

The recommendation systems for food
- according to historical beloved food and ratings
- according to the ingredients we have

# Dataset
The first two dataset we used are collected from kaggle (https://www.kaggle.com/shuyangli94/food-com-recipes-and-user-interactions). `RAW_recipes.csv` contains 230185 different recipes and `RAW_interactions.csv` contains 1125283 comments from users regarding the recipes. In `RAW_recipes.csv`, the column 'tags' contains information about country and dish type of the recipe, which is used for further analysis. Also, the ingredients need and cooking steps of eac recipe is provided. In `RAW_interactions.csv`, the reviews and the corresponding recipe id enable NLP analysis of people's feedback towards recipes.

# A list of internal milestones up until project milestone 3

17.11

- Change Topic to "Everyone can be a cook"
- Download the required data
- Search for additional information on quantities of each ingredient usage corresponding to the recipes, scrape data to augment dataset.

23.11

- Data cleaning for newly found data (identification and removal of invalid data)
- Extract countries(regions) informations from raw dataset and classify recipes according to continents. It helps analysis distributions and patterns on different granularity level.
- Extract flavors from user description, using it as target label of further multi-class classification training. 
- Classify recipes by meal types, explore most common used ingredients and cooking method of each country

10.12


- build and test the correlationship between food and disease occurance on the level of countries(regions)
- train classification model to predict flavors of recipes based on ingredients inputs.
- train regression model to predict nutritions of recipes based on ingredients and cooking method.
- NLP processing for recipe instructions and ingredients to find similarities between different recipes and cluster them. It is also possible to establish recommendation system based on recipe similiarity. 
- implement recommendation system based on matrix factorization.

18.12

- Compare the effectiveness of trained model 
- Explore possibilities for the data visualization
- Summarize results and figures, find the best way to present them in datastory

23.12

- Comment and refactor our code
- Release of final notebook and datastory

# Questions for TA
Do you have any suggestions for recommendation system? 
Is it consistent with the rest of our project?  
