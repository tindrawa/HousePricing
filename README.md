# HousePricing
Project Overview
The project involves a comprehensive analysis of residential property data, focusing on various attributes that could influence the sale price. The dataset includes a wide range of features, from the type of dwelling and zoning classification to specific details about the property’s physical characteristics and condition.

Key Features Analyzed
Dwelling Type and Zoning:
MSSubClass: Identifies the type of dwelling involved in the sale (e.g., 1-story, 2-story, duplex).
MSZoning: General zoning classification (e.g., Residential, Commercial, Industrial).
Lot and Property Characteristics:
LotFrontage: Linear feet of street connected to the property.
LotArea: Lot size in square feet.
Street and Alley: Type of road and alley access (e.g., paved, gravel).
Property Shape and Contour:
LotShape: General shape of the property (e.g., regular, irregular).
LandContour: Flatness of the property (e.g., level, hillside).
Utilities and Configuration:
Utilities: Type of utilities available (e.g., all public utilities, electricity only).
LotConfig: Lot configuration (e.g., inside lot, corner lot).
Neighborhood and Condition:
Neighborhood: Physical locations within city limits.
Condition1 and Condition2: Proximity to various conditions (e.g., arterial street, railroad).
Building and House Style:
BldgType: Type of dwelling (e.g., single-family, duplex).
HouseStyle: Style of dwelling (e.g., one story, two story).
Quality and Condition Ratings:
OverallQual: Rates the overall material and finish of the house.
OverallCond: Rates the overall condition of the house.
Construction and Remodel Dates:
YearBuilt: Original construction date.
YearRemodAdd: Remodel date.
Roof and Exterior:
RoofStyle and RoofMatl: Type and material of the roof.
Exterior1st and Exterior2nd: Exterior covering on the house.
Foundation and Basement:
Foundation: Type of foundation (e.g., brick, concrete).
BsmtQual, BsmtCond: Quality and condition of the basement.
Heating and Electrical Systems:
Heating: Type of heating system.
HeatingQC: Heating quality and condition.
Electrical: Electrical system type.
Living Area and Rooms:
1stFlrSF, 2ndFlrSF: First and second floor square feet.
GrLivArea: Above grade living area square feet.
TotRmsAbvGrd: Total rooms above grade.
Bathrooms and Kitchens:
FullBath, HalfBath: Full and half bathrooms above grade.
KitchenQual: Kitchen quality.
Garage and Parking:
GarageType: Garage location.
GarageCars, GarageArea: Size of garage in car capacity and square feet.
GarageQual, GarageCond: Quality and condition of the garage.
Porches and Decks:
WoodDeckSF, OpenPorchSF: Wood deck and open porch area in square feet.
EnclosedPorch, 3SsnPorch, ScreenPorch: Enclosed, three-season, and screen porch area in square feet.
Miscellaneous Features:
PoolArea, PoolQC: Pool area and quality.
Fence: Fence quality.
MiscFeature: Miscellaneous features not covered in other categories.
Sale Information:
MoSold, YrSold: Month and year sold.
SaleType: Type of sale (e.g., warranty deed, contract).
SaleCondition: Condition of sale (e.g., normal, foreclosure).
Purpose and Goals
The primary goal of this project is to identify and analyze the factors that significantly impact the sale price of residential properties. By understanding these factors, stakeholders such as real estate agents, property developers, and potential buyers can make more informed decisions. The analysis aims to:

Determine Key Influencers: Identify which features have the most significant impact on sale prices.
Predict Sale Prices: Develop models to predict the sale price of properties based on their attributes.
Improve Property Valuation: Enhance the accuracy of property valuations by considering a comprehensive set of features.
Guide Investment Decisions: Provide insights that can guide investment decisions in the real estate market.
Methodology
The project involves several steps, including data cleaning, exploratory data analysis (EDA), feature engineering, and model building. Key methodologies include:

Data Cleaning: Handling missing values, correcting data types, and removing outliers.
Exploratory Data Analysis: Visualizing data distributions, relationships, and correlations.
Feature Engineering: Creating new features from existing ones to improve model performance.
Model Building: Using machine learning algorithms to build predictive models.
Conclusion
This project provides a detailed analysis of residential property features to understand their impact on sale prices. By leveraging data science techniques, the project aims to offer valuable insights into the real estate market, ultimately helping stakeholders make better-informed decisions.

• Ridge Regression:

Train Performance: MSE of 685,599,102.97, RMSE of 26,183.95, R^2 Score of 0.885.

Test Performance: MSE of 706,342,523.93, RMSE of 26,577.11, R^2 Score of 0.908.

Insight: While Ridge Regression is simple and interpretable, its performance suggests it might be less effective with non-linear relationships.

• Lasso Regression:

Train Performance: MSE of 1,544,248,645.42, RMSE of 39,296.93, R^2 Score of 0.741.

Test Performance: MSE of 939,136,056.32, RMSE of 30,645.33, R^2 Score of 0.878.

Insight: Lasso Regression shows less accuracy and higher error compared to Ridge Regression, highlighting limitations with feature selection and regularization.

• Random Forest:

Train Performance: MSE of 0.00, RMSE of 0.00, R^2 Score of 1.000.

Test Performance: MSE of 981,304,192.71, RMSE of 31,325.78, R^2 Score of 0.872.

Insight: Excellent on training data but performs less well on test data, indicating potential overfitting. Nevertheless, it handles complex interactions well.

• XGBoost:

Train Performance: MSE of 158,478,529.12, RMSE of 12,588.83, R^2 Score of 0.973.

Test Performance: MSE of 766,298,981.98, RMSE of 27,682.11, R^2 Score of 0.900.

Insight: Provides high accuracy and performs well on both training and test data, indicating robustness and effectiveness in handling complex data.
