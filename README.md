# Smart Parking Web App

A Flask-based full-stack web application for real-time parking slot booking with PayPal integration.

## ⚙️ Features

- **Real-time Parking Slot Booking**: Reserve parking slots with date/time selection
- **Multi-user System**: Separate interfaces for customers, managers, and administrators
- **PayPal Payment Integration**: Secure payment processing
- **Location-based Parking**: Multiple parking locations with different pricing
- **Session Management**: Secure user authentication and session handling
- **SQLite Database**: Efficient data storage for users, bookings, and transactions
- **Responsive UI**: Clean and user-friendly interface

## 🧠 Tech Stack

| Area | Technologies Used |
|------|-------------------|
| **Frontend** | HTML, CSS, JavaScript, Bootstrap |
| **Backend** | Python, Flask |
| **Database** | SQLite |
| **Payment** | PayPal REST SDK |
| **Authentication** | Flask Sessions |
| **Version Control** | Git + GitHub |

## 📦 Installation & Setup

### Prerequisites
- Python 3.7+
- pip (Python package manager)

### Installation Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/adhwaith43/Smart-Parking-WebApp.git
   cd Smart-Parking-WebApp
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the database**:
   - The app uses SQLite database
   - Make sure your database file is properly configured in `app.py`

4. **Run the application**:
   ```bash
   python app.py
   ```

5. **Access the application**:
   Open your browser and navigate to:
   ```
   http://localhost:5000
   ```

## 👥 User Roles & Access

### 🎯 Customer
- **Register/Login**: User registration and authentication
- **Book Parking**: Select location, date/time, and make payments
- **View Bookings**: Access booking history and details

### 👨‍💼 Manager  
- **Dashboard**: View bookings for specific locations
- **Location Management**: Monitor slot availability and bookings
- **Login**: `muser@example.com` / `password2` (Day location)
- **Login**: `m2user@example.com` / `password` (Dawn location)

### 👨‍💻 Administrator
- **Admin Portal**: Overall system management
- **View All Bookings**: Access to all booking records
- **Login**: `admin@example.com` / `adminpassword`

## 📁 Project Structure

```
Smart-Parking-WebApp/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── static/
│   ├── style.css         # Main stylesheet
│   └── script.js         # Client-side JavaScript
├── templates/
│   ├── index.html        # Landing page
│   ├── user.html         # User dashboard
│   ├── user login.html   # User login page
│   ├── user register.html # User registration
│   ├── adminportal.html  # Admin dashboard
│   ├── manager dashboard.html # Manager interface
│   ├── payment.html      # Payment processing
│   ├── payment_success.html # Payment confirmation
│   └── ... (other templates)
└── README.md             # Project documentation
```

## 🔄 Key Routes

- `/` - Home page
- `/map` - User parking location selection
- `/login` - User authentication  
- `/register` - User registration
- `/payment` - Payment processing
- `/adminLogin` - Administrator access
- `/loginM` - Manager login
- `/booking_info_day` - Day location bookings
- `/booking_info_dawn` - Dawn location bookings

## 💳 Payment Integration

- **Sandbox Mode**: Currently configured for PayPal sandbox testing
- **Secure Transactions**: Payment verification and status tracking
- **Booking Confirmation**: Automatic booking confirmation upon successful payment

## 🗄 Database Schema

Main tables include:
- `user` - Customer accounts
- `manager` - Manager accounts  
- `booking` - Booking records
- `Location` - Parking location details
- `transaction1` - Payment transactions
- `user_session` - Active user sessions

## 📌 Project Roadmap

| Feature | Status |
|---------|--------|
| Basic booking system | ✅ Completed |
| User authentication | ✅ Completed |
| PayPal integration | ✅ Completed |
| Multi-role access | ✅ Completed |
| UI/UX Enhancement | ⏳ In Progress |
| Email notifications | 🔜 Planned |
| Advanced analytics | 🔜 Planned |
| Mobile app | 🔜 Planned |

## 🏗️ Current Status

**⚠️ Work in Progress - MVP Stage** 
- Core functionality is implemented and working
- PayPal integration in sandbox mode
- Basic UI implemented
- Regular updates and improvements being made

## 🚨 Important Notes

- This is a **development version** for portfolio demonstration
- PayPal is configured in **sandbox mode** for testing
- Database file should be properly initialized with required tables
- Secret keys should be environment variables in production

## 👤 Developer

**Adhwaith A M**  
📍 Kerala, India  
📧 Email: adhwaith43@gmail.com  
🔗 LinkedIn: [linkedin.com/in/adhwaith-a-m-7408a8314](https://www.linkedin.com/in/adhwaith-a-m-7408a8314)  
🐙 GitHub: [github.com/adhwaith43](https://github.com/adhwaith43)

---

*This project demonstrates full-stack web development capabilities with Flask, database management, and third-party API integration.*