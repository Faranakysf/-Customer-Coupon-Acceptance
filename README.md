# -Customer-Coupon-Acceptance
The goal of this project is to distinguish between customers who accepted a driving coupon versus those that did not. 
# Customer-Coupon-Acceptance
This analysis seeks to answer the question, “Will a customer accept the coupon?"

# Coupon Acceptance Analysis
The goal of this project is to distinguish between customers who accepted a driving coupon versus those that did not. The analysis uses Python, Pandas, Matplotlib, and Seaborn to explore the coupon acceptance and the data comes from the UCI Machine Learning repository. The data was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc.,

## Dataset
The dataset (`data/coupons.csv`) is sourced from the UCI Machine Learning Repository.

## Tools Used
- Python, Pandas, Matplotlib, Seaborn
  
## Repository Structure

- **`coupon.ipynb`**: The main Jupyter Notebook containing the full analysis, including data cleaning, visualizations, bar coupon analysis, and an independent investigation of Coffee House coupons.
- **`data/couponsdata.csv`**: The dataset used for analysis, containing 12,684 rows and 26 columns of driver attributes, contextual attributes, and coupon attributes.
- **`images/`**: Folder containing visualization images generated from the notebook:
  - `bar_age25.png`: Bar plot comparing bar coupon acceptance for frequent visitors over 25 vs. others.
  - `bar_combined_group.png`: Pie chart comparing bar coupon acceptance for a combined group vs. others.
  - `bar_non_kid_non_farming.png`: Bar plot comparing bar coupon acceptance for frequent visitors with non-kid passengers and non-farming occupations.
  - `temperature_distribution.png`: Histogram of temperature values.
  - `bar_visit_frequency.png`: Pie chart comparing bar coupon acceptance rates by visit frequency.

## Data Description

The dataset includes:
- **User Attributes**: Gender, age, marital status, income, occupation, visit frequency to bars, coffee houses, etc.
- **Contextual Attributes**: Destination, weather, temperature, time, passenger.
- **Coupon Attributes**: Coupon type (e.g., Restaurant(<20), Coffee House, Bar), expiration time.
- **Target Variable**: `Y` (1 = accepted, 0 = not accepted).

Key data cleaning steps:
- Dropped the `car` column due to 99.15% missing values (12,576 out of 12,684 rows).
- Dropped missing rows in `CoffeeHouse`, `CarryAway`, `Bar`.

## Key Findings

Based on the analysis of bar coupon acceptance in the dataset, I hypothesize that drivers who accept bar coupons are more likely to be frequent bar visitors (visiting more than once per month) and are typically over 25 years old. Additionally, they are often traveling with friends or partners rather than children, creating a social context that aligns with bar visits. Their occupations also play a role—those not in farming occupations are more likely to accept coupons, possibly due to lifestyle differences that make bar visits more feasible or appealing.

In addition, these drivers tend to exhibit cost-conscious behavior, often having incomes below $50,000 and frequently visiting inexpensive restaurants (more than 4 times per month). This suggests that they are motivated by discounts and value-driven offers, making bar coupons particularly attractive. Overall, the profile of a bar coupon acceptor appears to be a socially active, budget-conscious individual who is already inclined to visit bars and sees the coupon as an added incentive for their lifestyle.

## Visualizations
Visualization images are included in the repository in images folder.

## How to Run the Analysis

1. **Clone the Repository**:
   ```bash
   git clone https://github.com//Faranakysf/Customer-Coupon-Acceptance.git
