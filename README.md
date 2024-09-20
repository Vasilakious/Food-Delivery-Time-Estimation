# Food Delivery Time Estimation

This Python application estimates delivery times for food orders using a large dataset from Kaggle. By applying various algorithms and mathematical functions, we identify the data points that have a significant impact on the delivery time.

## Table of Contents

- [Tech Stack](#tech-stack)
- [Haversine Function](#haversine-function)
- [Data Loading](#data-loading)
- [Data Exploration](#data-exploration)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Correlation Analysis](#correlation-analysis)
- [Geospatial Visualization](#geospatial-visualization)
- [Temporal Analysis](#temporal-analysis)
- [Age Distribution](#age-distribution)
- [Application Showcase](#application-showcase)

## Tech Stack

We use Python 3.10.8 as the programming language for this project. The application is developed using the Replit environment, which supports a wide range of libraries that are essential for the analysis.

### Libraries Used:
- **NumPy**: For numerical computations.
- **Pandas**: For data manipulation and analysis.
- **OS**: To interact with the file system.
- **Matplotlib**: For plotting basic visualizations.
- **PySpark**: For large-scale data processing.
- **Seaborn**: For statistical data visualization.

## Haversine Function

We define a `haversine` function to compute the distance between geographic coordinates (latitude and longitude) using the Haversine formula.

![image](https://github.com/user-attachments/assets/83615575-87be-4bf9-af17-dbee5258ab79)

## Data Loading

In this step, we load a dataset named `food_delivery_time.csv` into a Pandas DataFrame called `data_frame`.

## Data Exploration

1.  Display the first and last five rows of the dataset to get a quick overview of the data.
2.  Print information about the DataFrame, such as the number of entries, data types, and memory usage.
3.  Identify and print columns containing categorical and numerical data separately.
4. Check for missing values in the dataset.
5.  Check for duplicate rows in the dataset.

## Exploratory Data Analysis (EDA)

1. **Statistical Summary**:
   - Use the `describe` function to generate basic statistics for the numerical columns.
   
2. **Visualizations with Seaborn**:
   - **Order Types and Vehicle Types**: Plot the counts of different order types and vehicle types.
   - **Top IDs**: Display bar charts for the top 5 order IDs and top 5 delivery driver IDs.
   - **Correlation Heatmap**: Create a heatmap to visualize the correlations between numerical features.

## Correlation Analysis

- We calculate the correlation between each numerical column and the `Time_taken(min)` column.
- Visualize these correlations using a bar chart.
- This helps us identify the relevant variables that impact the delivery time.

![image](https://github.com/user-attachments/assets/bca06b42-2f1e-4ebb-96c5-1697f841ae47)

## Geospatial Visualization

- Create a scatter plot to represent the geographic locations of restaurants and delivery points using latitude and longitude.

![image](https://github.com/user-attachments/assets/6a5b9a2a-e8f1-45b0-9956-6d0d492bac0b)

- Compute the distance between the restaurants and delivery points using the Haversine function, adding a new column `distance` to the DataFrame.

## Temporal Analysis

- We analyze the distribution of delivery times based on the type of vehicle used by plotting kernel density estimation (KDE) plots.

![image](https://github.com/user-attachments/assets/2f41f238-8f9b-4088-86da-164a2dfc260b)

## Age Distribution

- Visualize the age distribution of delivery drivers using a histogram.

![image](https://github.com/user-attachments/assets/eec3e156-af17-4c4d-9586-b895c98fefaf)

## Application Showcase

Below, we will showcase pictures from the Streamlit application that demonstrate how the Food Delivery Time Estimation tool works. Stay tuned for screenshots!

---
### First Look on our Application and the variables we can input to have a precise calculation
![First-Look](https://github.com/user-attachments/assets/d566b612-8ea6-4ea3-9204-e3f55c2a1cc9)

---
### Our results by using the default options in the application
![DefaultOptions](https://github.com/user-attachments/assets/48df8f64-9399-4dcf-ae20-2d3b63a4047d)

---
### Our vast selection of Training Algorithms to showcase the difference between the capabilities of each algorithm on the specific dataset
![Algorithms](https://github.com/user-attachments/assets/924ba01d-5b04-45aa-9f1f-c32a1a254878)
