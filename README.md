<h1 align="center"><img src="https://bit.ly/2VnXWr2" width="60">

<h1 align="center">Machine Learning: Diamond Price Prediction with Linear Regression </h1>

<p align="center"> Final project developed in the Ironhack Data Analysis Bootcamp </h1>

![image](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
![image](https://img.shields.io/badge/pandas-150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![image](https://img.shields.io/badge/NumPy-013243.svg?style=for-the-badge&logo=NumPy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![image](https://img.shields.io/badge/Seaborn-lightblue.svg?style=for-the-badge&logo=Seaborn&logoColor=blue)
![image](https://img.shields.io/badge/scikitlearn-F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![image](https://img.shields.io/badge/Tableau-E97627.svg?style=for-the-badge&logo=Tableau&logoColor=white)

##  💻 About the project</br>

The main objective of this project was to analyze the historical data of video game sales to draw conclusions about which parameters are most critical for success in creating a game and then compare the insights with the results of a regression model.

Tableau: https://public.tableau.com/app/profile/thomaz.rizzo/viz/Final_Project_16785668158970/VideoGamesSalesDA?publish=yes

## 🛠 Data Analysis (Tableau):

Analyzing the dashboard itself we could observe that:

Sales Over the Years:

- Despite the drop in the curve, this does not mean that the market has weakened, quite the opposite, as the dataset only shows the year the game was released and the total sales through 2016. It is natural that games released more recently have fewer sales (with a few exceptions).

Genre/Platform (Manufacturer)/Rating:

- We can see that the Action, Sports and Shooter genres have had the most sales over the years.

- In relation to the platform (or in a more simplified way, the manufacturer), we could observe that the most successful games belonged to Sony, Nintendo and Microsoft platforms.

- Regarding rating, the best ones were Everyone (E), Teen (T) and Mature (E).

## 🛠 Data Analysis (Machine Learning):

Analyzing the chosen model (Model 1) and the coefficients of the variables considered (plotted alongside), we can draw some conclusions:

1) Considering theaverage sales value (US$ 690k) and the RMSE (US$ 430k), one can say that the RMSE was relatively high (i.e. a forecast of US$ 430k made from sales, a value not too far from the average, can actually be a total sales failure and result in US$ 0 in sales).

2) If we compare with the historical analysis done before the modeling, we also find some divergences:

Rating:
- K-A rating and RP are the variables with the highest index, while in the initial analysis we found that these variables were a minority (RP even not even appearing in the database). Even after artificially filling the data with the 'mode',these values remained very low and it does not make much sense to be as determinants of large number of sales.

Manufacturer:
- Here in fact it was found that Sony, Nintendo and Microsoft manufacturers are the most determinants, which was found in the initial analysis.

Genre:
- The genre variable was left in the middle ground. Some values make sense, like 'action', 'sports' and 'shooter', which are the top 3 best selling genres. But there is a divergence when assigning a high index to the simulation genre, for example, which was the fourth worst.

The model ended up performing in an average way and it is necessary to do more tests to obtain a more faithful model.

##  💻 Result Analysis:

Analyzing the dashboard itself seems to be more reliable than looking at linear regression models to predict sales of a video game based on history. 

As we can see, games made by Nintendo, followed by Sony and Microsoft, are the most successful historically.

Just as the most successful genres for each platform are:

- Nintendo: Platform, Action, Misc, Sports and Role-Playing;
- Sony: Action, Sports, Shooter, Racing and Role-Playing;
- Microsoft: Shooter, Action, Sports, Misc, and Racing. 

The next steps would be to create more regression models (not necessarily linear), to get better results and create a more assertive forecast to predict the number of sales.

## 🛠 Data Sources:

Video Game Sales Dataset 1980 - 2016 (Kaggle) - https://www.kaggle.com/datasets/thedevastator/global-video-game-sales
