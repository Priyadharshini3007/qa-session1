# Assertion Review

## Original Assertion

The login test used a weak assertion:

Expect(page).toContainText("Dashboard")

## Problem

This assertion only checks whether the word "Dashboard" appears on the page.

The test could pass even if:
- The wrong page is displayed.
- The dashboard is partially loaded.
- The text appears in an unexpected location.

## Improved Assertion

Expect(page.locator("[data-testid='dashboard-title']")).toHaveText("Dashboard")

## Benefits

- Verifies the correct dashboard element.
- Reduces false-positive test results.
- Ensures that the expected page is fully loaded.

## Result

The assertion now validates the actual application behavior more accurately.
