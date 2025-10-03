#10Pearls-Internship-Assignment-No-4

Project Overview

This project demonstrates API testing using Postman collections with multiple HTTP methods.
We tested the Simple Books API and JSONPlaceholder API by creating, updating, retrieving, and deleting resources.

# Learning Objectives

Through this assignment, the following objectives were achieved:

Creating and managing Postman collections

Using collection variables and dynamic data

Writing assertions with ChaiJS

Parsing JSON responses and logging values

Implementing Pre-request scripts and Tests

Chaining APIs by passing values between requests

Executing the full collection with Collection Runner

# Tools & Technologies

Postman

Simple Books API → https://simple-books-api.glitch.me

JSONPlaceholder → https://jsonplaceholder.typicode.com

# Tasks Completed

Used all HTTP methods (GET, POST, PUT, PATCH, DELETE)

Set Base URL as variable ({{baseUrl}})

Generated random request body data (clientName, clientEmail, customerName, title)

Parsed JSON responses and logged values to console

Added Chai assertions (including one intentional failing test)

Used Pre-request & Tests tabs for variable handling

Chained APIs using variables (e.g., orderId, accessToken)

Ran entire collection with Collection Runner

# Requests in Collection
1. GET /books

Fetch list of books

Tests: status 200, response JSON, length check

2. GET /books/:id

Fetch single book by ID

Tests: validate id, failing test included

3. POST /api-clients

Register new API client (generates accessToken)

Dynamic clientName & clientEmail

Token stored as collection variable

4. POST /orders

Create a new order with bookId & customerName

OrderId stored for later requests

5. GET /orders/:id

Retrieve specific order details

Validate orderId matches

6. PATCH /orders/:id

Update order partially (customerName)

Validate update

7. DELETE /orders/:id

Delete order by ID

Response 200/204

8. PUT /posts/1 (JSONPlaceholder demo)

Demonstration of PUT (full update)

Used random title

# Test Results

All major requests passed successfully

One failing test case (book type = science) is intentional, as required in assignment instructions

THIS README includes
Postan json file
A detailed step-by-step guide (with all requests, variables, scripts, and verification steps) is provided in the attached PDF file
