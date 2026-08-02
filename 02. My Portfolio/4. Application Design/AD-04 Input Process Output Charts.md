**Login/Register**

The Login/Register process is a critical component of the application, enabling secure access and personalised student experiences. This process allows new students to create accounts and existing users to authenticate their credentials to access their progress and scenarios.

**Summary of a user login:**

Input
- Username or email address
- Password (plain text)

Process
- Sanitise and validate the username/email and password
- Calculate a password hash
- Check for an existing user using the username or email address
- If it exists, retrieve the stored password hash, otherwise reject the login
- Compare the stored and calculated password hashes
- If the password hashes match, initialise a user session
- Otherwise, allow entry of another password (up to 3 attempts), or prevent login attempts for 5 minutes (after 3 attempts)

Output
- Success message and redirect to student dashboard
- Error message, if required
- Authentication session token

**Summary of user registration:**
Input
- Full name
- Email address
- Password (plain text)

Process
- Sanitise and validate the full name, email address, and password
- Check whether an account already exists with the provided email address
- If an account exists, return an error prompting the user to log in instead
- Otherwise, calculate a password hash from the plain text password
- Store the new user's details and hashed password in the database
- Initialise a new user session upon successful registration

Output
- Success message and redirect to student dashboard
- Error message, if required
- Authentication session token