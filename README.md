# Price Prediction of Pre-owned Cars

## Table of Contents

- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Steps Performed](steps-performed)
- [Results](#results)
- [Acknowledgements](#acknowledgements)

---

## Problem Statement

Storm Motors is an e-commerce company who act as mediators between parties interested in selling and buying pre-owned cars. For the year 2015-2016, they have recorded data about the seller and car including: - Specification details, Condition of car, Seller details, Registration details, Web advertisement details, Make and model information and Price. The company wishes to develop an algorithm to predict the price of the cars based on various attributes associated with the car.

## Dataset

Here is the dataset description:
| Variables | Datatype | Description |
|----------|----------|-------------|
| dateCrawled | date | date when the ad first crawled |
| name | string | string consisting of car name, brand, model etc. |
| seller | string | nature of seller |
| offerType | string | whether the car is on offer or the buyer requested an offer |
| price | integer | price on the ad to sell the car |
| abtest | string | two versions of ad |
| vehicleType | string | types of cars |
| yearOfRegistration | integer | year in which car was registered |
| gearbox | string | type of gearbox |
| powerPS | integer | HP |
| model | string | model type |
| kilometers | integer | kilometers car has travelled |
| monthOfRegistration | integer | month of registration |
| fuelType | string | types of fuel |
| brand | string | make of a car |
| notRepairedDamage | string | status of repair for damages (yes, if damage not rectified) |
| dateCreated | date | date on which the ad was created |
| postalCode | integer | postal code of seller |
| lastSeen | date | when the crawler saw the ad last online |

## Technologies Used

- Python
- Pandas
- Matplotlib, Seaborn
- Scikit-Learn
- Jupyter Notebook


## Steps Performed
- Libraries imported.
- Load dataset.
- Removed unwanted columns (dateCrawled, name, postalCode, dateCreated, lastSeen).
- Removed duplicates.
- Data Cleaning - removing extreme values from (yearOfRegistration, price, powerPS) and formatted the 'age' column.
- Finding insignificant vaiables with the help of visualisations.
- Dropping insignificant variables and null values.
- Model building (omitted data) - base model, linear regression model, random forest model.
- Model building (imputed data) - base model, linear regression model, random forest model.
- Compared models' accuracy with both omitted & imputed data.
