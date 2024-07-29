
# CLTV and RFM Analysis Using BG-NBD and Gamma-Gamma Models

## Project Overview

This project involves analyzing customer behavior data from the FLO dataset to predict Customer Lifetime Value (CLTV) and conduct Recency, Frequency, Monetary (RFM) analysis. The dataset includes information on customer transactions from both online and offline channels during 2020 and 2021. The BG-NBD and Gamma-Gamma models are used for CLTV prediction.

## Dataset

The dataset consists of the following columns:

- **master_id**: Unique customer ID
- **order_channel**: The platform used for shopping (Android, iOS, Desktop, Mobile, Offline)
- **last_order_channel**: The channel used for the last purchase
- **first_order_date**: The date of the customer's first purchase
- **last_order_date**: The date of the customer's most recent purchase
- **last_order_date_online**: The date of the customer's most recent online purchase
- **last_order_date_offline**: The date of the customer's most recent offline purchase
- **order_num_total_ever_online**: Total number of purchases made by the customer online
- **order_num_total_ever_offline**: Total number of purchases made by the customer offline
- **customer_value_total_ever_online**: Total amount spent by the customer on online purchases
- **customer_value_total_ever_offline**: Total amount spent by the customer on offline purchases
- **interested_in_categories_12**: List of categories the customer has shopped in the last 12 months

## Methodology

### Data Preprocessing

1. Data cleaning and preparation.
2. Aggregating customer transaction data to calculate:
   - Total number of purchases (online and offline).
   - Total monetary value of purchases (online and offline).
3. Calculating Recency, Frequency, and Monetary (RFM) values for each customer.

### CLTV Prediction

Using the BG-NBD and Gamma-Gamma models to predict CLTV:

1. **BG-NBD Model**: Estimates the expected number of transactions a customer will make in the future.
2. **Gamma-Gamma Model**: Estimates the average monetary value of transactions for each customer.

### Results

- RFM analysis to segment customers based on their purchasing behavior.
- CLTV predictions to identify high-value customers and inform business strategies.

## Installation

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/99Abdurrahman/CRM-Analytics.git
cd CRM-Analytics/



