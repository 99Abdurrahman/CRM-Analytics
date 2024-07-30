# CLTV and RFM Analysis Using BG-NBD and Gamma-Gamma Models

## Project Overview
This project involves analyzing customer behavior data from the FLO dataset to predict Customer Lifetime Value (CLTV) and conduct Recency, Frequency, Monetary (RFM) analysis. The dataset includes information on customer transactions from both online and offline channels during 2020 and 2021. The BG-NBD and Gamma-Gamma models are used for CLTV prediction.

## Business Problems
### 1. CLTV Prediction and RFM Analysis
One of the most important problems in e-commerce is predicting Customer Lifetime Value (CLTV) accurately. By understanding the value of each customer, businesses can tailor their marketing strategies, improve customer retention, and optimize resources. Additionally, conducting RFM analysis helps segment customers based on their purchasing behavior, allowing for more personalized marketing efforts.

#### Dataset
The dataset consists of the following columns:
- `master_id`: Unique customer ID
- `order_channel`: The platform used for shopping (Android, iOS, Desktop, Mobile, Offline)
- `last_order_channel`: The channel used for the last purchase
- `first_order_date`: The date of the customer's first purchase
- `last_order_date`: The date of the customer's most recent purchase
- `last_order_date_online`: The date of the customer's most recent online purchase
- `last_order_date_offline`: The date of the customer's most recent offline purchase
- `order_num_total_ever_online`: Total number of purchases made by the customer online
- `order_num_total_ever_offline`: Total number of purchases made by the customer offline
- `customer_value_total_ever_online`: Total amount spent by the customer on online purchases
- `customer_value_total_ever_offline`: Total amount spent by the customer on offline purchases
- `interested_in_categories_12`: List of categories the customer has shopped in the last 12 months

### 2. Comparison of A/B Test and Conversion of Bidding Methods
Facebook recently introduced a new type of bidding, “average bidding”, as an alternative to the existing type of bidding called “maximum bidding”. One of our clients, bombabomba.com, decided to test this new feature and run an A/B test to see if average bidding brings more conversions than maximum bidding. The ultimate success metric for bombabomba.com is Purchase. Therefore, for statistical testing, the focus is on the Purchase metric.

#### Dataset
This dataset, which contains a company's website information, includes information such as the number of advertisements seen and clicked by users, as well as information about the earnings from these advertisements. There are two separate datasets for the Control and Test groups. Maximum Bidding was applied to the control group and Average Bidding to the test group.

#### Variables:
- `impression`: Number of ad views
- `Click`: Number of clicks on the displayed ad
- `Purchase`: Number of products purchased after clicking ads
- `Earning`: Earnings from purchased products

## Methodology
### Data Preprocessing
- Data cleaning and preparation.
- Aggregating customer transaction data to calculate:
  - Total number of purchases (online and offline).
  - Total monetary value of purchases (online and offline).
- Calculating Recency, Frequency, and Monetary (RFM) values for each customer.

### CLTV Prediction
Using the BG-NBD and Gamma-Gamma models to predict CLTV:
- **BG-NBD Model**: Estimates the expected number of transactions a customer will make in the future.
- **Gamma-Gamma Model**: Estimates the average monetary value of transactions for each customer.

## Notebooks
The repository includes the following Jupyter notebooks:
1. **CLTV_RFM_Analysis.ipynb**: This notebook contains the solution to the problem of predicting CLTV and conducting RFM analysis.
2. **AB_Test_Analysis.ipynb**: This notebook contains the solution to the problem of comparing A/B test results for different bidding methods.

## How to Run the Notebooks
1. Clone the repository:
    ```bash
    git clone https://github.com/99Abdurrahman/CRM-Analytics.git
    ```
2. Navigate to the repository directory:
    ```bash
    cd CRM-Analytics
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Open the Jupyter notebooks:
    ```bash
    jupyter notebook
    ```
## Acknowledgements
- The dataset is sourced from FLO.

Feel free to reach out if you have any questions or suggestions!

---

**Author:** Abdurrahman Güzel

---
