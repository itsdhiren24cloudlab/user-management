# user-management
Spring Boot CRUD application for User management.

# User Management Application

The User Management Application is a Spring Boot-based web application that provides CRUD (Create, Read, Update, Delete) functionality for managing user records in a MySQL database.

## Features

- Create, update, and delete user records.
- View a list of all user records.
- Search for users by various criteria.
- Store user information in a MySQL database.

## Technologies Used

- Spring Boot: A powerful framework for building Java applications.
- MySQL: A relational database management system for data storage.
- POSTMANThymeleaf: A Java-based templating engine for server-side rendering.
- Maven: A build and project management tool for Java applications.

## Prerequisites

- Java Development Kit (JDK) 17 or later
- MySQL Database
- Maven
- IDE (e.g., IntelliJ IDEA)

## Getting Started

1. Clone the repository to your local machine:

   ```shell
   git clone https://github.com/yourusername/user-management-app.git
## Database Configuration
Configure your MySQL database connection in application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/user_management
spring.datasource.username=yourusername
spring.datasource.password=yourpassword
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
spring.mvc.content.negotiation.defaultContentType=application/json
## Testing the REST API with Postman

You can use Postman, a popular API testing tool, to interact with the User Management Application's REST API. Here are the steps to get you started:

1. **Install Postman:** If you haven't already, download and install Postman from the [Postman website](https://www.postman.com/downloads/).

2. **Import the Postman Collection:** Download the Postman collection for this API from the following link: [User Management API Postman Collection](#). Import the collection into Postman by following these steps:
   
   - Launch Postman.
   - Click on the "Import" button.
   - Choose the downloaded collection file.

3. **Set Environment Variables:** To simplify testing, configure environment variables in Postman to store your API base URL. Here are the required variables:

   - `base_url`: The base URL of your User Management Application, e.g., `http://localhost:8080/api`.

4. **Perform API Operations:**
   - Use the imported Postman collection to perform CRUD operations on the User Management Application. The collection includes requests for creating, updating, deleting, and retrieving user records.

5. **Run the Requests:**
   - Run the requests in the Postman collection, and observe the responses to verify the functionality of your API.

Please make sure your User Management Application is running before testing with Postman.

## API Endpoints

Here are the API endpoints you can interact with using Postman:

- `GET /api/users`: Get a list of all users.
- `GET /api/users/{id}`: Get a specific user by ID.
- `POST /api/users`: Create a new user.
- `PUT /api/users/{id}`: Update an existing user.
- `DELETE /api/users/{id}`: Delete a user by ID.

Remember to replace `{id}` with the actual user's ID when using the respective endpoints.

**Note:** Ensure that you include appropriate authentication and authorization mechanisms if your API requires them. This example assumes that your API is open for testing.


