

# Full Stack Flask App Template with Firebase Integration

This template provides a robust starting point for building full-stack Flask applications with authentication and authorization capabilities powered by Google Firebase and Firestore. Designed to streamline the development process, this template includes pre-built functionalities such as user authentication (login, signup, password reset), session management, and CSRF protection, all optimized for mobile viewing.

## Features

- **Firebase Authentication Integration**: Supports login, signup, and forgot password functionalities.
- **Firestore Database Integration**: Easy setup to start using Firestore as your application database.
- **Secure Cookie Handling**: Client-side and server-side setup for secure cookie management.
- **Page Authorization**: Middleware setup for page-specific authorization to protect routes.
- **Responsive Design**: A basic responsive navbar and optimized interfaces for mobile and desktop viewing.
- **Pre-built Pages**: Pre-configured pages for authentication processes including login, signup, and password recovery.

## Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.8 or later
- pip (Python package installer)

## Getting Started

To get a local copy up and running follow these simple steps.

### 1. Clone the repository

git clone https://github.com/adjdunn/simple_firebase_app
cd flask-firebase-auth-template

### 2. Install dependencies

pip install -r requirements.txt

### 3. Configuration

#### Firebase Setup 
- Create Firebase account (https://firebase.google.com/)
- Go to the Firebase Console.
- Add a new project.
- Add web app to project.
- Go to "Project Settings" > Scroll to "SDK setup and configuration" > Select "Config" radio button and copy "firebaseConfig" data.
- Paste "firebaseConfig" data into firebase-config.js file.
- Paste "firebaseConfig" data into firebase-config.py file (adjust format to make it a valid python dict).
- Navigate to the "Firestore Database" section and create your database.
- Go to "Project Settings" > "Service accounts" > "Firebase Admin SDK" > Python option and click on the "Generate new private key" button Download the JSON file.
- Place the downloaded JSON file in your project directory and rename it to firebase_auth.json.
- Navigate to the "Authentication" section > click "Sign-in Method" and enable sign-in for Email/Password and Google options.
- Inside the "Autentication" section > click "Settings" > "Authorized Domains" and add your website domain to allow it to use the Google sign in (localhost is authorized by default).

#### Environment Variables
Create a .env file in the root directory of the project and add the following environment variables:

SECRET_KEY=your_secret_key_here


### 4. Run the application

python app.py

This will start the Flask application on http://localhost:5000 by default.

### 5. Customize the template to build your own app.



## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

Fork the Project
Create your Feature Branch (git checkout -b feature/AmazingFeature)
Commit your Changes (git commit -m 'Add some AmazingFeature')
Push to the Branch (git push origin feature/AmazingFeature)
Open a Pull Request

## License
Distributed under the MIT License. 

## Contact
Aaron Dunn - @your_twitter - wiresift@gmail.com

Project Link: https://github.com/yourusername/flask-firebase-auth-template

## Acknowledgements
Flask
Firebase






