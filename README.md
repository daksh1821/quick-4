# QuickCommerce Grocery Delivery Website

QuickCommerce is a MERN stack-based grocery delivery website that provides a seamless shopping experience. The platform is designed to offer quick and easy access to various grocery items, along with secure and efficient management of cart and payment features. This README provides a detailed overview of the project, including its setup, structure, and features.

---

## Features

### Frontend (React.js)
- **Dynamic Product Listing:** Displays a variety of products with detailed descriptions, nutritional information, pricing, and discounts.
- **Product Counter:** Add or remove items from the cart with real-time updates.
- **Interactive UI:** Responsive and user-friendly interface.
- **Routing:** React Router for seamless navigation.

### Backend (Node.js and Express.js)
- **API Development:** RESTful API for managing products, user authentication, and cart operations.
- **Authentication:** JWT-based authentication system.
- **Database:** MongoDB for storing user and product information.
- **Secure Data Handling:** Password hashing and validation.

---

## Project Structure

### Backend Directory
```plaintext
/backend
|-- controllers
|   |-- authController.js
|   |-- productController.js
|-- models
|   |-- User.js
|   |-- Product.js
|-- routes
|   |-- authRoutes.js
|   |-- productRoutes.js
|-- config
|   |-- db.js
|-- middlewares
|   |-- authMiddleware.js
|-- .env
|-- server.js
```
- **controllers/**: Contains logic for handling requests.
- **models/**: Defines database schemas.
- **routes/**: Defines API routes.
- **middlewares/**: Contains middleware like authentication.
- **config/**: Database connection file.
- **server.js**: Main server entry point.

### Frontend Directory
```plaintext
/frontend
|-- public
|   |-- index.html
|-- src
|   |-- components
|   |   |-- ProductCard.js
|   |   |-- Cart.js
|   |-- pages
|   |   |-- Home.js
|   |   |-- Services.js
|   |-- App.js
|   |-- index.js
|-- package.json
```
- **components/**: Reusable components like ProductCard and Cart.
- **pages/**: Pages like Home and Services.
- **App.js**: Main React app entry point.
- **index.js**: Renders the app.

---

## Installation

### Prerequisites
- Node.js (v16+)
- MongoDB
- npm or yarn

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/quick-commerce.git
   cd quick-commerce
   ```
2. Install dependencies for both backend and frontend:
   ```bash
   cd backend
   npm install
   cd ../frontend
   npm install
   ```
3. Configure environment variables:
   - Create a `.env` file in the `backend` directory with the following:
     ```env
     PORT=5000
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_jwt_secret
     ```
4. Start the development servers:
   - Backend:
     ```bash
     cd backend
     npm start
     ```
   - Frontend:
     ```bash
     cd frontend
     npm start
     ```
5. Open the app in your browser at `http://localhost:3000`.

---

## API Endpoints

### Authentication
- `POST /api/auth/register`: Register a new user.
- `POST /api/auth/login`: Log in a user.

### Products
- `GET /api/products`: Get all products.
- `GET /api/products/:id`: Get a specific product by ID.

### Cart
- `POST /api/cart`: Add a product to the cart.
- `GET /api/cart`: Get user cart.
- `DELETE /api/cart/:id`: Remove a product from the cart.

---

## Technologies Used

### Frontend
- React.js
- React Router
- CSS for styling

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT for authentication

---

## Future Enhancements
- Implement payment gateway integration.
- Add order tracking functionality.
- Enable product reviews and ratings.
- Develop a mobile app version.

---

## Contributors
- **Daksh Jain**

---

## License
This project is licensed under the MIT License.

---

## Contact
For any inquiries, please contact [Daksh Jain](mailto:daksh2872004@gmail.com).
