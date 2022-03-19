# Backend Take Home Assignment

This is a take home assignment for backend developers applying to IDFlo.

## Introduction

You need to write a command line based tool to handle a warehouse by adding or removing inventory in the form of products you can create or delete. This project will require you to create a DB schema in MySQL (or any RDBMS of your choice) and persist all the data into the database.

You need to allow a user to enter any 1 of the following commands into the console after starting your program:

* CREATE WAREHOUSE
* DELETE WAREHOUSE
* CREATE PRODUCT
* DELETE PRODUCT
* STOCK WAREHOUSE
* UNSTOCK WAREHOUSE
* LIST PRODUCTS
* LIST STOCK

### Explanation Of The Commands

The following is an explanation of each of the above commands

#### CREATE WAREHOUSE
This is the expected format of the command:  `CREATE WAREHOUSE --name ${warehouseName}`
This command is used to create a new warehouse

#### DELETE WAREHOUSE
This is the expected format of the command: `DELETE WAREHOUSE --name ${warehouseName}`
This command is used to delete an existing warehouse

#### ADD PRODUCT
This is the expected format of the command: `CREATE PRODUCT --name ${productName} --sku ${skuNumber}`
This command is used to create a new product. Here the skuNumber can be a 10 character alphanumeric string and it must be unique for each product

#### DELETE PRODUCT
This is the expected format of the command: `DELETE PRODUCT --sku ${skuNumber} --quantity ${quantity}`
This command is used to delete an existing product. The user can provide a quantity that may exceed the product quantity currently in the DB

#### STOCK WAREHOUSE
This is the expected format of the command: `STOCK WAREHOUSE --warehouse ${warehouseName} --sku ${skuNumber} --quantity ${quantity}`
This command is used to add a certain product's stock to a warehouse.

#### UNSTOCK WAREHOUSE
This is the expected format of the command: `UNSTOCK WAREHOUSE --warehouse ${warehouseName} --sku ${skuNumber} --quantity ${quantity}`
This command is used to remove a certain product's stock from a warehouse.

#### LIST PRODUCTS
This is the expected format of the command: `LIST PRODUCTS --warehouse ${warehouseName}`
This command is used to list all details of all products in a warehouse.


### Criteria

Your assignment will be scored based on the following criteria:

1. Your ability to clearly understand the instructions laid out in the assignment and ask questions to clear up any doubts
2. Your ability to architect your code in a way that is scalable.
3. The readability of your code. You can choose to emphasize the readability either through code style or documentation.
4. The design of your SQL schema

Good luck!
