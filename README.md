# Home-LLC-assignment

# S&P/Case-Shiller Home Price Index Analysis
# Objective
The primary goal of this project is to conduct a comprehensive analysis of publicly available data related to economic, demographic, and real estate indicators. The ultimate aim is to build a predictive model that elucidates the influence of these factors on the S&P/Case-Shiller Home Price Index, a crucial indicator of U.S. home prices, spanning the last two decades.

# Introduction
The S&P CoreLogic Case-Shiller Home Price Indices are pivotal in monitoring the price levels of single-family homes in the United States. These indices offer valuable insights into the dynamic housing market, providing a nationwide perspective on the overall value of single-family homes. By aggregating data from nine different regions and updating on a monthly basis, the S&P CoreLogic Case-Shiller U.S. National Home Price Index is a key component of this system. The analysis extends to city indices, covering 20 major metropolitan areas, further grouped into two composites. These indices have the unique capability to measure percentage changes in housing market prices while maintaining a consistent level of quality, excluding variations due to house types, sizes, or physical characteristics.

# Data and Methodology
# 3.1 Data Collection
Data for various features was identified through a literature survey of The S&P CoreLogic Case-Shiller Home Price Indices. The majority of the data was collected from FRED (Federal Reserve Economic Data).

CSUSHPISA: S&P/Case-Shiller U.S. National Home Price Index

Units: Index Jan 2000=100, Seasonally Adjusted
Source
HNFSEPUSSA: New One Family Homes for Sale in the United States

Units: Thousands of Units, Seasonally Adjusted
Source
HOUST1F: New Privately-Owned Housing Units Started: Single-Family Units

Units: Thousands of Units, Seasonally Adjusted Annual Rate
Source
... (and so on)

# 3.2 Data Preparation
The NASDAQ Composite Index, initially with a daily frequency, was converted to monthly data by averaging daily values.
Features with quarterly frequency remained unchanged for the next two months to align with monthly data.
All features were merged using the date as a common key.
The assumption made for the S&P Case-Shiller data is that each data point is considered independently, without considering temporal or sequential relationships between data points.
# 3.3 Exploratory Data Analysis
Exploratory Data Analysis (EDA) was conducted to extract essential insights and identify significant features. Refer to the Final_report.pdf for a detailed analysis.

# 3.4 Model Selection and Evaluation
Lasso, Ridge, and Elastic Net regression models were chosen for development to assess the influence of various factors on the S&P/Case-Shiller Home Price Index. R-squared values were used for model evaluation, with higher values indicating better performance.

# Result and Discussion
# 4.1 Exploratory Data Analysis
Key insights from EDA, including the relationship between various features and the S&P Home Price Index, are detailed in the Final_report.pdf.
# 4.2 Correlation Matrix
The correlation matrix analysis highlights the top 5 correlated factors with the S&P/Case-Shiller Home Price Index.
# 4.3 Machine Learning Models
Lasso, Ridge, and Elastic Net regression models were analyzed. Elastic Net regression, striking a balance between Lasso and Ridge, was chosen for its ability to achieve a good R-squared and identify important parameters.
# 5. Conclusions
A summary of the important features identified by the Elastic Net model, along with their impact on the S&P Home Price Index.
For a comprehensive understanding, please refer to the detailed analysis in the Final_report.pdf.
