# SQL Theory: Practical Exam on Database Management and Querying



 ## 1. Objective  
To demonstrate practical SQL skills including creating tables, inserting records, and performing queries such as sorting and filtering.



## 3. Expected Outcome  
- A structured customer table named CustomerTB  
- Multiple data entries inserted successfully  
- Queries executed for displaying, sorting, and filtering data  
- Strong understanding of core SQL operations


## Exploratory Data Analysis (EDA)


### 4. Key Questions  
1. Return the FirstName and Email of every customer who has ever purchased the product 
“Wireless Mouse”. (10 Marks) 
2. List all customers’ full names in ascending alphabetical order (LastName, then 
FirstName). (10 Marks) 
3. Show every order together with the customer’s full name, the product name, quantity, 
unit price, total price (quantity × unit price), and order date. (20 Marks) 
4. Show average sales per product category and sort in descending order (20Marks) 
5. Which city generated the highest revenue for AxiaStores? (10Marks)



## 5. Project Overview  
This project simulates a database task where a customer table is created and populated. The data includes names, emails, phone numbers, and cities. After creation, the table is queried to retrieve and manipulate the data using SQL commands.




## 6. Tools  
- SQL Server Management Studio (SSMS)  
[Website](https://office.com)




## Data Analysis

### Code/syntax
 #### Create Datasat

<pre>
  CREATE DATABASE AxiaStores;

  CREATE TABLE (CustomerTB)

  CREATE TABLE CustomerTB (
CustomerID INT PRIMARY KEY,
FirstName VARCHAR (50),
LastName VARCHAR (50),
Email VARCHAR (50),
Phone VARCHAR (50),
City VARCHAR (100));

INSERT RECORDS 

  INSERT INTO CustomerTB (CustomerID, FirstName, LastName, Email, Phone, City)
VALUES
('1', 'Musa', 'Ahmed', 'musa.ahmed@hotmail.com', '0803‐123‐0001', 'Lagos'),
('2', 'Ray', 'Samson', 'ray.samson@yahoo.com', '0803‐123‐0002', 'Ibadan'),
('3', 'Chinedu', 'Okafor', 'chinedu.ok@yahoo.com', '0803‐123‐0003', 'Enugu'),
('4', 'Dare', 'Adewale', 'dare.ad@hotmail.com', '0803‐123‐0004', 'Abuja'),
('5', 'Efe', 'Ojo', 'efe.oj@gmail.com', '0803‐123‐0005', 'PortHarcourt'),
('6', 'Aisha', 'Bello', 'aisha.bello@hotmail.com', '0803‐123‐0006', 'Kano'),
('7', 'Tunde', 'Salami', 'tunde.salami@yahoo.com', '0803‐123‐0007', 'Ilorin'),
('8', 'Nneka', 'Umeh', 'nneka.umeh@gmail.com', '0803‐123‐0008', 'Owerri'),
('9', 'Kelvin', 'Peters', 'kelvin.peters@hotmail.com', '0803‐123‐0009', 'Asaba'),
('10', 'Blessing', 'Mark', 'blessing.mark@gmail.com', '0803‐123‐0010', 'Uyo'); </pre>


#### Create table (ProductTB)

<pre>
  CREATE TABLE ProductTB (
ProductID INT PRIMARY KEY,
ProductName VARCHAR (50),
Category VARCHAR (50),
UnitPrice DECIMAL,
StockQty INT);

  INSERT RECORDS

  INSERT INTO ProductTB (ProductID, ProductName, Category, UnitPrice, StockQty)
VALUES
('1', 'Wireless Mouse', 'Accessories', '7500', '120'),
('2', 'USB‐CCharger 65W', 'Electronics', '14500', '75'),
('3', 'Noise‐CancelHeadset', 'Audio', '85500', '50'),
('4', '27" 4K Monitor', 'Displays', '185000', '20'),
('5', 'Laptop Stand', 'Accessories', '19500', '90'),
('6', 'Bluetooth Speaker', 'Audio', '52000', '60'),
('7', 'Mechanical Keyboard', 'Accessories', '18500', '40'),
('8', 'WebCam 1080p', 'Electronics', '25000', '55'),
('9', 'Smartwatch Series 5', 'Wearables', '320000', '30'),
('10', 'Portable SSD 1TB', 'Storage', '125000', '35'); </pre>



#### Create table (OrdersTB)  


<pre>
CREATE TABLE OrdersTB (
OrderID INT PRIMARY KEY,
CustomerID INT,
ProductID INT,
OrderDate DATE,
Quantity INT);

INSERT RECORDS 

INSERT INTO OrdersTB (OrderID, CustomerID, ProductID, OrderDate, Quantity)
VALUES
('1001', '1', '3', '2025‐06‐01', '1'),
('1002', '2', '1', '2025‐06‐03', '2'),
('1003', '3', '5', '2025‐06‐05', '1'),
('1004', '4', '4', '2025‐06‐10', '1'),
('1005', '5', '2', '2025‐06‐12', '3'),
('1006', '6', '7', '2025‐06‐15', '1'),
('1007', '7', '6', '2025‐06‐18', '2'),
('1008', '8', '8', '2025‐06‐20', '1'),
('1009', '9', '9', '2025‐06‐22', '1'),
('1010', '10', '10', '2025‐06‐25', '2'); </pre>



## Results
•	The table CustomerTB was successfully created with required columns and a primary key.
•	All customer records were inserted without errors.
•	Queries returned correct results based on sorting and filtering.

![image alt]https://github.com/Oluwato12-TB/SQL-Exam_Project/blob/main/CostumerTB.png
![image alt]https://github.com/Oluwato12-TB/SQL-Exam_Project/blob/main/ProductTB.png
![image alt]

