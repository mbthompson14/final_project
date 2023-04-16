 Final_p_noreen
# final_project
# Overview 
For Final Project we choose Music and Mental Health Data to work on and for visualization purpose we decided to use Tableau as a tool. In order to get a deep insight on how music helps four main mental illnesses like depression, anxiety, insomnia and OCD, we created different charts to check all possible ways that can determine the effects of music on mental health.
# Results

# Favorite Music Genres by Age
![image](https://user-images.githubusercontent.com/112978144/230151224-ebc71274-400a-42b0-90a1-8621aea2b893.png)


# Music (hours per day) and Anxiety

![image](https://user-images.githubusercontent.com/112978144/230151511-f6b17eff-acdf-42b3-a2ca-39df9b2ae2c4.png)

# Music (hours per day) and Insomnia

![image](https://user-images.githubusercontent.com/112978144/230151809-ad9897d4-24f1-4a3c-ad08-847a2b42d7bf.png)

# Music(Hours per day) and Depression

![image](https://user-images.githubusercontent.com/112978144/230152747-1e1c5960-8477-49bc-ac89-aa144c077110.png)


# Music (hours per day) and OCD

![image](https://user-images.githubusercontent.com/112978144/230152064-a45ab30b-ec86-497f-bde2-afbf388d5e9a.png)

# Music Effects on Mental Health

![image](https://user-images.githubusercontent.com/112978144/230152280-e977b08a-6d91-4c66-add7-84289fe1d26a.png)

# Mental Illness by Age

![image](https://user-images.githubusercontent.com/112978144/230152437-9bcb0b51-97af-472b-8699-5bf8572c802c.png)

# Mental illness by genre

![image](https://user-images.githubusercontent.com/112978144/230152926-7afc4812-5538-46cc-bf06-466308610a87.png)

# Favorite Music Genre by Age

![image](https://user-images.githubusercontent.com/112978144/230153153-93f89370-324e-47f6-8cad-5160cc17bb53.png)

# Music Effects by genre, age and Hours per day

![image](https://user-images.githubusercontent.com/112978144/230153396-89947dbc-5dcb-4d75-94d9-a7aedc177da6.png)

# Mental Illnesses by genre

![image](https://user-images.githubusercontent.com/112978144/230153573-7d21a810-6a1d-466e-85a5-3a7306937688.png)

# Music While Working

![image](https://user-images.githubusercontent.com/112978144/230153741-512139e2-9374-45e2-b1a3-a1aa4090a409.png)

# Dashboard
![image](https://user-images.githubusercontent.com/112978144/230153924-ec5f1b8d-245f-4f0c-ab0a-0b64af31e49c.png)








## Overview of the project:
The Center for Disease Control (CDC) reports that about 1 in 5 Americans will experience mental health issues in a given year. Often stigmatized, many who suffer do so in silence, seldom seek treatment for fear of judgment and many face dire consequences. Mental Health America (MHA) has declared the month of May as the mental health awareness month to promote awareness among the general public and more importantly to urge the public to seek appropriate treatment for mental illness. In the recent years alternative forms of treatment such as yoga, meditation, tai chi, music etc are being promoted as a means to reduce stress which possibly have a positive impact on mental health.
## Project Goal
The goal of this project is to explore music as an alternative form of therapy for mental health indicators such as anxiety, depression, insomnia and obsessive-compulsive disorder (OCD). The key indicator is whether music ameliorates their mental health condition.
## Data Overview:
The dataset is obtained from Kaggle.com entitled “Music and Mental Health Survey Results”. This survey includes a total 736 participants, belonging to a wide range of ages and listening to a variety of genres. The participants self-report their levels of anxiety, depression, insomnia and OCD and whether listening to music either reduced, not changed or worsened their mental health indicators.
## Extract Transform Load:
The data is available as a csv file. The data is first inspected for duplicated and missing values. There was a total of 129 missing values and 0 duplicated values. Some of the columns were renamed for clarity. The cleaned dataset is exported as a csv file and loaded onto a postgres sql database.
## Data preprocessing for machine learning:
The categorical variables are extracted into a separate dataframe. The number of categorical variables totaled to 23. Each categorical variable was checked whether the number sub-categories within each category was equal to 10 or below. Out of the 23, only one categorical variable, Favorite Genre, had 16 subcategories. A cutoff of 25 will set the number of sub-categorical variables to 10 and thus was chosen as a cutoff to bin the categories that were below 25 under the sub-category named "others". After binning, the categorical variables are encoded to numerical dummy variables by One Hot encoder. After encoding, the categorical variable dataframe is merged back to the original dataframe and the non-encoded categorical variables are dropped from the original dataframe. This second dataframe is exported as a csv file and stored in the postgres sql.

