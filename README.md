# Ami Coding Pari Na, An Django Authentication and Search App

This is a Django-based web application that provides user authentication and a search feature using Django Rest Framework. Users can register, log in, change their passwords, and reset forgotten passwords. In addition, the application allows users to input values, store them in a sorted order in the database, and perform searches on those values.

## Features

- User Registration: Users can register by providing their email, name, and password. Passwords are securely hashed and stored in the database.

- User Login: Registered users can log in using their email and password.

- User Profile: Authenticated users can view their profile information, including email and name.

- Change Password: Logged-in users can change their passwords by providing the current password and the new password.

- Password Reset: Users who forget their passwords can request a password reset. A password reset link is sent to the user's email, allowing them to create a new password.

- Storing Input Values: Users can input comma-separated integers, and the application stores the values in the database in descending order along with the user's ID and input timestamp.

- Khoj the Search: Users can enter a search value, and the application will determine if the search value exists in the stored input values. It returns "True" if found, and "False" if not found.

- API Endpoints: The application provides API endpoints for retrieving input values within a specified time range for a user.

## Installation

1. Clone the repository: `git clone https://github.com/mohidulislam23/Ami-Coding-Pari-Na`
2. Navigate to the project directory: `cd source`
3. Install the required packages: `pip install -r requirements.txt`
4. Set up your environment variables for email configuration (`EMAIL_USER` and `EMAIL_PASS`).
5. Apply database migrations: `python manage.py migrate`
6. Start the development server: `python manage.py runserver`

## Usage

1. Register a new user by visiting `/register/`.
2. Log in with your registered credentials at `/login/`.
3. View your profile at `/profile/`.
4. Change your password at `/changepassword/`.
5. Request a password reset link at `/send-reset-password-email/`.
6. Use the password reset link received in your email to reset your password at `/reset-password/<uid>/<token>/`.
7. Input values and store them in the database at `/store-input-values/`.
8. Perform a search using the "Khoj the search" feature at `/khoj-search/`.
9. Retrieve stored input values via API at `/get-input-values/`.

## API Endpoints

- `/get-input-values/`: Retrieve stored input values within a specified time range for a user.

## Contributors

- [Mohidul Islam](https://github.com/mohidulislam23)


---

Feel free to contribute to this project by creating pull requests or opening issues. Happy coding!