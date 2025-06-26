
🚀 <ins>**Project Brief: Customer Churn Prediction System**</ins>
- Address the rising issue of **customer churn** in a thriving subscription-based business.
- Emphasize the value of **retaining existing customers** over acquiring new ones.
- Pose the key question: **Can we predict which customers are likely to leave?**
- Goal: Build a **Customer Churn Prediction and Analysis System**.
- **Project journey will include:**
- **Data extraction and storage with SQL**
- **Data cleaning and Preaparation with Python and its Libraries**
- **Data visualization and reporting with Power BI**
- **Machine learning modeling**

- **Outcome: Provide actionable insights to proactively reduce churn and improve retention.**


🧭 <ins>**The Data Treasure Hunt [Extraction and Storage]**</ins>
- Begin the project with **data discovery**—exploring customer-related databases.
- Use SQL to design a **relational database** from raw data tables.
- Extract key customer information:
- **Personal details**
- **Subscription history**
- **Transaction data**
- **Churn flags**
- Query the data to filter and select **behaviorally significant records.**

[View Data Set](https://drive.google.com/drive/folders/15jqGLwlx-FOZwho49jqSYABqqvC616tl?usp=sharin)

<ins>**The Data Treasure Hunt**</ins>

The goal is to design and implement a **relational database** that can store customer data, subscription details, transaction history, and churn status.

<ins>**Tables**</ins>

**Customers**:-   CustomerID (Primary Key, INT),FirstName (VARCHAR),LastName (VARCHAR),Email (VARCHAR),PhoneNumber (VARCHAR),JoinDate (DATE),Status (VARCHAR),Region (VARCHAR)

**Subscriptions**:- SubscriptionID (Primary Key, INT),CustomerID (Foreign Key, INT),StartDate (DATE),EndDate (DATE),PlanType (VARCHAR)

**Transactions**:- TransactionID (Primary Key, INT),CustomerID (Foreign Key, INT),TransactionDate (DATE),Amount (DECIMAL),TransactionType (VARCHAR).

**Churn**:- ChurnID (Primary Key, INT),CustomerID (Foreign Key, INT),ChurnDate (DATE),Reason (VARCHAR).

<ins>**Relationships**</ins>:

The Customers table is related to Subscriptions and Transactions through the **CustomerID**.

The Churn table is related to Customers via **CustomerID**.
