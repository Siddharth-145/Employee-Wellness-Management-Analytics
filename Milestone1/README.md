# Employee Wellness Management Analytics - Milestone 1

## User Authentication Module using Streamlit

### Project Objective

The objective of this milestone is to develop a secure user authentication system for the Employee Wellness Management Analytics platform.

This module provides a complete authentication workflow that allows users to securely register, login, recover passwords, and access the wellness dashboard.

The system follows modern authentication practices by integrating password encryption, JWT based authentication, email OTP verification, and secure database management.

---

## Features Implemented

### Home Page
- Interactive Streamlit based user interface
- Employee Wellness Management Analytics landing page

### User Registration
- Collects user details:
  - Name
  - Email Address
  - Password
  - Confirm Password
- Validates user input
- Encrypts user passwords using bcrypt
- Stores user information securely in Neon PostgreSQL database
- Email verification using OTP

### User Login
- Authenticates users using email and password
- Generates JWT after successful authentication
- Maintains secure user sessions
- Redirects authenticated users to dashboard

### Forgot Password
- Verifies registered email address
- Generates secure OTP
- Sends OTP using Google SMTP service
- Validates entered OTP
- Allows password reset
- Updates encrypted password in database

### Dashboard
- Secure access after authentication
- Displays user information
- Allows employee wellness CSV file upload

---

## Technologies Used

- Python
- Streamlit
- Google Colaboratory
- Neon PostgreSQL
- JWT Authentication
- bcrypt Password Encryption
- Google SMTP
- pyngrok
- Pandas

---

## Database

Database Platform:

Neon PostgreSQL

Tables Created:

### users

Stores:
- User ID
- Username
- Email
- Encrypted password
- Verification status
- Created timestamp


### otp_codes

Stores:
- OTP code
- Email
- OTP purpose
- Expiry time
- Usage status

---

## Google Colab Setup Instructions

1. Open Authentication.ipynb in Google Colab

2. Install required dependencies

3. Add the following secrets in Google Colab:

```
DB_HOST
DB_PORT
DB_NAME
DB_USER
DB_PASSWORD
JWT_SECRET
SMTP_EMAIL
SMTP_APP_PASSWORD
NGROK_AUTHTOKEN

```

4. Execute all notebook cells.

5. Start the Streamlit application.

6. Open the generated ngrok public URL.

---

## Security Features

- Password hashing using bcrypt
- JWT based session handling
- OTP based verification
- Secure PostgreSQL connection
- Environment based secret management

---

## Milestone Status

Completed Successfully