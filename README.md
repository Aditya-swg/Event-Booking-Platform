#Full-Stack Event Booking Platform

Developed a full-stack event booking platform using the MERN stack that enables users to browse events, request ticket bookings, and
securely confirm reservations through OTP verification. Implemented JWT-based authentication with bcrypt password hashing and rolebased access control for Admin and User functionalities. The platform includes event management features for creating events and
smart booking system with seat availability validation. Integrated an admin analytics dashboard to monitor booking requests, revenue,
and confirmed clients. Automated email notifications for account verification and booking confirmations using Nodemailer.


## Features
- **User Authentication**: Secure login & registration with JWT and bcrypt.
- **2FA OTP Verification**: 
  - Mandatory Email OTP to activate your account upon Registration (or delayed login attempts).
  - Mandatory Email OTP to finalize and secure event ticket booking.
- **Role-Based Access**: 
  - **Admin**: Create, edit, and delete events. Confirm and reject all incoming booking requests, mark them as 'Paid' or 'Not Paid'. Access is strictly locked to database-flagged users only.
  - **User**: Browse events, submit ticket booking requests via OTP, view personal dashboard pending status, and cancel bookings.
- **Event Management**: Create free and paid events with detailed descriptions, external image URLs, dates, categories, and seating capacity.
- **Smart Booking System**:
  - Mandatory 2FA OTP to authorize a booking request.
  - All booking requests (both free and paid) enter a secure 'Pending' queue for Admin verification.
  - Seat availability accurately updates and securely validates against overbooking logic.
- **Admin Analytics Dashboard**: Track live data such as Pending Requests, Total Revenue, and Total Confirmed Paid Clients directly from the admin panel.
- **Email Notifications**: Automated email delivery upon successful booking confirmation using Nodemailer.

---
