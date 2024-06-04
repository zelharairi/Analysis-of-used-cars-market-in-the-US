# Analysis of used car market in the US

## Overview
This project analyzes a dataset of used car prices in the United States from 2000 to 2023. It utilizes various data processing techniques to explore trends and patterns in the data. The primary focus is on understanding how different factors such as manufacturing year, car brand, color, and mileage influence the price and accident rate of used cars.

## Dataset
The dataset used for this project is sourced from Kaggle and can be found [here](https://www.kaggle.com/datasets/ayaz11/used-car-price-prediction). It includes data on various attributes of used cars such as:
- Brand
- Mileage
- Price
- Car color (exterior and interior)
- Condition (number of owners and accidents)

## Dataframes
The dataset is divided into three dataframes based on the manufacturing years:
1. **Dataframe 1**: Cars manufactured in 2022 and 2023
2. **Dataframe 2**: Cars manufactured in 2020 and 2021
3. **Dataframe 3**: Cars manufactured in 2018 and 2019

This division allows for a focused analysis on the changes over the previous six years and the impact of different conditions on car prices.

## Queries and Analysis
The project performs the following queries to derive insights from the dataset:

### Query 1 and 2: Maximum and Minimum Prices
- **Objective**: To find the maximum and minimum prices of cars for each year.
- **Hypothesis**: The maximum price for each year should be higher in the newer models and the minimum price should be lower.
- **Result**: The hypothesis was correct for the minimum prices but not for the maximum prices due to the presence of high-value cars like Rolls Royce in the older models.

### Query 3: Most Common Car Brand and Model for Sale Each Year
- **Objective**: To identify the most common car brand and model for sale each year.
- **Method**: Group by each car brand and model, count occurrences, and find the maximum count for each year.

### Query 4: Ratio of Accidents to Car Color
- **Objective**: To test if red cars result in more accidents.
- **Method**: Functions were created to retrieve exterior color and number of accidents for each car. The ratio of cars in accidents to total cars for each color was calculated.
- **Result**: Higher percentage of grey cars were in accidents compared to other colors.

### Query 5: Ratio of Accidents to Car Mileage
- **Objective**: To analyze how mileage affects the number of accidents.
- **Method**: Created ranges for mileage and computed the average number of accidents for each range.
- **Result**: Cars with higher mileage tend to have more accidents.

### Query 6: Ratio of Accidents to Car Brand
- **Objective**: To determine if certain car brands are more prone to accidents.
- **Method**: Group by brand and accidents, compute the ratio.
- **Result**: GMC cars had the highest percentage of accidents, while Porsche had the least.

### Query 7: Average Miles for Cars Each Year
- **Objective**: To find the average mileage for cars each manufacturing year.
- **Method**: Created a function to convert mileage to integer and computed the average for each year.
- **Result**: Older car models tend to have higher average mileage.

## Results
- Detailed results for Query 6 can be found in the `result6.csv` file.
- Visualizations and graphs for the queries are included in the subsequent slides of the provided presentation.

## How to Run the Project
1. Clone the repository:
    ```sh
    git clone https://github.com/username/repository.git
    ```
2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```
3. Run the analysis scripts:
    ```sh
    python analysis.py
    ```

## Contributors
- Ziad El Harairi

## License
This project is licensed under the [MIT](https://choosealicense.com/licenses/mit/) License.