# Shop-Product-Management-System
This project is a comphrehensive Shop Product Management System implemented using Model-View-Controller(MVC) architectural pattern and Java Database Connectivity(JDBC). The system facilitates efficient management of shop products, enabling users to perform various operations such as adding, updating, deleting, and fetching product details. Additionally, it prompts users to enter shop details on first run, which are then stored and automatically displayed on subsequent runs.
# Features
> Product Management

1. Add Product: Add new products to the shop.
2. Delete Product : Remove existing products from the shop by ID.
3. Fetch Product Details : Retrieve and display details of all products.
4. Update Product : Modify Product details such as name, price, quantity based on product ID.

> Shop Details Management

1. Prompt for shop details for first run.
2. Automatically fetch the details and display it from the second run ownwards.

> MVC Architecture

Ensures a clean separation of concerns, enhancing, ensuring persistent storage of shop and product information.
# Components
> Model

The model represents the data layer of the application :

1. Product : A class representing a product with attributes like 'id', 'name', 'price', 'quantity' and 'availability'.
2. Shop : A class representing shop details with attributes like 'id', 'shop_Name','shop_Address','Gstno', 'contactNo', 'ownerName'.
> View

The view is responsible for displaying information to the user :

1. ProductView : Handles the display of product details and user prompts.
2. ShopView : Manages the display of shop details.
> Controller

The Controller handles user inputs and updates the model and view :

1. ProductController : Manages the flow of product-related operations, processing user inputs and invoking model and view methods.
2. ShopController : Handles the flow of shop details management, ensuring shop details/information is entered and displayed correctly.
# Getting Started
> Prerequisites
1. Java Development Kit (JDK) 8 or higher.
2. A relational database. (eg.,MySQL, Postgresql)
3. JDBC driver for your chosen database.
# Setup Instructions
> Add PostgresSQL Dependency

Ensure you have maven installed. Then, add the PostgreSQL dependency to your 'pom.xml' file

![Screenshot (53)](https://github.com/user-attachments/assets/2f8dac30-b3fa-4b31-b6ee-e984f0f3987a)
> Configure Database

1. Set up your postgreSQL database and create the necessary tables.
2. Update the database configuration by providing proper URL, username, password.
# Usage
> Initial Setup

On the first run, the system will prompt you to enter shop details (name, address, contact, gstno, ownerName, Id). These details will be stored and automatically dispalyed/fetched on subsequent runs.
> Product Operations

1. Add Products : Follow the prompts to enter product details (id, name, price, quantity).
2. View Products : Displays a list of all products in the database.
3. Update Product :
   
   a) Select a product by ID to update.
   
   b) Specify what attributes you want to update : name, price or quantity.
4. Delete Product : Remove a product by its ID.
5. Example of first run :

For the first run you are prompt to enter shop details
