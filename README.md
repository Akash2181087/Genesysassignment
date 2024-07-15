Perry’s Summer Vacation Goods and Services Message API Test Suite
This repository contains automated tests written in Java using JUnit and RestAssured to verify the functionality of Perry’s Summer Vacation Goods and Services Message API.

Prerequisites
Java Development Kit (JDK) installed on your machine.
Apache Maven for managing dependencies and building the project.
Knowledge of Java, JUnit, and RestAssured library for API testing.

Setup Instructions

Clone the Repository:
Use the following command to clone the repository:
**git clone <repository-url>
cd <repository-directory>**

Install Dependencies:
This project uses Maven for dependency management. Run the following command to install all necessary dependencies:
**mvn clean install**

Run Tests:
Execute the tests using Maven:
**mvn clean test**

Test Structure
The test suite includes the following tests to ensure the Message API functions correctly:

Create Message: Tests the creation of a new message.
Get Message by ID: Retrieves a message by its unique identifier.
Update Message: Modifies the content of an existing message.
Delete Message: Deletes a message from the system.

Test Cases

Create Message:
Sends a POST request to create a new message.
Verifies the response status code is 201 (Created).
Stores the ID of the created message for subsequent tests.

Get Message by ID:
Sends a GET request to retrieve the message by its ID.
Asserts that the response status code is 200 (OK).
Checks if the retrieved message ID matches the one created in the previous step.

Update Message:
Sends a PUT request to update the message content.
Validates the response status code is 200 (OK).
Verifies that the updated message content matches the sent request.

Delete Message:
Sends a DELETE request to remove the message from the system.
Ensures the response status code is 204 (No Content), indicating successful deletion.

Environment Configuration:
Adjust the baseUrl variable in MessageApiTest.java to match your local or deployed environment.







