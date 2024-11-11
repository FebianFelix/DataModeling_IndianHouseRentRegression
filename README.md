# Indian House Rent Regression

This project focuses on developing a regression model to predict house rental prices in various cities across India. By examining multiple factors such as the number of bedrooms, property size, furnishing status, and other amenities, this project aims to provide insights and predictions for the rental housing market.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Technologies and Libraries](#technologies-and-libraries)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Preparation](#data-preparation)
- [Modeling](#modeling)
- [Evaluation Metrics](#evaluation-metrics)
- [Web Deployment](#web-deployment)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The aim of this project is to predict house rental prices in India using linear regression techniques, specifically **Linear Regression** and **Lasso Regression**. It also includes a web-based application built using the Flask framework, enabling users to input house details and obtain predicted rental prices.

## Dataset

- **Source**: Kaggle (contributed by Sourav Banerjee)
- **Details**: This dataset contains information on house rentals in major Indian cities, including:
  - **City**: Location of the property
  - **Size**: Area of the house
  - **BHK**: Number of bedrooms
  - **Bathrooms**: Number of bathrooms
  - **Furnishing Status**: Whether the property is furnished
  - **Amenities**: Availability of additional facilities
  - **Tenant Preferences**: Who the property is suited for (e.g., families, bachelors)
  - **Contact Method**: Preferred method for property inquiries
  - **Other factors** relevant to house rental prices

## Technologies and Libraries

- **Python**: Core language for data analysis and model building
- **Jupyter Notebook**: Environment for data exploration and preprocessing
- **Flask**: Web framework for deployment
- **Libraries**:
  - **Pandas** and **NumPy** for data manipulation
  - **Matplotlib** and **Seaborn** for data visualization
  - **scikit-learn** for machine learning algorithms and evaluation metrics

## Exploratory Data Analysis (EDA)

Key steps in EDA include:
- Checking for missing values and outliers
- Visualizing distributions of critical variables like **BHK**, **Size**, **Bathroom**, and **Rent**
- Understanding relationships between features through correlation analysis and scatter plots

## Data Preparation

- **Outlier Removal**: Outliers in numeric variables were removed using the **Interquartile Range (IQR)** method to improve model performance.
- **Encoding**: Categorical variables were encoded to be compatible with regression models.
- **Assumption Testing**: Regression assumptions like linearity, homoscedasticity, and multicollinearity were validated to ensure data compatibility with linear regression techniques.

## Modeling

Two main models were developed and evaluated:
1. **Linear Regression**: Basic regression model to capture the relationship between features and rental prices.
2. **Lasso Regression**: Adds regularization to improve model performance and feature selection by reducing less impactful variables.

## Evaluation Metrics

The models were evaluated using the following metrics:
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **R-squared (R2)**

The performance of Lasso Regression was particularly notable due to its regularization, making it more robust by eliminating unimportant features.

## Web Deployment

The model was deployed using Flask, allowing users to interact with the predictive model via a web interface. Key functionalities of the application include:
- **User Input**: Fields for users to enter house details such as size, number of bedrooms, and furnishing status.
- **Prediction Output**: Immediate display of the predicted rental price based on user input.
  
## Installation

To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/FebianFelix/DataModeling_IndianHouseRentRegression.git
    ```
2. Navigate into the project directory:
    ```bash
    cd DataModeling_IndianHouseRentRegression
    ```
3. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Start the Flask application:
    ```bash
    python app.py
    ```

## Usage

1. Access the web app at `http://localhost:5000`.
2. Fill in the form with the required house details.
3. Click the "Predict" button to get the estimated rent.

## Contributing

To contribute:
1. Fork this repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE.md](LICENSE.md) file for more details.
