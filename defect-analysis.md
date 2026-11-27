# Defect Analysis

## Issue

Users occasionally experience login failures despite entering valid credentials.

## Steps to Reproduce

1. Navigate to the OrangeHRM login page.
2. Enter valid username and password.
3. Click Login.
4. Repeat the login process multiple times.

## Expected Result

The user should be redirected to the Dashboard after successful authentication.

## Actual Result

The login test intermittently fails even when valid credentials are supplied.

## Log Evidence

Authentication response is delayed intermittently.

Example:

Authentication request timeout after 5 seconds.

## Impact

Login validation becomes unreliable and causes intermittent test failures.
