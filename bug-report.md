# Bug Report

## Test Environment

- URL: https://www.saucedemo.com
- Browser: Mozilla Firefox
- Device: Laptop

---

## BUG-001 - Unclear Error Message for Invalid Login Credentials

### Related Test Case 
TC-002 - Invalid password

### Summary
Error message does not clearly indicate whether the issue is with the username or the password

### Steps to Reproduce:
1. Navigate to https://www.saucedemo.com
2. Enter valid username (e.g., standard_user)
3. Enter incorrect password
4. Click login

### Actual Result
Message displayed:
"Epic sadface: Username and password do not match any user in this service"

### Expected Result
A clearer message indicating the exact issue (e.g., incorrect password)

### Severity 
Low

### Priority 
Low

### Status
Open

### Notes
This may confuse users and make troubleshooting harder.

---

## BUG-002 - Password field lacks visibility toggle option

### Related Test Case
TC-004

### Summary
Password field does not provide an option to toggle visibility, making it difficult for the users to verify input.

### Steps to Reproduce:
1. Navigate to https://www.saucedemo.com
2. Enter a password in the password field
3. Attempt to verify typed characters

### Actual Result
Password is masked with no option to reveal it

### Expected Result
User should have an option to toggle password visibility (e.g., eye icon)

### Severity 
Medium

### Priority 
Medium

### Status
Open

### Notes
This impacts usability and may lead to repeated login attempts due to typing errors.

---

## BUG-003 - Cart Cannot Be Closed Directly from Cart Icon

### Related Test Case 
TC-008 Cart badge update check

### Summary
After opening the shopping cart from the cart icon, the user cannot close or collapse the cart by clicking the cart icon again.

### Steps to Reproduce
1. Log into the application
2. Add one or more items to the cart
3. Click the cart icon to open the cart
4. Attempt to return to the inventory page by clicking the cart icon again

### Actual Result
The cart remains open. The user must manually click "Continue Shopping" to return to the inventory page.

### Expected Result
The cart icon should allow users to toggle between opening and closing the cart, or provide a faster navigation option back to the inventory page.

### Severity 
Low

### Priority
Medium

### Status 
Open

### Notes
When multiple items are added to the cart, the "Continue Shopping" button may appear far below the visible area, forcing the user to scroll down before being able to return to the inventory page.

---

## BUG-004 - User Cannot Increase Quantity of Same Product in Cart

### Related Test Case 
TC-011 - Add multiple quantities of the same product

### Summary
The application does not allow users to add more than one unit of the same product to the cart.

### Steps to Reproduce
1. Log into the application
2. Add a product to the cart from the inventory page
3. Try to add the same product again from the inventory page
4. Open the cart
5. Try to increase the quantity of the same product from the cart page
6. Open the product detail page and try to add the same product again

### Actual Result
The user cannot add more than one unit of the same product. There is no option to increase quantity from the inventory page, cart page, or product detail page.

### Expected Result
If multiple quantities are supported, the user should be able to increase the quantity of the same product from the cart or product page.

### Severity 
Medium

### Priority
Medium

### Status 
Open

### Notes
This may limit the shopping experience if users want to purchase more than one unit of the same product. If this is an intentional business rule, it should be clearly indicated to the user.

---

## BUG-005 - Checkout Fields Lack Proper Input Validation

### Related Test Case 
TC-010 - Empty mandatory checkout fields

### Summary
The checkout form accepts unrealistic or insufficient values in mandatory fields without proper validation.

### Steps to Reproduce
1. Log into the application
2. Add a product to the cart from the inventory page
3. Proceed to checkout
4. Enter unrealistic values such as:
   - Single-character inputs
   - Extremely long strings
   - Repetitive/random characters
5. Click "Continue"
   
### Actual Result
The system accepts unrealistic values and allows the user to continue checkout.

### Expected Result
The system should validate:
- Minimum input length
- Maximum input length
- Acceptable character formats
- Realistic customer information

### Severity 
Low

### Priority
Medium

### Status 
Open

### Notes
Additional validation rules would improve data quality and prevent unrealistic or accidental submissions in a production environment.

---

## BUG-006 - Product Description Contains Inconsistent Technical Formatting

### Related Test Case 
TC-009 - Successful checkout

### Summary
The product description for "Sauce Labs Backpack" contains technical-style formatting that appears inconsistent with the rest of the application content.

### Steps to Reproduce
1. Log into the application
2. Navigate to the inventory page
3. Locate the "Sauce Labs Backpack" product
4. Observe the product description
5. Proceed through checkout and review the same product description again
   
### Actual Result
The following text appears in the product description:

"carry.allTheThings()"

The wording resembles technical or code-style formatting and appears inconsistent with the rest of the product description and UI content.

### Expected Result
Product descriptions should use clear, user-friendly, and commercially consistent language throughout the application.

### Severity 
Low

### Priority
Low

### Status 
Open

### Notes
The issue appears in multiple areas of the application, including the inventory page and checkout overview page.

---

## BUG-007 - Product Naming Uses Technical/Code-Style Terminology

### Related Test Case 
TC-009 - Successful checkout

### Summary
Some product names contain technical or code-style terminology that may be confusing or inconsistent for regular users in an e-commerce environment.

### Steps to Reproduce
1. Log into the application
2. Navigate to the inventory page
3. Locate the product:
   "Test.allTheThings() T-Shirt (Red)"
5. Observe the product name formatting
   
### Actual Result
The product name  includes code-style terminology:

"Test.allTheThings()"

The wording resembles programming syntax rather than standard commercial product naming.

### Expected Result
Product names should use clear, user-friendly, and commercially consistent naming conventions appropriate for customers.

### Severity 
Low

### Priority
Low

### Status 
Open

### Notes
Similar technical-style wording also appears in other descriptions across the application.

---

## BUG-008 - Checkout Flow Does Not Request Customer Email Address

### Related Test Case 
TC-009 - Successful checkout

### Summary
The checkout process does not include a field for the customer's email address.

### Steps to Reproduce
1. Log into the application
2. Navigate to the inventory page
3. Add a product to the cart
4. Proceed through checkout
5. Review the information requested during the checkout
   
### Actual Result
The checkout form only requests first name, last name, and postal code. No email address is requested.

### Expected Result
The checkout process should request a customer email address to support order confirmation, communication, and receipt delivery.

### Severity 
Low

### Priority
Low

### Status 
Open

### Notes
The absence of an email field limits customer communication and order confirmation capabilities, which are commonly expected in standard e-commerce checkout flows.
