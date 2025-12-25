# Portfolio Project - A/B Testing Analysis with Statistical Methods in Python

## **Description:**
This portfolio demonstrates a project on analyzing A/B testing results using statistical methods in Python. The calculation of statistical significance is demonstrated using a Python script. For better understanding, visualizations are included showing key conversion metrics and statistical significance for four metrics (add_payment_info, add_shipping_info, begin_checkout, and new_accounts).  
A two-proportion z-test was used to evaluate the effectiveness of A/B testing. The analysis was performed for the tests as a whole, as well as for segments by continent, country, and device.

## **Tools & Environment:**
- Google Colab.
- Google Drive (google.colab.drive).
  
## **Technologies & Libraries:**
1. BigQuery / SQL API (client.query)
2. Python for data analysis.
3. Pandas for data manipulation.
4. NumPy for numerical computing.
5. Matplotlib & Seaborn for data visualization.
6. SciPy.stats for:
   - norm.cdf;
   - z-test for two proportions;
   - p-value calculation;
   - basic statistics.
7. Statsmodels.stats.multitest.multipletests for:
   - multiple testing correction;
   - FDR;
   - Bonferroni.

## **Methods:**
- A/B testing.
- Robust two-sided Z-test for proportions (pooled).
- Conversion rate analysis.
- Multiple testing correction.
- Segmentation analysis.

## **Dataset:**
The dataset was created using a SQL query against tables in the BigQuery database. The dataset contained the following fields: date, country, device, continent, channel, test, test_group, event_name, and value. The event_name field represents user events and metrics used to analyze A/B testing results and conversion behavior in the sales funnel, including: add_payment_info, add_shipping_info, add_to_cart, begin_checkout, click, first_visit, new_account, page_view, scroll, select_item, select_promotion, session, session_with_orders, session_start, user_engagement, view_item, view_item_list, view_promotion, and view_search_results. Appropriate table joins were applied during the dataset creation, and UNION ALL was used to combine event-level data from multiple sources into a single analytical dataset.

## **List of tasks:**
1. Connecting to a database.
2. Description of the received dataset.
3. Calculation of statistical significance.  
   3.1. Setting up conversion metrics.  
   3.2. Calculating significance in total for the test.  
   3.3. Saving results to disk for basic metrics.  
   3.4. Visualization of results for each test.  
   3.5. Analysis of basic metrics by continent.  
   3.6. Analysis of basic metrics by country.  
   3.7. Analysis of basic metrics by device.  
4. Overall Сonclusion.
5. Results file.
6. Dashboard in Tableau Public.

## **Key Features & Skills:**
1. Data Analysis & Preparation:
  - Worked with real user event data extracted from analytics systems.
  - Performed event-level analysis, understanding event structure (event_name, value).
  - Transformed data from long to wide format for downstream analysis.
2. Data Cleaning & Validation:
  - Checked for NaN, empty, or pseudo-missing values.
  - Validated data types (datetime, Int64) and logical consistency (e.g., events ≤ sessions).
  - Ensured dataset integrity for reliable statistical analysis.
3. Statistical Significance Calculation:
  - Applied appropriate statistical tests for each metric (e.g., z-test for proportions).
  - Calculated Conversion Rates (CR), z-scores, and p-values.
  - Conducted analysis across multiple metrics simultaneously (4 conversion metrics).
4. Segmentation Analysis:
  - Performed A/B test analysis across various segments (Continents, Countries, Devices)/
  - Evaluated false positive risk and applied multiple testing correction (FDR).
5. Data Visualization:
  - Created analytical visualizations using matplotlib.
  - Provided clear visual interpretation of A/B test results for decision-making.
6. SQL & Google Colab Integration:
  - Extracted datasets via SQL queries from BigQuery.
  - Worked in Google Colab environment and saved results to Google Drive.
