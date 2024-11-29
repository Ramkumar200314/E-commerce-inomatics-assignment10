# E-Commerce Website (MERN Stack)

This is an e-commerce platform developed using the MERN stack (MongoDB, Express.js, React, Node.js). The application provides a fully functional online shopping experience, including features like user authentication, product listing, cart management, order placement, and more.

## Features

- **User Authentication**: Users can register, login, and logout. JWT (JSON Web Tokens) are used for authentication.
- **Product Management**: Admins can add, update, and delete products.
- **Product Catalog**: Users can browse products, filter by categories, and view product details.
- **Shopping Cart**: Users can add products to their cart, update quantities, and remove items.
- **Order Management**: Users can place orders, and admins can view and manage orders.
- **Payment Integration**: Integrates with Stripe or PayPal for payment processing (optional).
- **Responsive UI**: Fully responsive front-end built with React, ensuring a smooth experience on both desktop and mobile devices.

## Tech Stack

- **Frontend**: 
  - React.js
  - Redux (for state management)
  - React Router (for routing)
  - Axios (for making HTTP requests)
  - Material UI / Bootstrap (for UI components and styling)

- **Backend**: 
  - Node.js
  - Express.js
  - MongoDB (with Mongoose for ODM)
  - JWT for authentication
  - Bcrypt for password hashing

- **Payment Integration**: Stripe / PayPal (optional)

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/e-commerce-mern.git
cd e-commerce-mern
```

### 2. Install dependencies

#### Backend (Node.js / Express.js)

Navigate to the `backend` folder and install the necessary dependencies:

```bash
cd backend
npm install
```

#### Frontend (React.js)

Navigate to the `frontend` folder and install the necessary dependencies:

```bash
cd frontend
npm install
```

### 3. Setup Environment Variables

Create a `.env` file in both the `frontend` and `backend` folders and set the necessary environment variables.

#### Backend `.env`

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/ecommerce
JWT_SECRET=your_jwt_secret_key
PAYPAL_CLIENT_ID=your_paypal_client_id
STRIPE_SECRET_KEY=your_stripe_secret_key
```

#### Frontend `.env`

```env
REACT_APP_API_URL=http://localhost:5000/api
```

### 4. Running the Application

#### Start the Backend

Navigate to the `backend` folder and run:

```bash
cd backend
npm start
```

This will start the backend server on `http://localhost:5000`.

#### Start the Frontend

Navigate to the `frontend` folder and run:

```bash
cd frontend
npm start
```

This will start the frontend development server on `http://localhost:3000`.

## Usage

1. **Sign Up / Login**: Create a new account or log in with existing credentials.
2. **Browse Products**: Browse through the available products, view details, and add them to the cart.
3. **Manage Cart**: View your cart, update quantities, or remove items.
4. **Checkout**: Proceed to checkout and enter your shipping information. You can pay via Stripe or PayPal (depending on your setup).
5. **Order History**: Users can view their order history, and admins can manage orders from the admin panel.

## API Endpoints

### Auth Routes

- **POST /api/auth/register** - Register a new user
- **POST /api/auth/login** - Login and return JWT token
- **GET /api/auth/user** - Get the authenticated user's data

### Product Routes

- **GET /api/products** - Get a list of all products
- **GET /api/products/:id** - Get a specific product by ID
- **POST /api/products** - Add a new product (admin only)
- **PUT /api/products/:id** - Update a product (admin only)
- **DELETE /api/products/:id** - Delete a product (admin only)

### Cart Routes

- **GET /api/cart** - Get the user's cart
- **POST /api/cart** - Add an item to the cart
- **PUT /api/cart** - Update the quantity of an item in the cart
- **DELETE /api/cart/:id** - Remove an item from the cart

### Order Routes

- **GET /api/orders** - Get a list of all orders (admin only)
- **POST /api/orders** - Place a new order
- **GET /api/orders/:id** - Get a specific order by ID

## Screenshots

Include a few screenshots here to showcase the user interface and features.

## Contributing

If you would like to contribute to this project, feel free to fork the repository and submit a pull request. Please ensure your code follows the existing style and includes relevant tests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

