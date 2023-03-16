# Kaggle Competition

Notebook with EDA dataset from kaggle and GradientBoosting model

## Case description

Every dwarven settlement has a tavern where delicious ale is poured and wonderful buns are baked.  
Gnomes are quite forgetful and quick, and they forget their wallet at home, and pay off in the morning the next day.

Particularly dishonest residents of the community may not return the money to the institution at all.

## Task

Learn to predict whether a dwarf who left his wallet at home will return the money within the next few days or, in modern parlance, his order will default.   
This will increase the financial stability of the tavern by not fulfilling orders that will not be paid in advance.

## Solution

* Reviewing data, EDA.
* Training sample.
* Training the model and assessing its quality on the validation set.
* Testing another algorithms.
* Saving the model.
* Сonclusions

## Data

Table user_data.  
Contains information about all users of the social network.

|        Field name      |                         Overview                         |
|------------------------|----------------------------------------------------------|
| Deal_id                | Order number                                             |
| Deal_date              | Order date                                               |
| First_deal_date        | Date of first order                                      |
| Secret_dwarf_info_1    | Secret feature by dwarf No. 1                            |
| Secret_dwarf_info_2    | Secret feature by dwarf No. 2                            |
| Secret_dwarf_info_3    | Secret feature by dwarf No. 3                            |
| First_default_date     | First default date                                       |
| Successful_deals_count | How many paid orders were made                           |
| Region                 | Tavern region                                            |
| Tavern                 | Type of tavern                                           |
| Hashed_deal_detail_1   | Classified feature by order No. 1                        |
| Hashed_deal_detail_2   | Classified feature by order No. 2                        |
| Hashed_deal_detail_3   | Classified feature by order No. 3                        |
| Hashed_deal_detail_4   | Classified feature by order No. 4                        |
| Hashed_deal_detail_5   | Classified feature by order No. 5                        |
| Hashed_deal_detail_6   | Classified feature by order No. 6                        |
| Age                    | Age of the gnome who made the order                      |
| Gender                 | The gender of the gnome who made the order               |
| Default                | Did the gnome default on this purchase? 1 - yes, 0 - no. |

## Metric

PR-AUC

## Requirements

It is expected that the csv format prediction file contains two columns - Deal_id and Prediction, where the first column means the unique identifier of the order, and the second - the probability that the orderer will not return the money.

| Deal_id  | Prediction |
|----------|------------|
| 22487461 |      1     |
| 62494261 |     0.93   |
| 34822849 |     0.07   |
| 46893387 |     0.34   |
| 67128275 |     0.568  |
