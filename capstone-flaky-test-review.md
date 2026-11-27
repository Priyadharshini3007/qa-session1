# Flaky Test Review

Problem

Intermittent failure during login validation.

Cause

Timing dependency.

Improvements

- Added explicit waits
- Removed reliance on timing assumptions
- Improved assertion reliability

Outcome

Flaky behaviour eliminated during repeated execution.

Status

Stabilized
