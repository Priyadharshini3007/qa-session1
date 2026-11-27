**Prompt 1 - Requirement Ambiguity Analysis**
# Context

User Story:
As an HR Administrator, I want to add a new employee so that employee information can be managed in the system.

System:
OrangeHRM employee management module.

# Task

Review the requirement and identify ambiguities, assumptions and missing acceptance criteria.

# Requirements

- Identify functional ambiguities
- Highlight validation gaps
- Identify missing permission requirements
- Identify missing business rules

# Additional Info

Only HR Administrators should be allowed to create employee records.

**Prompt 2 - Test Case Generation****

# Context

User Story:
As an HR Administrator, I want to add a new employee so that employee information can be managed in the system.

System:
OrangeHRM employee management module.

# Task

Generate test cases in Given-When-Then format.

# Requirements

- Cover happy path scenarios
- Cover negative scenarios
- Cover boundary conditions
- Cover validation scenarios
- Cover authorization scenarios
- Assign priority as P0, P1 or P2

# Additional Info

Employee ID must be unique and mandatory fields should be validated.


**Prompt 3 - Traceability Matrix**

# Context

Requirement:
HR Administrator can create employee records.

Acceptance Criteria:
- Employee can be created successfully
- First Name and Last Name are mandatory
- Employee ID must be unique
- Success message should be displayed

# Task

Create a requirement-to-test traceability matrix.

# Requirements

- Map each acceptance criterion to corresponding test cases
- Ensure complete requirement coverage

# Additional Info

Format the output as a table.

**Prompt 4 - API Test Generation**

# Context

API Contract:

POST /api/employees

Body:
{
  "firstName": "string",
  "lastName": "string",
  "employeeId": "string"
}

# Task

Generate API test scenarios.

# Requirements

- Happy path testing
- Validation testing
- Authorization testing
- Duplicate employee ID testing
- Boundary testing

# Additional Info

Only authenticated HR Administrators can access the API.


**Prompt 5 - Test Data Generation**

# Context

Need employee records for employee creation testing.

# Task

Generate synthetic test data.

# Requirements

- Do not use real employee information
- Create unique employee IDs
- Provide realistic sample names

# Additional Info

Output should be privacy-safe and suitable for testing.
