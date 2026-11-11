# Lab: Contractors Lab

## Overview
A Flask application that manages contract and customer lookup requests. The application provides two routes for retrieving contract information and verifying customer existence while protecting sensitive customer data.


## Features
- Contract Lookup: Retrieve contract information using a contract ID.
- Customer Verification: Verify whether a customer exists without exposing personal information.
- Error Handling: Return appropriate HTTP status codes when requested records cannot be found.


## Routes
- /contract/<id>

Retrieves contract information.

- /customer/<customer_name>

Verifies customer existence without returning personal information.


## Technologies Used
- Python
- Flask
- Pipenv
- Pytest


## Installation and Setup
1) Clone the repository:
git clone https://github.com/learn-co-curriculum/python-flask-contracts-lab.git

2) Navigate to project directory

3) Install dependencies:
pipenv install

4) Activate virtual environment:
pipenv shell


## HTTP Status Codes
- 200 OK: The requested contract was found and its information was returned.
- 204 No Content: The requested customer exists, but no information is returned.
- 404 Not Found: The requested contract or customer could not be found.