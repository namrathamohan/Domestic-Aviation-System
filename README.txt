Introduction
----------------
We have designed a Database for Domestic Aviaton System. It is an Airline Ticketing System which is designed for eight airlines with almost 40 routes.

The Software package comprises an sql file which contains the create table statements and commands for inserting the data to tables. There are 
8 csv files one each for every table which contains the values to be inserted into tables. There are 12 files(select_sql) with one select query in each file.
The package also contains a README.txt containing instructions for executing the queries.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Step 1: Login to the classes server classes.csc.lsu.edu with valid userid and password

Step 2: Create a folder with name projectgroup10 in the classes server
            mkdir projectgroup10
Note: The folder name projectgroup10 is used in our commands for data Insertion. To avoid errors, please use the same name to create the folder.

Step 3: Go to the projectgroup10 directory 
            cd projectgroup10

Step 4: Upload all the files given in the package

Step 5: To list the files in projectgroup10 directory
             ls
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Files included in the projectgroup10 directory: 
Airline.csv                          Airport.csv                                Card.csv                       Customer.csv                          Flight.csv                                   Itinerary.csv
Payment.csv                      Schedule.csv                             createtable_sql            select_sql_1                           select_sql_2                              select_sql_3
select_sql_4                      select_sql_5                              select_sql_6                 select_sql_7                           select_sql_8                              select_sql_9
select_sql_10                    select_sql_11                            select_sql_12               select_sql_13                         README.txt
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
SQL Execution Steps:
-----------------------------
Note: Please make sure that you are in projectgroup10 directory before running the SQLs

Test Case 1: To create the tables and insert data in all the tables.

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <createtable_sql

Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

- createtable_sql contains create table statements and the command to insert values to each table.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 2: This is a select query to "Select the name and city of Customers departing from California between 9:00 and 23:00"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_1
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentials and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_1 file and paste in the server
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 3: This is a select query to "Select the Airport Name and City in the state of Louisiana for Flights departing and arriving between 2017-01-01 to 2019-12-12 and group by Airport Name"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_2
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_2 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 4: This is a select query to "Select the Airport ID, Name, and City of Airports that have not had Customers from San Jose or Seattle City depart or arrive from that Airport"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_3
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_3 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 5: This is a select query to "Select the Airport name and daily revenue of Airports with a daily revenue of more than $200 arranging the results in descending order of daily revenue"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_4
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_4 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 6: This is a select query to "Select customer names, city and seats of customers who are arriving at stations that are along the Latitude>30 and Latitude<42 and Longitude>-101 and Longitude<126
"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_5
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_5 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 7: This is a select query to "Select the Customer Name who have a card that does not expire in 2018 and have not ridden a flight owned by Spirit Airline
"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_6
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_6 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 8: This is a select query to "Select the Airport ID, name, and city of Airports in Texas with flights arriving between 14:00 and 20:00
"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_7
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_7 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 9: This is a select query to "Select Flight ID, Airline Name, Departure and Arrival Time and Date that starts from the Airport in city of Las Vegas and group by departure time
"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_8
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_8 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 10: This is a select query to "Select Airport ID and Name from Airport that don't have any Itinerary
"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_9
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_9 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 11: This is a select query to "Select the Airport Name, Airport id and Customer Name pairs where a Customer has arrived at an airport in the city of the Customer
"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_10
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_10 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 12: This is a select query to "Select Airline Name and number of Flights for each Flight"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_11
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_11 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Case 13: This is a select query to "Select the Airline Name and Number of transactions made by customers between 2017-05-22 and 2017-12-30
"

Step to execute the sql script using MYSQL server:
mysql --local-infile  -uxxxxxx -pzzzzzz yyyyyy <select_sql_12
     
Note: xxxxxx refers to sql server username
          zzzzzz refers to the sql server password
          yyyyyy refers to the database name(For our project, we used the default database assigned to individuals in the classes server)
Please replace the above three values with your sql server credentails and the database name.

(OR)

Steps to execute in MYSQL server
Step 1: Ensure you are in the projectgroup10 directory. Login to MYSQL server using the below command
            mysql --local-infile  -uxxxxxx -p
Note: xxxxxx refers to sql server username

Step 2: provide the sql server password

Step 3: select the database to be used using the below command
            use <database name>

Step 4: Copy the sql written in select_sql_12 file and paste in the server
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------