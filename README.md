# Pet-Docker
Application source file ---- main.py

Following functionalities have been developed and tested: a. Login b. User registration c. Simple dashboard with wallet balance d. Adding expenses e. Updating wallet balance f. Home page

APIs developed: a.Wallet balance retrieval API: https://ss979hyehb.execute-api.ap-south-1.amazonaws.com/WalletBalance b.Wallet balance updation API: https://l1gdzvb6k6.execute-api.ap-south-1.amazonaws.com/addwallamount c. API to set the Expenses: https://ket0h58q15.execute-api.ap-south-1.amazonaws.com/ExpenseAPI? d. API to fetch the Expenses: https://5996kr662d.execute-api.ap-south-1.amazonaws.com/ExpenseQA? e. API to fetch user details: https://nirmgp3j2c.execute-api.ap-south-1.amazonaws.com/fetchuser?user= f. API to push user details: https://nqwsosw3ag.execute-api.ap-south-1.amazonaws.com/QA?

Associated Lambda functions: a. putinfo: pushes user info into a database b. fetchUser: pulls user details from the database c. walletbalance : pulls wallet balance from the database d. push_expense_data : pushes expense data into the database e. fetchExpenses: fetches expense details of a user from the database f. addwalletamount : pushes additional amount to wallet balance g. limitsns(Created but not working): tried to send an SNS message upon exceeding a monthly limit but not working

Associated AWS DynamoDBs: a. users - user details b. expense_summary - expenses related to user c. wallet_balance - contains user wallet balance d. monthly_limits - contains user set monthly limits for expenses

Functionalities to be completed: a. Dynamic data integration for expense graphs(static data reflects in graph) ----FIXED(3/6/2021) b. SNS integration with expense limits c. Session handling and form field validations
