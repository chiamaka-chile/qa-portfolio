# Bug Report – BR-001

**Title:** Product images fail to load when logged in as problem_user

**Severity:** Medium
**Priority:** Medium
**Environment:** Chrome browser
**URL:** https://www.saucedemo.com
**Account Used:** problem_user / secret_sauce
**Reported by:** Chiamaka Chile
**Date:** November 2026

---

### Description
When logging in with the `problem_user` account, several product images on the inventory page do not load correctly. Broken image icons or incorrect images are displayed instead of the actual product photos.

### Steps to Reproduce
1. Go to https://www.saucedemo.com
2. Enter username: `problem_user`
3. Enter password: `secret_sauce`
4. Click the **Login** button
5. Observe the product images on the inventory page

### Expected Result
All product images should load and display correctly (same behavior as when using `standard_user`).

### Actual Result
Multiple product images appear broken or fail to load properly.

### Additional Notes
- This issue does **not** occur when using the `standard_user` account.
- The rest of the page (product names, prices, and Add to Cart buttons) still loads.
- This appears to be an intentional issue on the Sauce Demo site for the `problem_user` account, but it is still a valid defect from a user experience perspective.

