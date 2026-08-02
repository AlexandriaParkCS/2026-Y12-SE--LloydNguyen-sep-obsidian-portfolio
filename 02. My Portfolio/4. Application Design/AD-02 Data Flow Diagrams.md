**Context Diagram** The application interacts with a number of external entities (actors) as shown on the following Context Diagram.

The actors include:

- **User**: a person who registers, logs in, and interacts with the orders, message, artworks. 
- **SQLite DB**: the application uses an SQLite3 database (sql.db) to store user accounts and service requests.

**Level 1 Data Flow Diagram** The following diagram shows the top level structure of the application.

Users must register via the Sign Up process before they can log in. During sign up, the user provides a name, username, email, and password. The password is hashed before being stored in the users table.

Once registered, users log in by providing their email and password. The application retrieves the user record from the database, verifies the password hash, and if successful, stores the user's ID and username in a Flask session (D2).

The Home Page process checks the Flask session to determine whether the user is logged in. If not, the user is redirected to the login page. If logged in, the user's username is displayed and they can access the Send Request page.

The upload artwork process also checks the session. Only logged-in artist users can upload.
