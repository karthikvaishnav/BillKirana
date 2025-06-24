BillKirana 🛒

From Store to Screen, Effortless Management!
Welcome to BillKirana, a web app to digitize small and medium grocery stores across India, inspired by my dad’s kirana shop. As my first major web development project, I’m taking on a 10-day challenge to build a platform that empowers shop owners to manage inventory and customers to shop seamlessly—all with a few clicks! Built with HTML, CSS, JavaScript, and Firebase, this is a work-in-progress with non-clean, non-responsive code (bear with me, I’m learning!). Join me in this journey to modernize local kiranas! 🚀
Motivation
Growing up, I watched my dad manage his grocery store manually—tracking inventory, billing customers, and juggling records. This sparked the idea for BillKirana: a digital solution to streamline operations for small and medium kirana shops and enhance the shopping experience for customers. My goal is to empower local businesses to thrive in a digital world, one store at a time.
Features
Completed (Day 1-3)

Landing Page: Sleek UI with a catchy slogan and toggle for owner/customer views.
Email & Phone Authentication: Firebase-powered signup/login for owners and customers using email/password or phone number (OTP).
Role-Based Dashboards: Redirects to owner-dashboard.html or customer-dashboard.html based on user role stored in Firestore.
Password Toggle: Show/hide password with eye icon for secure input.
Remember Me: Persists login sessions across browser restarts.
Logout: Sign out from dashboards with redirect to login page.

Planned (Day 4-10)

Forgot Password: Reset password via email or SMS.
Owner Dashboard: Inventory management (add/edit items, track name, quantity, price).
Customer Features: Browse products, place orders, view order history.
UI Polish: Make the app responsive and refine code for production.
Security: Tighten Firestore rules and add input validation.

Tech Stack

Frontend: HTML, CSS (Inter font, Login.css), JavaScript
Backend: Firebase Authentication (email, phone), Firestore
Assets: mainimage.jpeg, Designer.jpeg, eye.png, eye-slash.png
Tools: VS Code, Live Server

Setup

Clone the Repository:git clone https://github.com/yourusername/BillKirana.git
cd BillKirana


Firebase Setup:
Create a Firebase project at console.firebase.google.com.
Enable Email/Password and Phone authentication.
Add your Firebase config to firebase.js.
Update Firestore rules:rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /users/{userId} {
      allow read: if true;
      allow write: if request.auth != null;
    }
  }
}




Install Dependencies:
Ensure eye.png, eye-slash.png, mainimage.jpeg, Designer.jpeg are in the project folder.
No additional packages needed (uses Firebase CDN).


Run Locally:
Open with VS Code’s Live Server (http://localhost:5500/Login.html).



Usage

Sign Up: Go to signup.html, choose owner/customer, enter name, email/phone, and password. For phone, verify OTP.
Login: Use Login.html with email/phone and password (or OTP). Check “Remember Me” for persistent sessions.
Dashboards: Owners see owner-dashboard.html, customers see customer-dashboard.html. Logout redirects to Login.html.
Password Toggle: Click the eye icon to show/hide passwords.

Project Status
This is my first major web dev project, so the code isn’t fully clean or responsive yet. I’m iterating daily in this 10-day challenge to add features and polish the app. Current files:

Login.html: Login page with email/phone auth and toggle.
signup.html: Signup page with role selection.
customer-dashboard.html, owner-dashboard.html: Basic dashboards with logout.
firebase.js: Firebase config and auth/firestore imports.
Login.css: Styles for UI and toggle.

Contributing
I’d love your feedback to make BillKirana better! 🙌 Feel free to:

Open issues for bugs or suggestions.
Submit pull requests for improvements.
Share ideas for features like inventory management or customer ordering.

Check my daily progress on LinkedIn and star this repo to follow the journey!
License
MIT License - feel free to use and contribute!
Contact
Connect with me on LinkedIn or email me at [your.email@example.com]. Let’s digitize kirana stores together! 🛒

Built with ❤️ for local kiranas
