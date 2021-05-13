# Tanzania Water Pump Analysis

**Authors**: David Tian, Christopher de la Cruz

## Overview

Our analysis currently reflects all the factors that play a role into predicting whether a well in Tarzania is function, in need or repair, or non-functional. We take a closer look at some of the heavier weighted predictors to give us a glimpse into what affects a well's functional status. ADD CONCLUSION HERE. This data can be used by any Tarzanian government organization or non-profit in Tarzania looking to make decisions basen on well status.

## Business Problem

We are a Tarzanian government agency. Using data from Taarifa and the Tanzanian Ministry of Water, can we predict which pumps are functional, which need some repairs, and which don't work at all? A smart understanding of which waterpoints will fail can improve maintenance operations and ensure that clean, potable water is available to communities across Tanzania.

## Data

Our dataset contains well function statuses as well as numerous different factors about the well such as its age and gps height. There are the predictors we elected that our model uses:

- GPS Height = Altitude of the well<br>
- Population = Population around the well<br>
- Construction Year = Year of construction of the well<br>
- Basin = Geographic water basin<br>
- Region Code = Geographic location (coded)<br>
- District Code = Geographic location (coded)<br>
- LGA = Geographic location<br>
- Public Meeting = True/False<br>
- Scheme Management = Who operates the waterpoint<br>
- Permit = If the waterpoint is permitted<br>
- Extraction Type = The kind of extraction the waterpoint uses<br>
- Management = How the waterpoint is managed<br>
- Payment Type = What the water costs<br>
- Water Quality = The quality of the water<br>
- Quantity = The quantity of water<br>
- Source = The source of the water<br>
- Waterpoint Type = The kind of waterpoint<br>
- Geographical Split = Which quadrant is the well located in<br>

## Methods

After cleaning the data, we ran the data through several different models (KNN, Logistic Regression, Decision Tree, and Random Forest) and optimized each model to see which one gave us optimal results for predicting each class.

## Result 1

Our model shows that not all renovations generate enough savings to necessarily be worth the price and labor (we showcase the relationships in our conclusion). Here are the results of our grade & condition model.

### Visual 1

![gradeconmodel](https://user-images.githubusercontent.com/77891283/115739327-d375db80-a35b-11eb-9add-fbe1051d8b0d.png)


## Conclusions

These are our business recommendations regarding renovations done to a house before selling it on the market:

Our analysis shows that square footage of the living space is strongly correlated with the price of a house. While we realize that increasing an already-built house's footage may not always be realistic, we've discovered that there is statistical differences in the price of homes depending on it's Grade or Condition rating.

For Grade, we're 95% confident of the following: <br>
- Upgrading homes with a grade of 6 to a 7 can generate a 53K - 77K savings amount.
- Upgrading homes with a grade of 7 to an 8 can generate a 52K - 78K savings amount.
- Upgrading homes with a grade of 8 to a 9 can generate a 38K - 65K savings amount.

For Condition, we're 95% confident of the following: <br>
- Upgrading homes with a condition of 2 to a 3 can generate a 41K - 55K savings amount.
- Upgrading homes with a condition of 2 to a 4 can generate a 57K - 71K savings amount.
- Upgrading homes with a condition of 2 to a 5 can generate a 75K - 90K savings amount.
- Upgrading homes with a condition of 3 to a 4 can generate a 8K - 23K savings amount.
- Upgrading homes with a condition of 3 to a 5 can generate a 27K - 42K savings amount.
- Upgrading homes with a condition of 4 to a 5 can generate a 11K - 26K savings amount.


## For More Information

Please review our full analysis in our Jupyter Notebook or our presentation: https://docs.google.com/presentation/d/1SX5UJGmCgV2di-Wo5SZsfECan8wcSG7Y7HiPm24aCQs/edit#slide=id.gd0341dc497_0_842

For any additional questions, please contact **Christopher de la Cruz at cdelacruz2013@gmail.com, David Tian at dt1086@stern.nyu.edu**

## Repository Structure

```
├── README.md                                         <- The top-level README for reviewers of this project
├── Phase2 Project.pdf                                <- PDF version of project presentation
├── Real Estate Recommendations Analysis.ipynb        <- Narrative documentation of analysis in Jupyter notebook 
├── data                                              <- Both sourced externally and generated from code     
└── images                                            <- Both sourced externally and generated from code
```
