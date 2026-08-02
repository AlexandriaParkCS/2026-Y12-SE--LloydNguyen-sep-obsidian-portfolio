**Sign Up** The Sign Up process allows new users to create an account. It is a critical entry point that ensures only valid, unique users are stored in the database.

Input
- Name (text)
- Username (text)
- Email address (valid email format)
- Password (plain text, minimum 8 characters)

Process
- Validate all fields are non-empty
- Check password length ≥ 8 characters
- Check password matches confirm password
- Call `sqldb.create_user(username, email, password)`
    - Hash password using `werkzeug.security.generate_password_hash()`
    - Execute `INSERT INTO users (username, email, password) VALUES (?, ?, ?)`
    - If IntegrityError, username or email already exists → return None
- If user created successfully, flash success message and redirect to login
- If creation failed, return error message to sign-up template

Output
- Success: redirect to `/login.html` with flash message "Account created! Please log in."
- Failure: error message displayed on sign-up form (e.g. "That username or email is already taken.")

