##Dosa Restaurant REST API Backend:

This project is a REST API backend for a dosa restaurant. It provides CRUD (Create, Read, Update, Delete) operations for three main objects: customers, items, and orders. The backend is built using FastAPI and uses an SQLite database to store and retrieve data.

##Project Structure:

-db_init.py: Script to initialize an empty SQLite database with relational constraints based on the provided example_orders.json file.

-main.py: FastAPI application implementing endpoints for CRUD operations on customers, items, and orders.

-example_orders.json: Sample data file used to populate the database during initialization.

-db.sqlite: SQLite database file where data is stored.

##Installation and Setup:

Clone the repository:

'''python
git clone <repository_url>

##Install dependencies:

'''python
pip install fastapi

'''python
install fastapi uvicorn

'''python
pip install pydantic

##Database Initialization:

To initialize the SQLite database with sample data:

'''python
python db_init.py

This script creates tables for customers, items, and orders, and populates them with data from 'example_orders.json'.

##Running the FastAPI Application:

To start the FastAPI application:

'''css
uvicorn main:app --reload

The API will be available at ##http://localhost:8000.

##API Endpoints

Customers:

-POST /customers/: Create a new customer.
-GET /customers/{cust_id}: Retrieve a customer by ID.
-PUT /customers/{cust_id}: Update a customer by ID.
-DELETE /customers/{cust_id}: Delete a customer by ID.

Items:

-POST /items/: Create a new item.
-GET /items/{item_id}: Retrieve an item by ID.
-PUT /items/{item_id}: Update an item by ID.
-DELETE /items/{item_id}: Delete an item by ID.

Orders:

-POST /orders/: Create a new order.
-GET /orders/{order_id}: Retrieve an order by ID.
-PUT /orders/{order_id}: Update an order by ID.
-DELETE /orders/{order_id}: Delete an order by ID.

##Usage:

Use any HTTP client (e.g., Postman, curl) to interact with the API endpoints.

Refer to the API documentation or OpenAPI schema (http://localhost:8000/docs) for detailed usage instructions.
