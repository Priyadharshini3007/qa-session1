# Generated Test Cases

TC-01 Valid Login (P0)

Given a registered administrator account

When valid username and password are entered

Then the Dashboard should be displayed

----------------------------------------------------

TC-02 Invalid Password (P0)

Given a registered administrator account

When an invalid password is entered

Then an authentication error should be displayed

----------------------------------------------------

TC-03 Empty Username (P1)

Given the login page

When the username field is empty

Then login should be prevented

----------------------------------------------------

TC-04 Empty Password (P1)

Given the login page

When the password field is empty

Then login should be prevented

----------------------------------------------------

TC-05 Unauthorized Access (P1)

Given an unauthenticated user

When Dashboard URL is accessed directly

Then access should be denied

Approval

Approved: Yes
