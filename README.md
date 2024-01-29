
# Game Reccomendation Using Machine Learning 🖥️

The project gathers data about games from well-known platfrom steam, preprocesses it and finally creates different types of reccomendation system. 


## About Dataset 🗂️💾

Data has been gathered from steam serach website - [Link Here](https://store.steampowered.com/search/?category1=998&ndl=1&ignore_preferences=1)

The data has been scraped in early September. It is unorganized and needs cleaning/preprocessing.

Link to the dataset - [Click Here](https://www.kaggle.com/datasets/nikatomashvili/steam-games-dataset)
# Methodology⛕
We started by scraping a video game platform steam. We used a rolling page in which the games were loaded endlessly while scrolling until games ran out. The order is less important. In the first scraping phase, we obtained Game data, namely name, price, discounted price, release date, and Link. Later, using the link, we expanded the data and extracted more information for each game. We merged the two datasets into a single file and moved to the next step.

In the second stage, we did preprocessing before we started EDA directly. This could have happened during the EDA, but it was possible to carry out certain manipulations from the beginning. We fixed what we could easily see before EDA and then moved to EDA. This phase was very important because several features were removed and added, new ones were created etc.

EDA describes a lot of things about data that happened
Cleaned, sorted, and visualized. Finally, data was prepared for analysis.

First in the analysis phase
The Jupiter notebook I worked in is Analysis_Main, where I made the main
machine-learning manipulations and finally got the game_recommendations CSV file.
One cell in this file returns an error, which I intentionally left as is and indicated why.

The next file is Analysis – improving, where the game_recommendations created in the previous notebook
was used and improved into the file game_recommendations2. (improved the model)

After that, the games were already grouped and we got the data
which showed 10 recommendations per game. With this, the system can be considered somewhat complete, but I decided to use the user's data for testing purposes. I took the data from Kaggle, just for testing purposes (scraping steam by a customer was completely limited). This file is called steam-200k where there is data on users. Recommendation System - Hybrid is the file in which the main test is used.
The file is hybrid, which means that a collaborative and content-based recommendation approach is used.

In this notebook, one cell saves only content-based file - user_recommendations_ContentBased.

After that I additionally made a Test_Collaborative_ItemBased notebook where only the collaborative approach is implemented, just for testing.

If the Data is used give credit to the owner.
## Names of the Notebooks
• Preprocessing

• EDA of preprocessed data

• ML_Analysis_Main

• ML_Analysis _improving

• Recommendation System - Hybrid (the main target)

• Recommendations system Item-based (just for example)
