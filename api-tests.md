API Endpoint

POST /api/employees

Happy Path

Scenario:
Create employee with valid data

Expected:
201 Created

------------------------------------------------

Validation Tests

Scenario:
Missing first name

Expected:
400 Bad Request

Scenario:
Missing last name

Expected:
400 Bad Request

Scenario:
Duplicate Employee ID

Expected:
409 Conflict

------------------------------------------------

Authorization Tests

Scenario:
Without token

Expected:
401 Unauthorized

Scenario:
Invalid token

Expected:
401 Unauthorized

Scenario:
Non-HR user

Expected:
403 Forbidden

------------------------------------------------

Boundary Tests

Scenario:
Maximum name length

Expected:
Employee created successfully

Scenario:
Special characters in Employee ID

Expected:
Validation error
