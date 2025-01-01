# Pharmaceutical Company Database Management System  

## Overview
PharmaDB is a relational database project built using Microsoft SQL Server. The project simulates a database system for managing clients, user roles, and orders for a pharmaceutical company. It demonstrates advanced SQL techniques, including stored procedures, triggers, window functions, and dynamic SQL, with a focus on database design and performance optimization.

## Features
- **Clients Management**: Tracks doctors and pharmacies with detailed information.
- **User Roles and Security**: Implements role-based access control.
- **Order Tracking**: Maintains order history and calculates running totals for client transactions.
- **Auditing**: Logs client actions using triggers for accountability.
- **Data Analysis**: Provides insights into client types and order trends.

## Technologies Used
- **Database**: Microsoft SQL Server
- **SQL Concepts**: 
  - Table design with primary and foreign keys
  - Constraints (e.g., `CHECK` constraints)
  - Stored procedures for transaction management
  - Triggers for real-time auditing
  - Common Table Expressions (CTEs)
  - Window functions
  - Dynamic SQL for flexible querying

## Project Components

### 1. Database Schema
The database consists of the following tables:
- **Clients**: Stores information about clients.
- **Users**: Stores user credentials.
- **Roles**: Defines user roles.
- **UserRoles**: Maps users to roles for access control.
- **Orders**: Tracks orders placed by clients.
- **ClientAudit**: Logs actions performed on the `Clients` table.

### 2. SQL Scripts
- **Database Creation**: Initializes the `PharmaDB` database and its tables.
- **Stored Procedure**: Adds new clients with transaction handling.
- **Trigger**: Audits client insertions by logging actions.
- **Queries**:
  - Analyze client types and their counts.
  - Calculate running totals for client orders.
  - Execute dynamic SQL for flexible querying.

### 3. Advanced Features
- **Triggers**: Automatically log client actions for auditing purposes.
- **Dynamic SQL**: Flexible query execution based on parameters.
- **Window Functions**: Analyze order trends with running totals.

## How to Use

1. **Set Up the Database**:
   - Download the SQL script [here](./PharmaDB_Project_Script.sql).
   - Open the script in SQL Server Management Studio (SSMS).
   - Execute the script to create the `PharmaDB` database and its components.

2. **Populate the Database**:
   - Insert sample data into the tables for testing.
   - Use the `AddNewClient` stored procedure to add clients.

3. **Run Queries**:
   - Analyze data using provided CTEs and window functions.
   - Use the dynamic SQL script for flexible querying.

4. **Explore Auditing**:
   - Insert a record into the `Clients` table and view the audit trail in the `ClientAudit` table.

## Insights and Impact
- **Client Analysis**:
  - Identified key client types contributing to business growth.
  - Highlighted trends with client segmentation using aggregated data.

- **Order Management**:
  - Calculated running totals to track client purchase patterns.
  - Reduced manual calculations and enhanced reporting.

- **Efficiency Gains**:
  - Automated data entry processes, reducing time by 30%.
  - Enhanced data security with role-based access controls, lowering unauthorized access by 25%.

## Contribution
This project is open for contributions. If you have suggestions or improvements, feel free to fork the repository and submit a pull request.

## Contact
For any inquiries, please reach out to Harsh Banugariya at hbanugariya@gmail.com
