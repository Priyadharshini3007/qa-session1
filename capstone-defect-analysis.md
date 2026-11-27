# Defect Analysis

Feature:
OrangeHRM Login

Defect ID:
BUG-001

Issue:
Intermittent login failure observed during negative test execution.

Reproduction Steps

1. Open login page.
2. Enter invalid credentials.
3. Click Login.
4. Verify error message.

Observed Result

Error message occasionally does not appear before validation executes.

Expected Result

Authentication error should consistently display.

Evidence

Execution logs showed delayed UI rendering.

Severity

Medium

Status

Analysed
