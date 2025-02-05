# Online Shop Backend

## Overview
This is the backend for an online shop built using **Node.js** and **Express.js**. It provides RESTful APIs for managing products, orders, and user carts.

## Tech Stack
- **Node.js**
- **Express.js**
- **Pug** (Template Engine)
- **EJS** (Template Engine)
- **Express-Handlebars** (Template Engine)
- **Body-Parser** (Middleware for parsing request bodies)
- **Nodemon** (For automatic server restarts during development)

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/jpayansh/online-shop.git
   ```
2. Navigate to the project directory:
   ```sh
   cd online-shop
   ```
3. Install dependencies:
   ```sh
   npm install
   ```
4. Start the development server:
   ```sh
   npm run dev
   ```
   This runs the server with **Nodemon**, allowing automatic restarts on code changes.

## API Endpoints

### Admin Routes
| Method | Endpoint | Description |
|--------|---------|-------------|
| GET    | `/admin/add-product` | Retrieve form to add a new product |
| GET    | `/admin/products` | Fetch all products |
| POST   | `/admin/add-product` | Add a new product |
| GET    | `/admin/edit-product/:productId` | Get edit form for a product |
| POST   | `/admin/edit-product` | Update product details |

### Shop Routes
| Method | Endpoint | Description |
|--------|---------|-------------|
| GET    | `/` | Homepage |
| GET    | `/products` | List all products |
| GET    | `/products/:productId` | Get details of a single product |
| GET    | `/cart` | View the shopping cart |
| POST   | `/cart` | Add a product to the cart |
| GET    | `/orders` | View customer orders |
| GET    | `/checkout` | Proceed to checkout |

## Project Structure
```
/online-shop-backend
│── /routes
│   ├── admin.js
│   ├── shop.js
│── /controllers
│   ├── adminController.js
│   ├── shopController.js
│── /views
│   ├── *.pug
│   ├── *.ejs
│── /models
│── /public
│── app.js
│── package.json
│── README.md
```

## Contributing
1. Fork the repository
2. Create a new branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m 'Add new feature'`
4. Push to your branch: `git push origin feature-name`
5. Submit a Pull Request

## License
This project is licensed under the MIT License.

