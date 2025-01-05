# Fruit Sell Order System

## Overview
The **Fruit Sell Order System** is a full-stack web application designed to streamline the ordering and management process for fruit sales. It allows customers to browse and place orders for various fruits, while administrators can manage inventory, process orders, and track sales. The system provides an intuitive interface for both customers and admins, offering a smooth experience for buying and selling fruits.

This project is built using modern web development technologies to demonstrate the full-stack capabilities, including a front-end for user interaction, a back-end for processing logic, and a database to store all necessary data.

## Features
- **Customer Side**:
  - Browse available fruits with detailed descriptions and prices.
  - Add fruits to the cart and modify quantity.
  - Place an order with personal and payment information.
  - View order history and status.
  
- **Admin Side**:
  - View and manage the inventory of fruits.
  - View and process customer orders.
  - Track sales data and generate reports.

## Technologies Used
### Frontend:
- **React.js**: For building a responsive and dynamic user interface.
- **Redux**: For managing global state.
- **CSS/SCSS**: For styling the application and making it visually appealing.

### Backend:
- **Node.js**: Server-side environment.
- **Express.js**: Web framework for building the RESTful API.
- **JWT Authentication**: For securing endpoints and handling user authentication.
  
### Database:
- **MongoDB**: A NoSQL database to store product, order, and user data.

### Other Tools:
- **Mongoose**: MongoDB Object Data Modeling (ODM) library for Node.js.
- **Axios**: For making HTTP requests from the client-side.
- **Stripe API**: For handling payment processing.

## Installation

### Prerequisites
Before starting, ensure that you have the following installed:
- **Node.js**: [Download and Install Node.js](https://nodejs.org/)
- **MongoDB**: [Install MongoDB](https://www.mongodb.com/try/download/community) (Or use MongoDB Atlas for cloud DB)
  
### Setup Instructions

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/fruit-sell-order-system.git
    cd fruit-sell-order-system
    ```

2. **Install dependencies**:
    For the backend:
    ```bash
    cd backend
    npm install
    ```
    For the frontend:
    ```bash
    cd frontend
    npm install
    ```

3. **Configure Environment Variables**:
    Create a `.env` file in the **backend** directory with the following environment variables:
    ```bash
    MONGO_URI=<your-mongo-db-uri>
    JWT_SECRET=<your-secret-key>
    STRIPE_SECRET_KEY=<your-stripe-secret-key>
    ```

4. **Run the Application**:
    - In the **backend** directory:
    ```bash
    npm start
    ```

    - In the **frontend** directory:
    ```bash
    npm start
    ```

    The backend will run on `http://localhost:5000` and the frontend on `http://localhost:3000`.

## Folder Structure
```
fruit-sell-order-system/
├── backend/
│   ├── controllers/       # Business logic for API endpoints
│   ├── models/            # Database models
│   ├── routes/            # API route definitions
│   ├── config/            # Configuration files (e.g., environment variables)
│   └── server.js          # Entry point of the backend application
│
├── frontend/
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── pages/         # React components for different views (e.g., home, order)
│   │   ├── actions/       # Redux actions for state management
│   │   ├── reducers/      # Redux reducers for managing the state
│   │   ├── App.js         # Main React component
│   │   └── index.js       # Entry point of the frontend application
│   └── public/
│       └── index.html     # HTML file for the frontend
│
└── README.md              # Project documentation
```

## Usage

### Customer
1. Open the app in your browser.
2. Browse the available fruits and add them to your cart.
3. Proceed to checkout and enter shipping and payment information to complete the order.
4. View your order history and track the status of your current orders.

### Admin
1. Log in using the admin credentials.
2. View all incoming orders and mark them as processed.
3. Manage the inventory by adding, updating, or removing fruits.
4. View sales reports and statistics.

## Contributing
We welcome contributions from the community! If you'd like to contribute, follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`.
3. Make your changes and commit them: `git commit -am 'Add feature'`.
4. Push to your branch: `git push origin feature-branch`.
5. Open a pull request describing your changes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- This project uses the **Stripe API** for payment processing.
- Thanks to **React**, **Node.js**, and **MongoDB** for providing the technologies that made this application possible.

--- 

This should give you a comprehensive idea about the project, from installation to usage and contribution!
