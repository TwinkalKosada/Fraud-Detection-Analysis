## Bank Transaction & Fraud Detection Dashboard

# A Power BI Analytics Project


This project presents a comprehensive Power BI dashboard designed to analyze banking transactions, monitor fraud patterns, and uncover high-risk behaviors. The solution includes multi-page reporting that enables financial institutions or analysts to identify unusual patterns, network-related anomalies, and fraud trends across regions.

# The dashboard consists of three interconnected report pages:

Overview

Fraud Detection

Transaction Details

# Overview Dashboard

This page offers a high-level summary of all transactions across time, geography, and transaction type.

Key Features

Total transactions and total transaction value

Trend analysis of transactions over time

Transaction breakdown by type (Transfer, Deposit, Withdrawal)

Success vs Failed transaction comparison

Fraud vs Non-Fraud distribution

World map showing transaction density by region

(https://github.com/TwinkalKosada/Fraud-Detection-Analysis/blob/main/Fraud%20Detection%201.png)


# Fraud Detection Dashboard

This page focuses entirely on fraudulent transaction patterns and network-level risk indicators.

Key Features

Total fraudulent transactions

Fraudulent transaction amount

Fraud breakdown by status

Fraud distribution based on Bandwidth Group

Fraud distribution across Network Slice ID

Global map showing suspicious activities

Screenshot:


# Transaction Details

This page contains a filterable table that displays all raw transaction records. It supports drill-down analysis, filtering by transaction type, fraud flag, device, and network slice ID.

Fields Include:

Transaction ID

Sender and Receiver Account IDs

Transaction Type

Fraud Flag

Amount

Status

Bandwidth Group

Network Slice ID

Timestamp

Screenshot:


# Key Insights
1. Transaction Volume & Behavior

The dataset contains 1,000 transactions totaling $771.17K.

Transaction activity varies significantly, with noticeable spikes around 10:30 AM and 10:50 AM, indicating possible batch processing or system-triggered transactions.

2. Transaction Status Analysis

Failed transactions (513) slightly exceed successful ones (487).

A high failure rate suggests potential issues such as:

Network bottlenecks

Device limitations

High system load during peak time

Invalid requests or operational constraints

3. Fraud Analysis

Fraudulent transactions account for 51.9%, while non-fraudulent account for 48.1%.

The fraud percentage is unusually high, indicating either:

A simulation-heavy dataset

Or an environment with frequent fraudulent attempts

Fraud is evenly distributed across transaction types, highlighting that all categories carry risk exposure.

4. Transaction Type Distribution

Transfers represent 37.4% of the dataset, making them the most common and potentially highest-risk transaction type.

Deposits (31.6%) and withdrawals (31%) follow closely, demonstrating a balanced mix of banking activity.

5. Regional Insights

Transactions span North America, Europe, and parts of Asia.

Fraud patterns appear globally distributed rather than localized, which suggests systemic risks rather than region-specific fraud clusters.

6. Bandwidth Group Insights

The 150–250 Mbps bandwidth group shows the highest fraud activity with 487 occurrences.

Fraud distribution across Network Slices is relatively equal (Slice1, Slice2, Slice3), indicating that network segmentation alone does not significantly influence fraud patterns.

7. Detailed Table Insights

Failed transactions appear consistently across all timestamps.

Fraudulent transactions occur throughout the entire time window, showing no specific time-bound pattern.

Fraud spans all account ranges, devices, and transaction categories.

Business Recommendations

Strengthen fraud detection algorithms especially for transfer transactions and high-bandwidth users.

Investigate system performance issues causing frequent failed transactions.

Implement additional network-level controls for high-bandwidth segments.

Enhance global monitoring since fraud attempts are not region-specific.

Introduce anomaly-based alerts for unusual transaction spikes.

# Tools & Techniques Used

Power BI Desktop

DAX Measures

Data Modeling (relationships, cardinality)

Time-series Visualization

Geospatial Mapping

KPI and donut visualization

Transaction-level table modeling
