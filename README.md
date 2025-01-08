🏦 Bank Transactions Data Cleaning and Visualization
This project focuses on data cleaning and visualization of bank transaction data to identify patterns, trends, and outliers. By transforming raw data into a structured format, the project aims to uncover meaningful insights and prepare the data for further analysis or machine learning applications.

📁 Dataset Overview
The dataset contains transaction details such as:

Transaction Amount
Customer Age
Transaction Type (Credit/Debit)
Account Balance
Transaction Date and Time
Location
Channel (ATM/Online)
Device ID, IP Address, and Merchant ID
Dataset Sample:
Transaction ID	Account ID	Transaction Amount	Transaction Type	Customer Age	Location	Channel
TX000001	AC00128	14.09	Debit	70	San Diego	ATM
TX000002	AC00455	376.24	Debit	68	Houston	ATM
TX000003	AC00019	126.29	Debit	19	Mesa	Online
🧹 Data Cleaning Steps
The following steps were applied to clean and preprocess the dataset:

Handling Missing Values: Imputed missing values with relevant statistics (mean, median, or mode) where appropriate.
Removing Duplicates: Ensured each transaction is unique by dropping duplicates.
Outlier Detection: Identified and handled outliers in columns like transactionamount and accountbalance using statistical techniques.
Date Parsing: Converted transactiondate into datetime format and extracted additional features like:
Transaction Hour
Day of the Week
Month of the Year
Categorical Encoding: Transformed non-numerical columns (e.g., transactiontype, channel) into numeric format for visualization and further analysis.
📊 Data Visualization
Key insights were derived using visualizations, including:

Transaction Type Distribution:

Customer Age vs. Transaction Amount:

Location-Based Transaction Patterns:

Account Balance Trends by Channel: Visualized account balance usage in Online vs. ATM transactions.

📈 Key Insights
Transaction Type: Most transactions were Debit compared to Credit.
Customer Age Trends:
Younger customers (ages 18–25) prefer Online transactions.
Older customers (ages 50+) predominantly use ATM transactions.
Outliers: Detected high-value transactions in specific regions that may require further investigation for fraud.
Peak Hours: Transactions spike during business hours (9 AM–5 PM), especially in Urban Locations.
🚀 Tools and Technologies
Python Libraries: Pandas, NumPy, Matplotlib, Seaborn, Plotly
Data Visualization: Matplotlib, Seaborn, and Plotly for interactive plots
Jupyter Notebook/Google Colab: For analysis and visualization
GitHub: Version control and collaboration
💻 How to Use
Clone the repository:
bash
Copy code
git clone https://github.com/harivign/bank-transactions-ds-data-cleaning-and-data-visualization.git
Install dependencies:
bash
Copy code
pip install -r requirements.txt
Run the notebook in Google Colab or Jupyter Notebook.
🔮 Future Enhancements
Interactive Dashboards: Use Dash or Streamlit for real-time data visualization.
Anomaly Detection: Implement algorithms to detect fraudulent transactions.
Predictive Modeling: Use cleaned data to classify transactions as fraudulent or legit.
📜 License
This project is licensed under the MIT License.

