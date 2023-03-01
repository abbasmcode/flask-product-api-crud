# flask-product-api-crud
A Flask backend app with RESTful API for managing product database. Provides CRUD functionality via HTTP requests. Built with Flask-SQLAlchemy and Flask-Marshmallow extensions. Ideal for managing product data through an API.

This CRUD app is a backend application that provides a RESTful API for performing CRUD (create, read, update, delete) operations on a product database. The app uses the Flask web framework, along with the Flask-SQLAlchemy and Flask-Marshmallow extensions, to create the API that allows users to create, retrieve, update, and delete products.

The app provides the following endpoints:

POST /product - Creates a new product in the database
GET /product - Retrieves all products from the database
GET /product/{id} - Retrieves a single product from the database by ID
PUT /product/{id} - Updates a product in the database by ID
DELETE /product/{id} - Deletes a product from the database by ID
When a user sends a request to the API, the app retrieves data from the database using SQLAlchemy, serializes the data using Marshmallow, and sends a JSON response back to the user. The app also handles errors and provides appropriate responses for different types of errors.

For example, if a user sends a GET request to the /product endpoint, the app retrieves all products from the database, serializes them using Marshmallow, and sends a JSON response back to the user containing an array of all the products. Similarly, if a user sends a DELETE request to the /product/{id} endpoint with a valid ID, the app deletes the product with that ID from the database and sends a JSON response back to the user indicating success.

Overall, this CRUD app provides a simple but powerful way to manage a product database through a RESTful API.
