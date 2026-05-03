# Test Cases - Login Functionality

| TC ID  | Title                         | Preconditions        | Steps                                                                 | Expected Result                          | Priority |
|--------|------------------------------|---------------------|----------------------------------------------------------------------|------------------------------------------|----------|
| TC-001 | Valid login                  | User on login page  |  1. Go to http://www.saucedemo.com 2.Enter username: standard_user 3. Enter password: secret_sauce 4. Click login     | User is redirected to inventory page     | High     |
| TC-002 | Invalid password             | User on login page  | 1. Enter username: standard_user  2. Enter invalid password  3. Click login   | Error message is displayed               | High     |
| TC-003 | Empty fields                 | User on login page  | 1. Leave fields username and password empty  2. Click login                               | Validation error is displayed            | Medium   |



