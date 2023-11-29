Day 1: Account Creation & Installation
I kicked off the challenge by;

Creating an account with Motherduck: https://app.motherduck.com/?auth_flow=signup

Installed DuckDB on my Local machine: https://duckdb.org/docs/guides/sql_editors/dbeaver.html

Installed Power BI on my computer and configured it: https://powerbi.microsoft.com/en-us/downloads/

Day 2: Data Loading, Database creation and Access
For day 2 of the challenge, the following were done;

Database Creation: I created a DuckDB database named "challenge"

Database Access: I integrated and accessed the DuckDB database on Motherduck, which serves as our collaborative platform (md:my_db?motherduck_token=)

Data Loading: I loaded the provided CSV files into the DuckDB database.

SQL Queries
---Table 1
CREATE TABLE fifa21_player AS
SELECT * FROM read_csv_auto('C:\Users\USER\Desktop\fifa21_raw_data.csv', ALL_VARCHAR=TRUE);

---Table 2
CREATE TABLE fifa21_player2 AS 
SELECT * FROM read_csv_auto('C:\Users\USER\Desktop\fifa21 raw data v2.csv', SAMPLE_SIZE=-1);# DuckDB30DaysChallenge
