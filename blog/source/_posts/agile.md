---
title: Agile Notes
---

## Initiative:

I want to be able to successfully register and login to this site with feedback.

## Epic 1: User Authentication

Enable users to register and login with confirmation and error feedback.

### User Story 1: Registration

**Description**: As a user, I want to enter my details (email, password) to register quickly.

**Acceptance Criteria**:

- User can enter an email and password.
- User clicks the register button to submit the form.
- Registration is successful when valid details are entered.

### User Story 2: Registration

**Description**: As a user, I want a confirmation message after registration to know it worked.

**Acceptance Criteria**:

- After successful registration, a confirmation message appears (e.g., “Registration successful!”).
- Confirmation message is clear and visible on the screen.

### User Story 3: Registration

**Description**: As a user, I want to see error messages if registration fails, so I know what to fix.

**Acceptance Criteria**:

- If the email format is invalid, an error message appears (e.g., “Invalid email format”).
- If the password doesn’t meet requirements, an error message appears (e.g., “Password must be 8+ characters”).
- Error messages appear in real-time and guide users to correct inputs.

### User Story 1: Login

**Description**: As a user, I want to enter my credentials (email, password) to log in easily.

**Acceptance Criteria**:

- User can enter a registered email and password.
- User clicks the login button to submit.
- Login is successful when correct credentials are provided.

### User Story 2: Login

**Description**: As a user, I want feedback (success/error) when logging in to know if it worked.

**Acceptance Criteria**:

- If login is successful, a success message appears (e.g., “Welcome back!”).
- If login fails (wrong password/username), an error message appears (e.g., “Incorrect credentials, please try again”).
- Error message guides the user on what went wrong.
