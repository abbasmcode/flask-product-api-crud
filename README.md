# Flask Product API CRUD

This is a simple Flask API that performs CRUD (Create, Read, Update, Delete) operations on a product entity. It utilizes SQLAlchemy to interact with a SQLite database and Marshmallow to serialize/deserialize objects.

## Requirements

This project requires the following dependencies:

- Flask
- Flask_SQLAlchemy
- Flask_Marshmallow

You can install them using pip:
`pip install Flask Flask_SQLAlchemy Flask_Marshmallow`


## Usage

1. Clone the repository and navigate to the project directory.
2. Initialize the database by running `python` in the terminal, then:
    ```
    from app import db
    db.create_all()
    exit()
    ```
3. Start the development server by running `python app.py`.
4. Use a tool such as Postman or cURL to send HTTP requests to the server.

### Available endpoints

- `POST /product`: creates a new product
- `GET /product`: retrieves all products
- `GET /product/<id>`: retrieves a single product by ID
- `PUT /product/<id>`: updates a single product by ID
- `DELETE /product/<id>`: deletes a single product by ID

License

This project is licensed under the MIT License - see the LICENSE file for details.
