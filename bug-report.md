# Bug Report

---

## BUG-001 - Unclear error message for invalid login credentials

### Related Test Case 
TC-002

### Sumary
Error message does not clearly indicate whether the issue is with the username or the password

### Environment
- URL: https://www.saucedemo.com
- Browser: Mozilla Firefox
- Device: Laptop

### Steps to Reproduce:
1. Navigate to https://www.saucedemo.com
2. Enter valid username (e.g., standard_user)
3. Enter incorrect password
4. Click login

### Actual Result
Message displayed:
"Epic sadface: Username and password do not match any user in this servic"

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

### Environment
- URL: https://www.saucedemo.com
- Browser: Mozilla Firefox
- Device: Laptop

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
