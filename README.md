## Introduction <a name="introduction"></a>

The E-commerce Backend is a powerful application that manages the backend operations of an e-commerce platform. This application is built using Express.js for routing, Sequelize ORM for database interactions, and MySQL as the database.

## Table of Contents

1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Usage](#usage)
4. [API Routes](#api-routes)
5. [Database Models](#database-models)
6. [Data Seeding](#data-seeding)
7. [Environment Setup](#environment-setup)
8. [Contributing](#contributing)
9. [Contact](#contact)

## Installation <a name="installation"></a>

Follow these steps to get the E-commerce Backend up and running:

1. Clone this repository to your local machine.
2. Navigate to the project directory in your terminal.
3. Run `npm install` to install the required dependencies.

## Usage <a name="usage"></a>

To start the server, run `npm start`.

Access the API endpoints using tools like [Postman](https://www.postman.com/) or `curl` commands. Refer to the [API Routes](#api-routes) section for details on available endpoints and their functionalities.

## API Routes <a name="api-routes"></a>

The E-commerce Backend provides the following API routes:

- **Categories:**

  - `GET /api/categories`: Fetch all categories with associated products.
  - `GET /api/categories/:id`: Get a category by its ID with associated products.
  - `POST /api/categories`: Create a new category.
  - `PUT /api/categories/:id`: Update a category's name by its ID.
  - `DELETE /api/categories/:id`: Delete a category by its ID.

- **Products:**

  - `GET /api/products`: Retrieve all products with associated category and tags.
  - `GET /api/products/:id`: Fetch a product by its ID with associated category and tags.
  - `POST /api/products`: Create a new product.
  - `PUT /api/products/:id`: Update a product's data by its ID.
  - `DELETE /api/products/:id`: Remove a product by its ID.

- **Tags:**
  - `GET /api/tags`: Get all tags with associated products.
  - `GET /api/tags/:id`: Fetch a tag by its ID with associated products.
  - `POST /api/tags`: Create a new tag.
  - `PUT /api/tags/:id`: Update a tag's name by its ID.
  - `DELETE /api/tags/:id`: Delete a tag by its ID.

## Database Models <a name="database-models"></a>

The application defines the following Sequelize models:

- **Category:** Represents a product category.
- **Product:** Represents a product with details like name, price, and stock.
- **Tag:** Represents a tag associated with products.
- **ProductTag:** Represents the relationship between products and tags.

## Data Seeding <a name="data-seeding"></a>

Seed files are included to populate the database with sample data. Run `npm run seed` to execute the seed files and populate the database with categories, products, tags, and product-tag associations.

## Environment Setup <a name="environment-setup"></a>

Before running the application, update the `.env` file with your MySQL database credentials:

```dotenv
DB_NAME='ecommerce_db'
DB_USER='<Your Database User>'
DB_PASSWORD='<Your Database Password>'
```

## Contributing <a name="contributing"></a>

Contributions are welcome! If you find any issues or have suggestions, feel free to create a pull request.

## Contact <a name="contact"></a>

If you have questions or need assistance, you can contact me at [moerahman1234@gmail.com ](mailto:your.email@example.com).

---

Feel free to customize this README to your needs. It's designed to provide comprehensive information about the E-commerce Backend, making it easier for users and developers to understand, install, and utilize the application.
