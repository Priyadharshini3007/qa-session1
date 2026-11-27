# API Test Design

Endpoint

POST /api/login

Positive Scenario

Valid username and password return access token.

Negative Scenario

Invalid password returns authentication failure.

Boundary Scenario

Empty username and password return validation errors.

Assertions

- Status code validation
- Response body validation
- Error response validation

Reviewed:
Yes
