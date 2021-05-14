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

Our model showed that the top predictors for the Random Forest (our best model) was gps_height, population, construction year, and well age. We also deemed it worth noting that the top predictors in the Logistic Regression model are quantity type and waterpoint type (which data visualization seems to confirm the importance of these predictors as well).

### Visual 1

![scatter_long](https://user-images.githubusercontent.com/77891283/118209480-b1411c00-b436-11eb-8f0a-c2117a37038b.png)

### Visual 2

![status_histo](https://user-images.githubusercontent.com/77891283/118209530-c5851900-b436-11eb-916c-0d38d0692ffd.png)

## Conclusions

With an approximately 79% accuracy rate, our optimized random forest model is able to point out some very important predictors for determining a well's status. That being said, the topic of well status in Tarzania likely requires more data and research in order to build models able to make more accurate predictions along all three classes.

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
