# TellCo Data Analysis

## **Approach**

### **Task-1: Overview of the User's Behavior on Applications**

- **Aggregate per-user information** in the column:  
  - Number of xDR (data sessions Detail Record)
  - Session duration
  - Total download and upload data
  - Total data volume (in Bytes) during the session for each application
- Conduct an **Exploratory Data Analysis (EDA)** on the data and communicate useful insights.

### **Task-2: Tracking the User's Engagement Using the Following Engagement Metrics**

- Session's frequency, duration, and total traffic.
- Aggregate and report the metric per customer ID (MSISDN).
- Normalize each engagement metric and run a **K-means (k=3)** to classify customers into three groups of engagement.
- Compute the minimum, maximum, average & total non-normalized metrics for each cluster.
- **Plot the top 3 most used applications** using appropriate charts.

### **Task-3: User Experience Analysis**

- **Aggregate per customer average**:
  - TCP retransmission
  - Round Trip Time (RTT)
  - Throughput
  - Handset type
- Compute & list:
  - 10 of the top, bottom, and most frequent TCP values
  - RTT values
  - Throughput values in the dataset
- Compute & report:
  - Distribution of the average throughput and average TCP retransmission per handset type.
  - Provide interpretation.
- Perform a **k-means clustering** (where k=3) to segment users into groups of experiences and provide a brief description of each cluster.

### **Task-4: Customer Satisfaction Analysis**

- Write a Python program to assign an **engagement score** to each user:
  - Consider the engagement score as the **Euclidean distance** between the user data point & the least engaged cluster.
- Assign an **experience score** to each user:
  - Consider the experience score as the **Euclidean distance** between the user data point & the worst experience cluster.
- **Satisfaction score**:  
  - Consider the average of both engagement & experience scores and report the top 10 satisfied customers.
- Build a regression model of your choice to **predict the satisfaction score** of a customer.
- Run a **K-means (k=2)** on the engagement & experience scores.
