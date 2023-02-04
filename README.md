# Data Driven Modelling Project

The final project of the TH Köln module "Data Driven Modelling" (https://digital-sciences.de/en/modules/data-driven-modelling/) as part of the Digital Sciences Master's Degree.

The dataset contains information on supermarket fridges, including temperatures of the fridges and heat pumps, outside temperatures, humidity, the energy used in kW to power the fridges, and more. On a given date these fridges had had their door seals changed to a new type of material, and the aim of this project was to analyse this dataset in order to answer the research question: "Was it worth it to change the door seal?"

As the dataset contains real proprietary data from a German company, **only the analysis code is available in this repository, and the original dataset is not made public**.

## Project Files

The code is provided in Jupyter notebooks:
[1. Data Exploration](https://github.com/Natasha-R/Data-Driven-Modelling-Project/blob/main/1.%20Data%20Exploration.ipynb)
[2. Data Pre-Processing](https://github.com/Natasha-R/Data-Driven-Modelling-Project/blob/main/2.%20Data%20Pre-Processing.ipynb)
[3. Data Modelling](https://github.com/Natasha-R/Data-Driven-Modelling-Project/blob/main/3.%20Data%20Modelling.ipynb)

The slides used in the final project presentation are also provided, along with the documentation utilised in project milestones:
[DDM Project Presentation](https://github.com/Natasha-R/Data-Driven-Modelling-Project/blob/main/DDMProjectPresentation.pdf)
[DDM Project Documentation](https://github.com/Natasha-R/Data-Driven-Modelling-Project/blob/main/DDMProjectDocumentation.xlsx)

## Project Results

* The modelling approach taken in this project was to use a multiple linear regression model with "chilling power" as the dependent variable, and other features, including a binary "before/after door seal change" feature as the independent variables.   
* The "door seal change" feature was significant with a negative coefficient, suggesting that the seal change had reduced the amount of energy required to chill the fridges and thus that it was worth it to change the door seal.
* However the final conclusion noted that the seal change feature was confounded with time, therefore any other changes over time could also have influenced the effect; e.g. if the contents of the fridges were also changed before/after the door seal was changed, thus affecting heat capacities and subsequently chilling energy required. The data also contained no control group; it was not known if simply replacing old degraded door seals with a new door seal of the old material would have been just as effective.
