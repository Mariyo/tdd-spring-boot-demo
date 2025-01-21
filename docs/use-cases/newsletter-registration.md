# Use Case: Newsletter Registration

## Goal
Allow users to register for a newsletter.

## Actors
- User

## Preconditions
- User is on the newsletter registration page.

## Main Success Scenario
1. User navigates to the newsletter registration page.
2. User enters their email address.
3. User submits the registration form.
4. System validates the email address.
5. System saves the email address to the database.
6. System sends a confirmation email to the user.
7. System displays a success message to the user.

## Extensions
- 4a. Invalid email address:
  - 1. System displays an error message indicating the email address is invalid.
- 5a. Email address already registered:
  - 1. System displays a message indicating the email address is already registered.

## Postconditions
- The user's email address is saved in the database.
- The user receives a confirmation email.

## Notes
- The confirmation email should contain a link to unsubscribe.
