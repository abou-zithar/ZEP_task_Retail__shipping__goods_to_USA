# Truck Trip Analysis and Prediction

This project involves analyzing truck trip data, calculating distances between locations, and predicting trip durations. The project uses various libraries like Pandas, NumPy, Matplotlib, and Seaborn for data manipulation, analysis, and visualization. It also uses machine learning techniques from Scikit-learn for prediction.

## Prerequisites

Before running the code, make sure to have the following libraries installed:

- `pandas`: Install using `pip install pandas`
- `numpy`: Install using `pip install numpy`
- `matplotlib`: Install using `pip install matplotlib`
- `seaborn`: Install using `pip install seaborn`
- `scikit-learn`: Install using `pip install scikit-learn`

Additionally, you need to have access to the dataset file (`ZepDataSet.xlsx`) from your Google Drive.

## Data Loading and Exploration

- The data is loaded from the Excel file using Pandas and parsed as datetime for specific columns.
- The structure of the data is explored using `.head()` and `.tail()` functions.

## Distance Calculation

- A function `get_distance` is defined to calculate the distance between two points using the haversine formula.
- Distances are calculated for each pair of latitude and longitude coordinates.

## Trip Distance Analysis

- Trip distances and corresponding truck IDs are calculated and analyzed.

## Data Preprocessing

- Date and time features are extracted from the columns and used to calculate differences in hours.
- New date and time features are created and unnecessary columns are dropped.

## Data Visualization

- Seaborn and Matplotlib are used to create various visualizations, including KDE and histogram plots.

## Feature Engineering

- New features are created using date and time components.
- One-hot encoding is applied to categorical features.

## Dimensionality Reduction

- Principal Component Analysis (PCA) is applied to reduce the dimensionality of the dataset.
- The variance explained by each component is plotted.

## Model Building and Evaluation

- A RandomForestRegressor is trained on the preprocessed data.
- Predictions are made and evaluated using mean absolute error and mean squared error.

## Note

- The project assumes that you have the dataset file (`ZepDataSet.xlsx`) available in your Google Drive.
- Adjust the path to the dataset file as needed based on your directory structure.

## Author

Created by Mahmoud Abou Zithar

## License

This project is licensed under the [MIT License](LICENSE).
