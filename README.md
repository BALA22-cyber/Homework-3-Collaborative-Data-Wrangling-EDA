# Steam Games Dataset Analysis


## Dataset Source and Description
The dataset used in this project is the Steam Games Dataset originally sourced from Kaggle (accessed September 2025).

Link to the dataset: https://www.kaggle.com/datasets/fronkongames/steam-games-dataset

It contains information about games published on Steam, including attributes(30+ attributes) such as:

	•	Game name
	•	Price
	•	Description text (“About the game”)
	•	Release year
	•	Device compatibility (Windows, Mac, Linux)

This dataset has been created with [this code](https://github.com/FronkonGames/Steam-Games-Scraper) (MIT) and use the API provided by Steam, the largest gaming platform on PC. Data is also collected from Steam Spy.

Dataset had a csv structure issue(missing comma), so we fixed it manually. Fixed dataset link:  https://drive.google.com/file/d/1_OBVdhz99-_iKvFOKMgTmw0e69B6jymt/view?usp=sharing

## Data Analysis and cleaning

### Checkout data_cleaning.ipynb for data cleaning code

Balaji Selvakumar performed data cleaning by removing certain columns which are NLP specific("object" datatypes) and might not be relevant for EDA of the current assignment. 

- Removed NaN Values and replaced them to 0
- Removed Duplicate AppIDs
- Changed "object" dtype NaNs to Unknown
- Parsed `Release year` from `release_date` (dropped rows missing critical fields). 
- Reduced total number of missing values from 14% to 0.2% 

## EDA 

Davis Hunter performed Exploratory Data Analysis (EDA), including price trends, game description word/phrase analysis, platform compatibility, and release year trends.

### Checkout 'eda.ipynb' for EDA


