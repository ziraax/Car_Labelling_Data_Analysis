# Car Labelling Dataset Analysis

![Car Labelling](https://img.shields.io/badge/Car%20Labelling-Dataset-blue)

This README provides an overview of the data analysis conducted on the "Car Labelling" dataset from ADEME France. The analysis aims to explore and understand the dataset, perform data preprocessing, conduct exploratory data analysis (EDA), and provide insights into various aspects of car information. Below, you will find information on the dataset, the analysis process, the technology stack used, and key findings.

## About "Car Labelling" and ADEME

"Car Labelling" is a platform that offers an analytical view of the new car market. It provides valuable insights into various aspects of the automotive industry, including information on the environmental impact of vehicles. In addition to this platform, ADEME (Agence de la transition écologique) makes available source data, which has been curated from diverse sources and refined. These data sources serve as the foundation for the "Car Labelling" platform and are intended to support the emergence of new applications that promote the acquisition of vehicles with a lower environmental impact. These data can also be used for further analyses to inform decision-makers and vehicle buyers.

[Download Data](https://www.data.gouv.fr/fr/datasets/ademe-car-labelling/)


## Dataset Description

The "Car Labelling" dataset from ADEME France contains information about various aspects of cars, including their energy source, brand, power, emissions, and more. The dataset is structured as a CSV file with several columns. Here are some of the key columns in the dataset:

- **Energie**: The type of energy source used by the vehicle.
- **Marque**: The brand of the vehicle.
- **Puissance fiscale**: The fiscal power of the vehicle.
- **Puissance maximale**: The maximum power of the vehicle.
- **CO2 vitesse mixte Avg**: The average CO2 emissions of the vehicle under mixed speed conditions.
- **Poids à vide**: The empty weight of the vehicle.
- **Prix véhicule**: The price of the vehicle.
- **Essai particules**: Information about particle emissions.

## Technology Stack

The data analysis was performed using Python and various libraries. Here's a list of the main libraries and tools used:

- Python: The primary programming language for data analysis.
- Pandas: Used for data manipulation and preprocessing.
- Matplotlib and Seaborn: Utilized for data visualization and plotting.
- Scikit-Learn: Used for K-Means clustering analysis.

## Data Preprocessing

The data preprocessing steps included handling missing values by filling them with appropriate values based on the column type. Additionally, columns with minimum and maximum values were merged to create an average column for certain attributes. The preprocessed data was saved as "Preprocessed_data.csv" for further analysis.

## Exploratory Data Analysis (EDA)

The EDA section explored various aspects of the dataset, including:

- Distribution of energy types among vehicles.
- Distribution of vehicle brands.
- Analysis of power-related variables.
- Analysis of CO2 emissions.
- Relationships between weight, power, consumption, and emissions.
- Clustering analysis to identify patterns in weight and consumption.

## Key Findings

Some key findings from the analysis include:

- The distribution of energy types showed a significant presence of diesel and gasoline vehicles.
- Certain vehicle brands were more prevalent in the dataset.
- Power-related variables exhibited various distributions and relationships.
- CO2 emissions varied across different vehicle brands and energy types.

One noteworthy observation is the strong correlation between weight and both consumption and CO2 emissions. Heavier vehicles tend to have higher consumption and emissions, emphasizing the importance of vehicle weight in environmental impact assessments.

![weight-consumptionEmissions](/data_viz/PoidsAVide_Conso-CO2.png)

Similarly, there is a notable correlation between the price of the vehicle and its environmental characteristics. Higher-priced vehicles often exhibit lower emissions, indicating a potential link between cost and environmental performance.

![weight-consumptionEmissions](/data_viz/Prix_Conso-C02.png)


- Clustering analysis revealed patterns in vehicle weight and consumption.

These findings underscore the significance of vehicle weight and price as influential factors in the context of consumption, emissions, and environmental impact, which can be valuable insights for consumers and policymakers.

![weight-consumptionEmissions](/data_viz/Dsitrib_CO2_marque.png)


## Conclusion

This repository provides an overview of the analysis conducted on the Car Labelling dataset from ADEME France. The analysis aimed to explore and understand various aspects of the dataset, and key findings were highlighted. The provided code and visualizations offer insights into the characteristics of vehicles, which can be valuable for further research or decision-making related to environmental impact and energy-efficient transportation.
