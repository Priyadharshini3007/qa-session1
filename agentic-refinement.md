# Refinement

Original Validation

expect(errorMessage).toBeVisible();

Improved Validation

await expect(errorMessage)
.toBeVisible({ timeout: 5000 });

Additional Improvements

- Removed fixed waits
- Used explicit element waits
- Reviewed selectors for stability
- Confirmed no hardcoded credentials

Verification

Test executed successfully 10 consecutive times.

Result

Flaky behaviour no longer observed.

Approval

Approved: Yes
