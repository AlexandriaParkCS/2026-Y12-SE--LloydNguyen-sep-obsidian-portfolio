**Login Process** The Login process is responsible for authenticating a user and establishing a session. It is initiated when a user submits the login form at `/login.html`.

At the top of the hierarchy is the `login()` function in `app.py`, which coordinates all submodules to validate input, retrieve the user, verify the password, and create the session.