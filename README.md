# Crypto Trader Performance Analysis

An analysis of how market sentiment (Fear vs. Greed) impacts the profitability and behavior of different crypto trader segments.

##  How to Setup and Run This Project

### step 1: Open Jupyter Notebook
Open your terminal or Command Prompt.

Navigate to the folder where you saved your assignment files.
Launch Jupyter by running:
jupyter notebook

### Step 2: Install Required Packages
Open your terminal (or Command Prompt / Anaconda Prompt) and run the following command to install the necessary libraries:
pip install pandas numpy matplotlib notebook

### Step 3:Run the Code
In the Jupyter browser interface, click on the file named Data_Analysis_Assignment.ipynb to open it.
In the top menu bar, click Cell -> Run All (or Kernel -> Restart & Run All).
The code will execute, and the data tables and performance charts will display instantly.

### Project Overview & Summary

#### Methodology
Data Prep: Cleaned daily trading metrics and logs, resolved duplicates, and merged them with market sentiment indices by date.
Segmentation: Split traders by their volume into Frequent Traders (high-activity pros) and Infrequent Traders (casual retail).

#### Core Insights
Panic Drives Profits: Traders make over double the daily profit on Fear days compared to Greed days because panics create opportunities to buy assets at a steep discount.
Pros Thrive on Volatility: Frequent Traders hit peak performance during market panics, generating an average of $332,577/day by absorbing rapid retail panic-selling.
Quiet Markets are Deadzones: On Neutral days, price movement stalls, and average daily profits drop below $8,000 for all groups due to a lack of volatility.

#### Strategy Recommendations
Strategy 1: Automatically prompt high-frequency models for Frequent Traders when the index flags Fear to maximize volatility capture.
Strategy 2: Enforce lower position limits or risk alerts for Infrequent Traders on Greed days to protect them from buying at bubble peaks (FOMO).
