# Engineering Intent — ezFinance

## 1. Project name

EzFinance

## 2. Problem statement

The user has to download different bank trasactions distributed across different financial institutions normalize and categorize the data, and manually create an analysis to understand their expeses and get an overview of their finances

### 2.1 What happens because of the problem?

The user does not know whether their expenses stay within  budget, which could negatively affect their quality of life and financial well-being 

### 2.2 What outcome should improve?

The user should be able to reduce the impact of unforeseen expenses and avoid going over budget

## 3. Primary user

A person who already downloads transaction statements from multiple Colombian banks and wants to consolidate and analyze them without maintaining a spreadsheet manually.

## 4. User goals

- Understand where money is being spent without manually maintaining a spreadsheet.
- See monthly income, expenses and balance in one place.
- Identify whether spending is staying within expected limits.
- Compare spending patterns across periods and categories.

## 5. Core capabilities — V1

The project will be able to:

- Import statement
- Parse bank-specific format
- Normalize transaction
- Persist normalized transactions
- Prevent duplicate imports
- Classify transactions
- View transactions 
- Filter transactions
- Aggregate financial data
- Allow the user to manually assign a category to a transaction.- Display financial overbview
- Generate a dynamic dashboard

### 5.1 Supported sources in V1:
- Receive bank transactions from Falabella and Bancolombia
- Receive XLSX


## 6. Out of scope

- More complex dashboards
- Automatic categorization of expenses
- A Chatbot with full context of the user's budget
- The app will be available anyone who want visibility over personal finances
- Besides current banks, it will receive bank transactions from Nequi and Davivienda
- Will support PDF files 


## 7. Constraints

- The MVP must be completed in 3 weeks
- First iteration will be a web application
- The MVP will not have user authentication yet, I will be the primary user testing all functions


## 8. Risks

- The user might upload sensitive personal data through bank documents
The project still requires the user to manually download their bank transactions and upload them to the application. In simple terms, the system depends on an initial action from the user and is not fully automated yet.
- The initial transaction categories will be provided by the user, which could negatively affect the user experience if the user does not know how to categorize their transactions
- Uploaded files may contain incorrectly formatted data, invalid fields or irrelevant information which could cause errors during processing.

## 9. Success criteria

- A supported bank statement can be imported without manually copying transaction rows.
- Imported transactions appear correctly normalized in the application.
- The user can determine total income, total expenses and spending by category for a selected period without using Excel or pivot tables.
- Re-importing the same statement does not create duplicate transactions.
- Processing a typical supported statement should complete within [X] seconds.