
# 📊 PhonePe Transaction Insights

Gain insights into digital payment trends with this project, which uses PhonePe transaction data for analysis and visualization. This project is designed for data enthusiasts looking to explore finance/payment systems data and develop skills in data analytics and visualization.

---

## **Skills You'll Gain**
- **Data Extraction**: Efficiently gather and process data.
- **SQL Proficiency**: Query data from relational databases.
- **Data Visualization**: Create interactive visualizations using Plotly.
- **Streamlit Development**: Build intuitive web applications.
- **Analytical Thinking**: Derive insights from complex datasets.

---

## **Domain**
**Finance / Payment Systems**
Analyze digital transaction data to understand trends and optimize payment strategies.

---

## **Features**
### 1. **Transactions**:
- Visualize state-wise data of total transactions and transaction amounts.
- Display the count of transactions for each state.
- Bar charts showing the most popular payment types.
- District-wise transaction data for selected states.

### 2. **Users**:
- Display the total number of users and their app opening frequency state-wise.
- District-wise user data based on selected states.

### 3. **Insurances**:
- Visualize state-wise transaction amounts related to insurance.
- Display transaction counts and amounts for insurance data.
- Top payment types for insurance transactions.

### 4. **About Section**:
- Provides details about PhonePe Pulse and the services offered by PhonePe.
- Includes information about PhonePe's offerings such as UPI, digital wallet, bill payments, insurance, mutual funds, and more.
- Multimedia content including images and videos of PhonePe campaigns.

---

## **Menu-1: Home**
### Welcome to PhonePe Transaction Insights
The home page introduces the application and highlights the features of PhonePe. It serves as a user-friendly interface with the following elements:

- **Title and Tagline**:
  - "PHONEPE TRANSACTION INSIGHTS"
  - "A User-Friendly Tool Using Streamlit and Plotly"

- **Overview**:
  - PhonePe is India's leading digital payments app with various features, including:
    - Credit & Debit card linking
    - Bank Balance check
    - Money Storage
    - PIN Authorization
    - Easy Transactions
    - Multiple Payment Modes
    - QR Code Payments
    - Direct Bank Transfers
    - Earn Rewards

- **Media and Interactivity**:
  - Image showcasing the PhonePe logo.
  - Video introduction to PhonePe Pulse.
  - Download button to access the app.

---

## **Menu-2: Top Charts**
### Explore Top Charts
The Top Charts menu allows users to explore detailed insights into transactions, users, and insurances using interactive filters. Key elements include:

- **Filters**:
  - **Type**: Choose between "Transactions," "Users," or "Insurances."
  - **Year**: Select a year (2018 to 2024).
  - **Quarter**: Choose a specific quarter (1 to 4).

#### Transactions
- Displays the top 10 states, districts, and pincodes based on the total number of transactions and the total amount spent on PhonePe.
- **Visualization**:
  - Pie charts created using Plotly visualize the top states, districts, and pincodes by transaction amounts.
  - Data includes:
    - **Names** (States/Districts/Pincodes)
    - **Total Transaction Count**
    - **Total Amount Spent**
- **Dynamic Updates**:
  - If no data is available for a specific quarter in 2024 (Q3 or Q4), a message is displayed: "Sorry No Data to Display for 2024 Qtr 3,4."
- Example SQL Query:
  ```sql
  SELECT States, SUM(Transaction_count) AS Total_Transactions_Count, SUM(Transaction_amount) AS Total
  FROM aggregated_transaction
  WHERE Years = {Year} AND Quarter = {Quarter}
  GROUP BY States
  ORDER BY Total DESC
  LIMIT 10;
  ```

---

## **Technologies Used**
- **GitHub Cloning**
- **Python**
- **Pandas**
- **MySQL**
- **mysql-connector-python**
- **Streamlit**
- **Plotly**

---

## **Demo Video**
(https://www.linkedin.com/posts/vasuki-arul-18034a341_datascience-fintech-visualization-activity-7285522720463724544-my7B?utm_source=share&utm_medium=member_desktop)

---

## **Links**
- https://www.linkedin.com/in/vasuki27/
- [GitHub Repository](Your GitHub Link)

---

## **Setup Instructions**

### Prerequisites
- Python 3.7+
- MySQL database with transaction data.

### Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/phonepe-transaction-insights.git
   cd phonepe-transaction-insights
   ```

2. **Install Dependencies**
   Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure Database**
   - Ensure your MySQL server is running.
   - Update the database connection details in the script:
     ```python
     conn = mysql.connector.connect(
         host="localhost",
         user="root",
         password="xxxxxxx",
         database="phonepe_data_new"
     )
     ```

4. **Run the Application**
   Launch the Streamlit app:
   ```bash
   streamlit run app.py
   ```

---

## **Screenshots**
Add screenshots or GIFs here to showcase your dashboard and key features.

---

## **Contributing**
Contributions are welcome! To contribute:
1. Fork this repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

---

## **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---


## **About**
### **PhonePe Pulse:**
PhonePe Pulse is India's first interactive website with data, insights, and trends on digital payments in the country. Launched on Sept. 3, 2021, it showcases more than 2000+ Crore transactions by consumers on an interactive map of India. The website provides insights into the digital payment habits of Indians, with a market share of over 45% by PhonePe. 

The insights are drawn from PhonePe's transaction data combined with merchant and customer interviews. You can download reports and explore PhonePe Pulse on the website and GitHub.

### **Key Features of PhonePe:**
- **Unified Payments Interface (UPI):** Real-time peer-to-peer money transfers and payments.
- **Digital Wallet:** Store money and use it for various transactions.
- **Bill Payments:** Pay utility bills like electricity, water, and gas.
- **Mobile Recharge:** Recharge prepaid mobile phones and pay postpaid bills.
- **Online Shopping:** Shop online and avail discounts and cashback offers.
- **Insurance & Mutual Funds:** Invest and manage financial portfolios.
- **Gold Purchase:** Buy and sell digital gold securely.
- **Travel Services:** Book flights, hotels, and bus tickets for your travels.

---

## **Author Information**
### Name: VASUKI ARUL
### Batch: DS-C-WD-E-B29
### Domain: DATA SCIENCE


---

