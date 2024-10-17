---
title: User Stories!
---

# Epic: User Authentication System (Login and Registration)

### Objective:

Build a secure and functional user authentication system that allows users to register, verify their account, and log in to the platform, while ensuring database integrity and secure data handling.

---

## Stories:

### Story 1: **User Registration**

**As a user, I want to register an account with my email and password so that I can create a unique account and access the platform.**

#### Acceptance Criteria:

1. **Email Input Validation**:

   - The system must accept only valid email formats.
   - Invalid email addresses should trigger error messages (e.g., "Please enter a valid email address.").
   - **Quantifiable:** 95%+ accuracy for detecting invalid emails.

2. **Password Requirements**:

   - Password must be at least 8 characters long.
   - Must include at least one uppercase letter, one number, and one special character.
   - **Quantifiable:** 100% compliance with password policy.

3. **Database Interaction**:

   - Ensure that a unique user record is created in the database for each registration.
   - If the email is already taken, return an error (e.g., "This email is already registered.").
   - **Quantifiable:** Unique email enforced at database level (no duplicates).

4. **Success Notification**:

   - After successful registration, display a confirmation message (e.g., "Registration successful. Please check your email to verify your account.").
   - **Quantifiable:** Email verification link sent within 2 seconds of registration.

5. **Email Verification**:
   - System should send a verification email with a unique link. The link must expire after 24 hours.
   - **Quantifiable:** 99%+ success rate of email delivery.

---

### Story 2: **User Login**

**As Joey, I want to log in to my account using my registered email and password so that I can access the system securely.**

#### Acceptance Criteria:

1. **Login Validation**:

   - Email and password must be validated against the database.
   - If incorrect credentials are entered, display an error (e.g., "Invalid login credentials.").
   - **Quantifiable:** 99%+ match rate for correct credentials.

2. **Password Encryption**:

   - Ensure that all passwords are stored as hashed and salted values in the database.
   - **Quantifiable:** 100% of passwords stored encrypted.

3. **Session Handling**:

   - Upon successful login, create a session token (JWT) valid for 1 hour.
   - If "Remember me" is selected, extend the session validity to 7 days.
   - **Quantifiable:** 95%+ session stability without invalid tokens.

4. **Rate Limiting**:

   - Lock the account after 5 failed login attempts within a 10-minute period.
   - Account unlock link is sent via email.
   - **Quantifiable:** 100% compliance with the lockout policy.

5. **Database Interaction**:
   - User credentials should be retrieved securely from the database, with no plaintext passwords.
   - **Quantifiable:** Zero incidents of plaintext password storage.

---

### Story 3: **Password Reset**

**As a user, I want to reset my password if I forget it so that I can regain access to my account without contacting support.**

#### Acceptance Criteria:

1. **Forgot Password Link**:

   - Display a "Forgot password?" link that redirects to a password reset request page.
   - **Quantifiable:** 100% visibility and function of the link.

2. **Email Verification for Reset**:

   - Users must enter their registered email to receive a password reset link.
   - **Quantifiable:** 99%+ success rate of password reset emails.

3. **Reset Link Expiration**:

   - Password reset link should expire after 1 hour.
   - **Quantifiable:** Expiration mechanism should work 100% of the time.

4. **Password Reset Page**:
   - Users should be able to create a new password following the password policy (min. 8 characters, special characters, etc.).
   - **Quantifiable:** 100% compliance with the password policy during reset.

---

## Initiative:

## This epic is part of a larger initiative to provide secure user management features, including login, registration, and password management, to enhance the user experience and platform security.
