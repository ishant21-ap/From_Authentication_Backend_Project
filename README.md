# User Registration and Authentication System

This project is a **User Registration and Authentication System** implemented using **Spring Boot** for the backend, **MongoDB** as the database, and **Postman** for testing the APIs. The system includes functionalities for user registration, OTP verification, login, password reset, and basic authentication.

---

## Features

1. **User Registration**:
   - User can register with email, name, mobile number, and password.
   - Password is encrypted using **BCryptPasswordEncoder** for security.
   - Email verification is done via OTP sent to the user's email address.

2. **User Login**:
   - Users can log in using their email and password.
   - Authentication is done using **BCryptPasswordEncoder** to match the password with the stored encrypted password.

3. **Forgot Password**:
   - Users can request to reset their password by providing their email.
   - An OTP is sent to the registered email address for verifying the user's identity.

4. **Reset Password**:
   - Users can reset their password by providing their email, OTP, and new password.
   - OTP verification ensures that the reset request is valid.

---

## Tech Stack

- **Backend**: Java, Spring Boot
- **Database**: MongoDB
- **Security**: Spring Security (for authentication and authorization)
- **Email**: **JavaMail API** for sending OTP emails
- **Password Encoding**: BCrypt for secure password storage
- **Validation**: Jakarta Validation (e.g., `@NotBlank`, `@Email`)
- **API Testing**: Postman

---
