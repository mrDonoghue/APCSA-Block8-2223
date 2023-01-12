# AdvancedArrayChallenge

## Problem Description
Write a program that implements a simple inventory management system for a small store. The program should read a list of products and their quantities from a file, and store the data in an array of product objects. Each product object should have the following attributes:

* Product name
* Product ID
* Quantity in stock
* Reorder threshold
* Restock level

The program should then provide the following functionality:

* Display the current inventory
* Allow the user to search for a product by name or ID
* Allow the user to update the quantity of a product in the inventory
* Allow the user to add a new product to the inventory
* Automatically reorder products that have reached their reorder threshold


To make this problem more challenging, you may also choose to implement one or more of the following additional features:

* Generate reports on the inventory (e.g., a list of low-stock items, a list of expired products, etc.)
* Process orders from customers
* Track the sales history of each product
## Input
The input file will contain a list of products, one per line, in the following format:
```
product_name,product_id,quantity,reorder_threshold,restock_level
```

## Output
The program should output the following:

* A list of the products and their quantities in the inventory
* The search results for a product search
* A message indicating the success or failure of an update or add operation
* A message indicating which products were reordered and the quantities that were reordered

## Constraints
* The product names and IDs will be alphanumeric strings with a maximum length of 100 characters.
* The quantities and reorder thresholds will be positive integers.
* The restock level will be a positive integer or zero.

#### Step by step? needs editing for sure
Open replit

Define a Product class that represents a product in the inventory. The Product class should have the following attributes:

* name: a String representing the product name
* id: a String representing the product ID
* quantity: an int representing the quantity in stock
* reorderThreshold: an int representing the reorder threshold
* restockLevel: an int representing the restock level

Define appropriate constructors, getters, and setters for the Product class.

Write a method that reads the input file and creates an array of Product objects based on the data in the file. The method should take the name of the input file as a parameter and return the array of Product objects.

Write a method that displays the current inventory. The method should take an array of Product objects as a parameter and display a list of the products and their quantities.

Write a method that searches for a product in the inventory by name or ID. The method should take an array of Product objects and a search query as parameters, and return the index of the product in the array if it is found, or -1 if it is not found.

Write a method that updates the quantity of a product in the inventory. The method should take an array of Product objects and an index as parameters, and allow the user to enter a new quantity for the product at the specified index.

Write a method that adds a new product to the inventory. The method should take an array of Product
