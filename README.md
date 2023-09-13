# stored-procedure-in-mysql-using-python
Helped online stores create a stored procedure so that they can call them according to their requirements in their Python-based application. 
## Scenario: 

Little Lemon needs to perform some tasks on a daily basis, and they involve extracting data from one or more tables. The tasks include finding the guest with maximum spending, retrieving the bookings for no arrival, and displaying the order status to the guests. To keep consistency during the data retrieval process, Little Lemon is interested in implementing the required tasks using stored procedures. You can help Little Lemon create stored procedures so that they can call them according to their requirements in their Python-based application. 

## Task 1:

Little Lemon is running a marketing campaign this month. They need to issue a discount coupon to the top spender on a daily basis. Create a stored procedure `TopSpender` that can retrieve the booking ID, guest’s full name, and the bill amount of the top spender at closing. Call the procedure and print the results.   

**TIP:** Target `BookingID`, `GusetFistName`, `GuestLastName`, and `BillAmount` columns from the `Bookings` and the `Orders` tables. Use the concatenation function to get the guest’s full name. Join the two tables and retrieve the top spender. Create a stored procedure, call it by its name using Python, and print the results. 

## Task 2:

Help Little Lemon retrieve all those bookings where the guests did not appear today. How will you implement this task using a stored procedure? Use `NoArrival` as a name for your stored procedure.

TIP: Target the `Orders` and the `Bookings` tables, join them on `BookingID`, and retrieve the records with a `NULL` value in the bill amount. Create a stored procedure, call it by its name using Python, and print the results.


## Task 3:

It is very important for Little Lemon to keep track of the status of each guest’s order and display it on the screen to keep their guests informed.  

This is how they categorize the orders:

* If not assigned to any employee, the status is `In Queue` 
* If assigned to the employees with IDs 4 and 5, the status is `Preparing Order` 
* If assigned to the employees with IDs 1, 2, and 3, the status is `Order Served` 

Create a stored procedure named `OrderStatus` for the above task and call to check if everything is working.  

**TIP:** Target `EmployeeID` column in the `Bookings` table and use the `CASE` function in your stored procedure query. Create a stored procedure, call it by its name using python and print the results.  

