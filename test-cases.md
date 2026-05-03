# Test Cases - Login Functionality

## Test Case 1: Valid login

Steps:
1. Go to http://www.saucedemo.com
2. Enter username: standard_user
3. Enter password: secret_sauce
4. Click login

Expected result:
User is redirected to the inventory page 

------

## Test Case 2: Invalid password

Steps:
1. Enter username: standard_user
2. Enter incorrect password
3. Click login

Expected result: 
Error message is displayed

------

## Test Case 3: Empty Fields

Steps:
1. Leave username empty
2. Leave password empty
3. Click login

Expected result:
Validation error is shown
