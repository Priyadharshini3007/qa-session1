# Test Cases

TC-01 Valid Login (P0)

Given valid credentials
When user logs in
Then Dashboard should load

TC-02 Invalid Password (P0)

Given valid username
When invalid password is entered
Then error message should appear

TC-03 Empty Username (P1)

Given login page
When username is empty
Then login should be blocked

TC-04 Empty Password (P1)

Given login page
When password is empty
Then login should be blocked

TC-05 Unauthorized Access (P0)

Given user is not authenticated
When Dashboard URL is accessed
Then access should be denied

Reviewed:
Yes
