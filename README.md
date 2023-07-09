# SQL-SupplyChainMgt
SQL Group Final Project 2022 -- Humber College

This project is related to Supply Chain Management, which includes customer order and return transactions, in IT Gadgets Store in Canada. 

#### Key activities:
1) Define 10 business rules for Supply Chain Management in the IT Gadget Store
2) Define a Conceptual, Logical, and Physical Entity Relationship Diagram (ERD)
3) Create tables and populate data into each table
4) Query data to support and tackle business insights

<img width="1043" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/0ea0e317-4ac5-4c5f-83de-fa9d95ee9fa8">

#### 10 Business rules:
1. Supplier – Product
One supplier can supply zero or many products, while a single product would be supplied by one or multiple suppliers.

2. Supplier – DeliveryNote
One supplier can create one or many delivery notes, while a single delivery note would be created for one supplier.

3. Customer – CustomerDetail
One customer can have a single customer detail, while a single customer detail would be under one customer.

4. Customer – SalesOrder
One customer can have zero or many sales orders, while one sales order would be ordered by only one customer.

5. SalesOrder – DeliveryNote:
One sales order will generate one or multiple delivery notes, while there will be one or multiple sales orders under one delivery note.

6. SalesOrder – LineItem
One sales order can have one or multiple LineItem, while a single LineItem would be under one and only one sales order.

7. Product – LineItem
One LineItem would contain one and the only one product, while One product would be in one or multiple LineItems.

8. LineItem – ReturnProduct
One LineItem can have a single return, while a single return would be under one LineItem.

9. LineItem – DeliveryNote
One LineItem would be in one or many DeliveryNote, while a DeliveryNote would contain one or many LineItem.

10. DeliveryNote – Truck
One DeliveryNote will be shipped by one and the only one truck, while one truck will deliver one or many DeliveryNote.

#### Create tables identified in the SQL Server database with respective constraints (with SQL)
<img width="904" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/aa2ba72b-3192-4ecc-89d0-7c5e72f0309f">

#### Populate each table with dummy data (with SQL)
Table: Customer
<img width="905" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/53a76b23-980b-4749-873a-b5fc3c455ef5">

Table: Customer Details
<img width="905" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/ae28e784-fe86-4e81-86e3-51fd3ce88307">

Table: Product
<img width="906" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/c9ff04f1-9fe4-4c95-836e-9783b4f3ba41">

Table: Truck
<img width="906" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/d268605f-baea-41e1-b69d-24e8d5e998ab">

Table: Sales Order
<img width="906" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/77faf976-f0df-4014-887b-e78848503825">

Table: Delivery Note
<img width="906" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/b9053b50-f7e1-42a0-970c-fbcee0dde777">

Table: Return Product
<img width="904" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/ed76f535-d274-4ec3-9bf5-166be31226e9">

#### Query data from tables
1) Query to calculate the number of sales orders and total sales amount from the table: Sales Order
Finding: We found that there are a total of 118 sales orders amounting to $38,333.29

![image](https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/86406ff7-8200-4ada-b5fb-937dc7655dbb)

<img width="912" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/4584e026-4cba-499b-9b72-1a92a00d43c1">

2) Query to find how many different products, which are more than $300 and belong to which category
Finding: For listed products with more than $300, we found that all listed products belong to "Technology."

![image](https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/ab54456c-9e19-4e76-b8cd-2a05c95af404)

<img width="911" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/6bcd831a-c489-453a-987a-ef0abf9b6878">

3) Query to find the specific product name to list all suppliers who can provide this product
Finding: 7 suppliers can provide this product. The result comes up with the supplier ID, name, and contact.

![image](https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/2ac72c73-d037-48be-be86-99eef8dbfaaf)

<img width="801" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/7167c762-4764-4887-befc-533866966981">

4) Query to find the product return that more than 2 items and analyze the reason for returning
Finding: From this analysis, we can see that major customer return reasons are from products arriving late and they are not satisfied with the products. So the company can use these findings to investigate for future improvement.

![image](https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/0e337a13-b1e9-4316-84ec-1fa5e89633fc)

<img width="909" alt="image" src="https://github.com/vcmeghan/SQL-SupplyChainMgt/assets/100189862/c62984c8-66e0-4fce-b63c-0fb63416ad1e">


