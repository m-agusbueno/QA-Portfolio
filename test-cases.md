# Test Cases - Login Functionality

# Test Cases – Login Functionality

| TC ID  | Title                         | Preconditions        | Steps                                                                 | Expected Result                          | Priority |
|--------|------------------------------|---------------------|----------------------------------------------------------------------|------------------------------------------|----------|
| TC-001 | Valid login                  | User on login page  | 1. Enter valid username  2. Enter valid password  3. Click login     | User is redirected to inventory page     | High     |
| TC-002 | Invalid password             | User on login page  | 1. Enter valid username  2. Enter invalid password  3. Click login   | Error message is displayed               | High     |
| TC-003 | Empty fields                 | User on login page  | 1. Leave fields empty  2. Click login                               | Validation error is displayed            | Medium   |

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
