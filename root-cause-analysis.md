# Root Cause Analysis

## Observed Behavior

The login test intermittently fails even though valid credentials are entered.

## Evidence

Application logs indicate that the authentication response is occasionally delayed.

Example Log:

Authentication service response exceeded the expected response time.

## Root Cause

A race condition exists between the login request completion and dashboard validation. The test attempts to verify dashboard elements before the authentication process has fully completed.

## Fix Applied

Replaced the fixed wait with an explicit wait for dashboard visibility after successful authentication.

## Verification

Executed the login test multiple times after the fix and did not observe any failures.
