# 🏦 **Credit Card and Customer Data Management Project**

## 📜 **Overview**
This project sets up a **SQL database** to manage credit card data and customer details. By importing CSV files into structured tables, you can handle credit card transactions, customer information, and more. It also includes mechanisms to handle common data import errors like date formatting issues.

## ⚙️ **Key Features**
- **Create Database**: We begin by creating a dedicated database called `ccdb`.
- **Data Tables**: Two tables manage the credit card and customer data:
  - **`cc_detail`**: Contains information like card category, transaction amounts, and utilization.
  - **`cust_detail`**: Stores customer demographic information, income, and satisfaction scores.
- **Data Import from CSV**: The project imports data using the `COPY` command, making it simple to populate the tables with data from CSV files.
- **Error Handling**: Includes error management for date format inconsistencies by adjusting the PostgreSQL `datestyle`.

## 📂 **Data Structure**

### `cc_detail` Table:
- **Card Details**: Includes client number, card type, annual fees, credit limits, and transaction amounts.

### `cust_detail` Table:
- **Customer Information**: Stores customer age, gender, education, marital status, income, and satisfaction scores.

## 🚀 **How to Use**
1. **Set Up Database**: Run SQL scripts to create the `ccdb` database and both data tables.
2. **Import Data**: Use the `COPY` commands to load data from CSV files into the tables.
3. **Handle Errors**: For date format issues, set the `datestyle` using `SET datestyle TO 'ISO, DMY';` to ensure consistent data imports.

## 📈 **Expandability**
You can continue to add more data, such as additional weeks' data, by following the same `COPY` process. This allows for easy expansion as your data grows.

## 💡 **Conclusion**
This project provides a strong foundation for managing large datasets with SQL. It ensures efficient data imports, robust error handling, and the flexibility to add more data as needed, making it perfect for anyone working with credit card and customer information.
