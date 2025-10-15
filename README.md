# Ambucall - Ambulance Booking Web App

Ambucall is a web application for booking ambulances, tracking bookings, and providing emergency support. It features user and driver authentication, Google and email sign-in, Firestore integration, and real-time location tracking.

## Features
- User sign-in via Google or email
- Driver/staff sign-in and registration
- Ambulance booking form with location support
- Firestore database for storing user and booking details
- Driver dashboard for managing bookings
- Real-time ambulance tracking
- Emergency first aid resources

## Technologies Used
- HTML, CSS, JavaScript (ES6 modules)
- Firebase (Auth, Firestore, Analytics)
- Leaflet.js for maps
- Google OAuth for authentication

## Project Structure
```
ambucall-main/
├── assets/                  # Static assets (images, policies)
├── booking.html             # Ambulance booking page
├── booking-details.html     # Booking details and map
├── booking_style.css        # Booking page styles
├── driver-dashboard.html    # Driver dashboard
├── driver-login.js          # Driver login logic
├── driver-signin.html       # Driver sign-in page
├── driver-signup.html       # Driver sign-up page
├── driver-register.js       # Driver registration logic
├── driver-navigation.html   # Driver navigation and tracking
├── email-signin.html        # User email sign-in page
├── email-signup.html        # User email sign-up page
├── emergency.html           # Emergency ambulance/hospital list
├── firstaid.html            # First aid resources
├── googlelogin.js           # Google sign-in logic
├── hospital-login.html      # Hospital/staff login page
├── index.html               # Landing page
├── login.js                 # User login logic
├── register.js              # User registration logic
├── results.html             # Booking results and map
├── signin_style.css         # Sign-in page styles
├── styles.css               # Global styles
├── track-by-booking-id.html # Track ambulance by booking ID
├── user-login.html          # User login page
```

## Setup Instructions
1. Clone the repository or copy the project files.
2. Set up a Firebase project:
   - Enable Authentication (Email/Password, Google)
   - Add your domain (localhost, 127.0.0.1) to Authorized Domains
   - Create Firestore database
   - Update Firebase config in all JS files with your project credentials
3. Serve the project locally (e.g., with Live Server or Python's http.server).
4. Open `index.html` or `user-login.html` in your browser.

## Usage
- Users can sign in with Google or email, book ambulances, and track bookings.
- Drivers/staff can sign in, view bookings, and update booking status.
- Location features use browser geolocation and Leaflet maps.

## Troubleshooting
- If Google sign-in fails with "auth/unauthorized-domain", check Firebase Console > Authentication > Authorized domains.
- Ensure Firebase config matches your project.
- For Firestore access issues, update security rules to allow authenticated reads/writes.

## License
This project is for educational/demo purposes. Please update and secure before production use.
