# MySQL-Project-LMS
# Library Management System (LMS)

## Introduction:
The Library Management System (LMS) is an essential tool for efficiently managing the operations of a library. It assists in organizing, tracking, and managing various aspects such as books, customers, employees, and branches. The system provides functionalities for book issuance, returns, employee management, and customer registration, among others.

In this project, a database named "library" with several tables is designed to accommodate the necessary information required for a library management system. These tables include Branch, Employee, Books, Customer, IssueStatus, and ReturnStatus.

## An overview of the tables and their attributes:

1.Branch:
  Branch_no (Primary Key)
  Manager_Id
  Branch_address
  Contact_no

2.Employee:
  Emp_Id (Primary Key)
  Emp_name
  Emp_Position
  Salary
  Branch_no (Foreign Key referencing Branch_no in Branch table)

3.Books:
  ISBN (Primary Key)
  Book_title
  Category
  Rental_Price
  Stock_Status (Indicating book availability)
  Author
  Publisher

4.Customer:
  Customer_Id (Primary Key)
  Customer_name
  Customer_address
  Reg_date (Registration date)

5.IssueStatus:
  Issue_Id (Primary Key)
  Issued_cust (Foreign Key referencing Customer_Id in Customer  table)
  Issued_book_name
  Issue_date
  Isbn_book (Foreign Key referencing ISBN in Books table)

6.ReturnStatus:
  Return_Id (Primary Key)
  Return_cust (Foreign Key referencing Customer_Id in Customer  table)
  Return_book_name
  Return_date
  Isbn_book2 (Foreign Key referencing ISBN in Books table)

This system enables to perform various queries and operations to efficiently manage library resources and services. This project includes the queries for the following:

1. Retrieve the book title, category, and rental price of all available books.
2. List the employee names and their respective salaries in descending order of salary.
3. Retrieve the book titles and the corresponding customers who have issued those books.
4. Display the total count of books in each category.
5. Retrieve the employee names and their positions for the employees whose salaries are above Rs.50,000.
6. List the customer names who registered before 2022-01-01 and have not issued any books yet.
7. Display the branch numbers and the total count of employees in each branch.
8. Display the names of customers who have issued books in the month of June 2023.
9. Retrieve book_title from book table containing history.
10.Retrieve the branch numbers along with the count of employees for branches having more than 5 employees

 The queries outlined in the project requirements allow us to retrieve valuable insights and perform necessary actions within the library management system.

