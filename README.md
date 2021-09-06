### Inventory-Managament-System
This repository contains all the files related to Inventory Management System project.

### Functionalities of this Project
1) The user can see all the products that are available in the inventory file records.json.
2) User can buy the product of his/her choice.
4) At last, a well-aligned Bill will be generated which contains all the details of the products bought.
5) When a user does a transaction then, that transaction will be added to sales.json file.
6) The owner can also add or delete products from the inventory.


### Functionality of Each File

### 1) records.json
This file contains the list of all the available products.
Product Id is the unique key of each product.
Each product has 5 attributes - Name, Quantity, MRP, Expiry Date and Discount

### 2) purchasing_products.ipynb
This file helps the user to buy any product available in the inventory.
First of all, the list of all the products available in the inventory is shown to the user.
Then, the user has to enter the Product Id and Quantity of the product (s)he has to purchase.
If the product is not available in the inventory then, a message informing "Product is not available in the inventory" is shown to the user.
But, if the product is available in the inventory then, the quantity of the product is checked whether the quantity user wants to purchase is available or not.
If that much of quantity is not available then, a message informing "Enough quantity is not present" is shown to user.
But, if enough quantity is present then, the quantity of the product purchased is updated in the inventory.
And, the transaction done is added to the sales.json file.
At last, the Bill of the shopping is displayed to the user.

### 3) adding_new_products.ipynb
Basically, this file is specially meant for the owner so, that (s)he can add or delete a product from the inventory.
First of all, the owner has to enter a choice whether (s)he wants to add a product or delete a product
If the owner wants to add a product to the inventory then, (s)he has to enter the details of the product.
If the product is already present in the inventory then, the details of that product is updated no new entry will be added to the records.json file.
But, if the product is not present in the inventory then, a new entry of the product will be added to the records.json file.
If the owner wants to delete a product then, (s)he has to enter the Product id of that product because every product has different product id.
And, the entry of that product will be deleted from the records.json file.
If the owner enters the wrong choice then, the program will prompt till the user enters the correct choice.

### 4) sales.json
This file contains the list of all the transactions done.
Transaction id is the unique key of each transaction.
Transaction id is generated with the help of uuid1() function.
Each Transaction has 6 attributes -   Product Id, Costumer Name, Quantity, Price, Grand Total and Time

