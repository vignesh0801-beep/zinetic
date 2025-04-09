Book Store App - Spring Boot + MongoDB

This is a Bookstore web application built using Spring Boot, MongoDB, and Cloudinary. It provides RESTful APIs to manage books with full CRUD functionality.

Features

Create, Read, Update, and Delete books
Stores book title, author, summary, publish year, ISBN, and image
Image hosting with Cloudinary
MongoDB for storing data
Swagger for API documentation
Built with Spring Boot and Maven
Tech Stack

Spring Boot
MongoDB
Maven
Cloudinary
Swagger
Setup Instructions

Clone the repository:t

Navigate into the project directory: cd bookstore-web-application

Make sure you have JDK 17+ and Maven installed and configured: mvn -v

Configure MongoDB: Update src/main/resources/application.properties with your MongoDB URI. Example for local MongoDB: spring.data.mongodb.uri=mongodb://localhost:27017/bookstore

Configure Cloudinary: Create a Cloudinary account and add the credentials in application.properties: cloudinary.cloud-name=your_cloud_name cloudinary.api-key=your_api_key cloudinary.api-secret=your_api_secret

Run the application: mvn spring-boot:run

Open the application: API base URL: http://localhost:6969/api/v1/books/ Swagger UI: http://localhost:6969/

API Endpoints

GET /api/v1/books - Get all books
GET /api/v1/books/{id} - Get book by ID
POST /api/v1/books - Add a new book (multipart/form-data with image)
PUT /api/v1/books/{id} - Update an existing book
DELETE /api/v1/books/{id} - Delete a book by ID
Note

Ensure MongoDB is running locally or accessible via URI before starting the app. If using Cloudinary, verify credentials are valid.
