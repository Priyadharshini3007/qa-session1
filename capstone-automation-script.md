# Automation Test Example

Framework:
Playwright

Example

test("successful login", async ({ page }) => {

await page.goto("/login");

await page.locator("[data-testid='username']")
.fill("Admin");

await page.locator("[data-testid='password']")
.fill("admin123");

await page.locator("[data-testid='login-button']")
.click();

await expect(
page.locator("[data-testid='dashboard']")
).toBeVisible();

});

Automation Review

- Uses data-testid selectors
- No hardcoded sleeps
- Explicit validation included

Reviewed:
Yes
