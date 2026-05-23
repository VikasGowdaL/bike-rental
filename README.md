# Bike Rental Web Application

A full-stack MERN (MongoDB, Express.js, React.js, Node.js) based Bike Rental Management System that allows users to browse available bikes, make bookings, and perform secure online payments using Stripe.

---

## Features

### User Features
- View all available bikes
- Check bike details
- Book bikes for specific time slots
- Secure online payment integration using Stripe
- View booking information

### Admin Features
- Add new bikes
- Edit bike details
- Delete bikes
- Manage bike availability
- View all bookings

---

## Tech Stack

### Frontend
- React.js
- Axios
- Bootstrap

### Backend
- Node.js
- Express.js

### Database
- MongoDB
- Mongoose

### Payment Gateway
- Stripe

---

## Project Structure

```bash
bike-rental/
│
├── client/                 # React frontend
│
├── models/                 # Mongoose models
│   ├── bikeModel.js
│   ├── bookingModel.js
│   └── userModel.js
│
├── routes/                 # Express route handlers
│   ├── bikesRoute.js
│   ├── bookingsRoute.js
│   └── usersRoute.js
│
├── server.js               # Main backend server
├── package.json
├── .env
└── .gitignore
```

---

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/VikasGowdaL/bike-rental.git
```

---

### 2. Navigate to the Project Directory

```bash
cd bike-rental
```

---

### 3. Install Backend Dependencies

```bash
npm install
```

---

### 4. Install Frontend Dependencies

```bash
cd client
npm install
```

---

### 5. Create Environment Variables

Create a `.env` file in the root directory and add:

```env
MONGO_URI=your_mongodb_connection_string
STRIPE_SECRET_KEY=your_stripe_secret_key
```

---

### 6. Run the Backend Server

```bash
npm start
```

---

### 7. Run the Frontend

Open another terminal:

```bash
cd client
npm start
```

---

## API Endpoints

### Bike Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/cars/getallcars` | Fetch all bikes |
| POST | `/api/cars/addcar` | Add a new bike |
| POST | `/api/cars/editcar` | Edit bike details |
| DELETE | `/api/cars/deletecar/:id` | Delete bike |

---

### Booking Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/bookings/bookcar` | Book a bike |
| GET | `/api/bookings/getallbookings` | Fetch all bookings |

---

## Database Models

### Bike Model
Stores:
- Bike name
- Image URL
- Fuel type
- Capacity
- Rent per hour
- Booked time slots

### Booking Model
Stores:
- User booking information
- Bike details
- Booking duration
- Transaction ID
- Payment information

---

## Security Improvements

- Stripe Secret Key moved to environment variables
- `.env` added to `.gitignore`
- Sensitive credentials hidden from GitHub

---

## Future Enhancements

- JWT Authentication
- Role-based Admin Access
- Booking Cancellation
- Email Notifications
- Bike Availability Filtering
- Deployment using Render/Vercel

---

## Author

Developed by Vikas Gowda

---

## License

This project is developed for educational and learning purposes.
