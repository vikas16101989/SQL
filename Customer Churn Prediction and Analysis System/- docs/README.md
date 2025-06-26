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
