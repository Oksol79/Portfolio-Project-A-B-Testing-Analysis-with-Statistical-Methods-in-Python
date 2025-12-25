# Portfolio Project A/B Testing Analysis with Statistical Methods in Python

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
6. Scipy.stats for:
   - norm.cdf;
   - z-test for two proportions;
   - p-value calculation;
   - basic statistics.
7. Statsmodels.stats.multitest.multipletests for:
   - multiple testing correction;
   - Bonferroni.

## **Methods:**
- A/B testing;
- z-test for proportions;
- conversion rate analysis;
- multiple testing correction;
- segmentation analysis.

## **Dataset:**
The dataset was created using a SQL query against tables in the BigQuery database. The dataset contained the following fields: date, country, device, continent, channel, test, test_group, event_name, and value. The event_name field represents user events and metrics used to analyze A/B testing results and conversion behavior in the sales funnel, including: add_payment_info, add_shipping_info, add_to_cart, begin_checkout, click, first_visit, new_account, page_view, scroll, select_item, select_promotion, session, session_with_orders, session_start, user_engagement, view_item, view_item_list, view_promotion, and view_search_results. Appropriate table joins were applied during the dataset creation, and UNION ALL was used to combine event-level data from multiple sources into a single analytical dataset.

## **List of tasks:**

## **Demonstrated Skills:**
