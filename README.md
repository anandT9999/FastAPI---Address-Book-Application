# Address Management App

## Description

This repository contains a FastAPI application for managing addresses and retrieving nearby addresses based on location coordinates. The application uses SQLite as the database to store address information.

## Files Structure

The repository includes the following files:

- **main.py**: This file contains the main FastAPI application code, including endpoint definitions and request handling logic.
- **database.py**: This file contains the Database class responsible for interacting with the SQLite database.
- **models.py**: This file contains the Pydantic models used for data validation and serialization/deserialization.
- **address_book.db**: This is the SQLite database file used to store address information.

## Features

The FastAPI application provides the following features:

- CRUD operations for managing addresses:
  - Create a new address
  - Update an existing address
  - Delete an address
  - Retrieve a list of all addresses
  - Retrieve a single address by ID

- Endpoint to retrieve nearby addresses based on location coordinates:
  - Given latitude, longitude, and a distance radius, retrieve nearby addresses within the specified distance.

## How to Use

To use the application, follow these steps:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/address-management-app.git

Install the required dependencies:

pip install -r requirements.txt

Run the FastAPI application:

uvicorn main:app --reload

Access the Swagger documentation at http://localhost:8000/docs to interact with the API endpoints.

Testing the Nearby Addresses Endpoint

To test the endpoint for retrieving nearby addresses, follow these steps:

Open the Swagger documentation at http://localhost:8000/docs.
Navigate to the /addresses/nearby/ endpoint.
Input the latitude, longitude, and distance values in the provided fields.
Click the "Try it out" button and then "Execute" to send the request.
View the response to see the nearby addresses retrieved based on the provided location coordinates and distance.
Running the Application Locally
