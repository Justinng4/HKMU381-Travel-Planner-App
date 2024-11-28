# Travel Planner Web Application

## Group info: COMP S381F Group 8
  |     Student Name: <sub>`** for our group leader`</sub>  |   Student ID  |
  | :---: | :---: |
  | <sup>**</su> Ng Man Hei | 13505304      |  
  | Tse Man Hin   | 13515463      |
  | Wong Sin Ngai | 13588511      |
  | Pau Ka Lok    | 13068093      |
  | Leung Aidan   | 13626010      |

## Project file info: 
  ### Summary of functionalities of our web provided Server.js:
  
  1. User Authentication
      * Registration
      * Login
      * Log out
      * Profile Management
    
  3. Trip Management
      * Create Trips
      * Edit Trips
      * Delete Trips
      * View My Trips
      
  4. Contact Form
      * Contact us

  5. Budget Calculator

  6. Trip Planner

  7. Setting
      
  ### package.json Dependencies:
  
    "bcrypt": "^5.1.1",
    "bcryptjs": "^2.4.3",
    "bootstrap": "^5.3.2",
    "connect-flash": "^0.1.1",
    "cookie-session": "^2.0.0",
    "dotenv": "^16.4.5",
    "ejs": "^3.1.10",
    "express": "^4.21.1",
    "express-ejs-layouts": "^2.5.1",
    "express-session": "^1.18.1",
    "font-awesome": "^4.7.0",
    "mongodb": "^6.3.0",
    "mongoose": "^8.8.2",
    "passport": "^0.6.0",
    "passport-facebook": "^3.0.0",
    "passport-instagram": "^1.0.0",
    "passport-local": "^1.0.0",
    "path": "^0.12.7"

  ### public

  ### views
# Views Folder Structure

  ### Routes
## User Management API

This project provides a RESTful API for managing `User` resources using **Express.js** and **MongoDB**. It supports basic CRUD operations and uses **Mongoose** for database interactions.

---
## **Description**

This API allows you to:

1. **Get all users**: Fetch all users in the database.
2. **Get a specific user by ID**: Retrieve details of a specific user using their unique identifier.
3. **Create a new user**: Add a new user to the database with fields like `name`, `email`, and `password`.
4. **Update an existing user**: Modify specific fields of an existing user.
5. **Delete a user**: Remove a user from the database by their ID.

The API also includes middleware (`getUser`) to fetch and validate a user for PATCH and DELETE operations.

---

## **Features**

- **GET `/users`**: Fetch all users.
- **GET `/users/:id`**: Retrieve a user by their unique ID.
- **POST `/users`**: Create a new user with name, email, and password.
- **PATCH `/users/:id`**: Update specific fields of a user (e.g., name, email, or password).
- **DELETE `/users/:id`**: Delete a user by their ID.

## Subfolders

### `admin/`
- **`contacts.ejs`**  
  Displays the list of user inquiries or contact requests.

### `partials/`
- **`footer.ejs`**  
  Defines the footer layout shared across multiple pages.
- **`header.ejs`**  
  Defines the header layout with navigation and branding.
- **`messages.ejs`**  
  Displays flash messages for user feedback (e.g., errors or success).

### `trips/`
- **`edit.ejs`**  
  A form to edit an existing trip's details.
- **`new.ejs`**  
  A form to create a new trip.

## Main `.ejs` Files
- **`about.ejs`**  
  Provides information about the application or company.
- **`add-trip.ejs`**  
  A form to add a new trip.
- **`budget-calculator.ejs`**  
  A tool for users to calculate trip budgets.
- **`contact.ejs`**  
  A page with a contact form for user inquiries.
- **`dashboard.ejs`**  
  Displays an overview of the user's activities or stats.
- **`footer.ejs`**  
  (Used in `partials/`) Shared footer for all pages.
- **`header.ejs`**  
  (Used in `partials/`) Shared header for all pages.
- **`index.ejs`**  
  The main landing page of the application.
- **`layout.ejs`**  
  The base layout template wrapping individual pages.
- **`login.ejs`**  
  A login form for user authentication.
- **`my-trips.ejs`**  
  Displays a list of trips created by the user.
- **`profile.ejs`**  
  Displays and edits user profile details.
- **`register.ejs`**  
  A form for user registration.
- **`setting.ejs`**  
  Manages user-specific settings or preferences.
- **`settings.ejs`**  
  Handles application-wide settings or configurations.
- **`trip-planner.ejs`**  
  Provides a form or interface for planning trips.
- **`trips.ejs`**  
  Displays a list of trips available to explore.
- **`updateProfile.ejs`**  
  A form to update user profile information.

  ### models
For models file , we have "Contact.js ", "Trip.js " , "User.js " in JavaScript file .

## Cloud-based server URL: 
https://hkmu381-travel-planner-app.onrender.com

## Operation guides
> Operation guides (like a user flow) for your server.
**'the use of Login logout pages'**

 User can go to the register site to make their own account,
 then will jump to the login page and then can login, and for the logout pages is the profile page, in there you can update you profile or you can logout the account.

1. Installation guideline
2. Open Visual Studio Code
3. Create .env file
4. Copy the code in env sample and modify the "SESSION SECRET" and "MONGODB_URL"
5. Makesure u install nodejs
6. Download npm install, "npm run dev"
7.  Terminal will display: 
   
|       Message          |
|-----------------------------------------|
| server is running on port 3001          |
| Connected to MongoDB                    |
| MongoDB Atlas Connected                 |
| Database ping Check Connection successful |


After go in the web:
-> Home
register
login

CRUD:
Dashboard
add new trip
enter destination
start date
end date
desciption
create trip

provide function
edit
delete
add new trip


- the use of Login/Logout pages: a list of valid login information, sign in steps? …
- the use of your CRUD web pages: which button or UI is used to implement create, read, update, and delete?
- the use your RESTful CRUD services: the lists of APIs? HTTP request types? Path URI? How to test them?
CURL testing commands?
Notes:
- `README.md` is important to let me know your project functions, which is crucial to marking the grade of
your project.
