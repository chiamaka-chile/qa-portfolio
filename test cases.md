# Sauce Demo – Test Cases

**Application:** https://www.saucedemo.com
**Tested by:** Chiamaka Chile
**Environment:** Chrome browser
**Test Accounts Used:** `standard_user`, `problem_user`

---

| Test Case ID | Module | Test Case Description | Preconditions | Steps | Expected Result | Actual Result | Status | Notes |
|--------------|-----------------|------------------------------------------------------------|----------------------------------------|-----------------------------------------------------------------------|------------------------------------------------------|----------------------------------------------------|--------|--------------------------------|
| TC-001 | Login | Login with valid standard user | User is on login page | 1. Enter username: standard_user <br> 2. Enter password: secret_sauce <br> 3. Click Login | User is redirected to the inventory/products page | User successfully logged in and saw product list | Pass | |
| TC-002 | Login | Login with problem_user | User is on login page | 1. Enter username: problem_user <br> 2. Enter password: secret_sauce <br> 3. Click Login | User should be redirected to the inventory page | User logged in successfully | Pass | |
| TC-003 | Inventory | Verify product images load correctly (problem_user) | Logged in as problem_user | 1. Login as problem_user <br> 2. Observe the product images on the inventory page | All product images should display correctly | Several product images are broken / not loading | Fail | See Bug Report BR-001 |
| TC-004 | Inventory | Sort products by Name (A to Z) using problem_user | Logged in as problem_user | 1. Login as problem_user <br> 2. Click the sort dropdown <br> 3. Select "Name (A to Z)" | Products should be sorted alphabetically A–Z | Sorting did not work correctly | Fail | Products remained unsorted |
| TC-005 | Inventory | Sort products by Name (A to Z) using standard_user | Logged in as standard_user | 1. Login as standard_user <br> 2. Click the sort dropdown <br> 3. Select "Name (A to Z)" | Products should be sorted alphabetically A–Z | Products sorted correctly from A to Z | Pass | |
| TC-006 | Cart | Add a single product to cart | Logged in as standard_user | 1. Click “Add to cart” on any product <br> 2. Check the cart badge | Cart badge should show 1 | Cart badge correctly showed 1 | Pass | |
| TC-007 | Cart | Remove product from cart | Product already added to cart | 1. Click “Remove” on the product <br> 2. Check the cart badge | Cart badge should return to 0 or disappear | Product removed and badge updated correctly | Pass | |
| TC-008 | Checkout | Complete checkout with valid information | At least one item in cart | 1. Click cart icon <br> 2. Click Checkout <br> 3. Enter First Name, Last Name, Zip Code <br> 4. Click Continue <br> 5. Click Finish | Order confirmation page should appear | Order was successfully completed | Pass | |

---

**Summary**
- Total Test Cases Executed: 8
- Passed: 5
- Failed: 3
