# Test Cases - Login Functionality

| TC ID  | Title                         | Preconditions        | Steps                                                                 | Expected Result                          | Priority |
|--------|------------------------------|---------------------|----------------------------------------------------------------------|------------------------------------------|----------|
| TC-001 | Valid login                  | User on login page  |  1. Go to http://www.saucedemo.com 2.Enter username: standard_user 3. Enter password: secret_sauce 4. Click login     | User is redirected to inventory page     | High     |
| TC-002 | Invalid password             | User on login page  | 1. Enter username: standard_user  2. Enter invalid password  3. Click login   | Error message is displayed               | High     |
| TC-003 | Empty fields                 | User on login page  | 1. Leave fields username and password empty  2. Click login                               | Validation error is displayed            | Medium   |
| TC-004 | Password usability check     | User on login page  | 1. Enter password  2. Try to verify input                           | User can confirm password input easily   | Medium   |
| TC-005 | Empty password field | User on login page | 1. Enter valid username 2. Leave password empty 3. Click login | Password required validation is displayed | Medium |
| TC-006 | Add product to cart | User logged into the application | 1. Navigate to inventory page 2. Click “Add to cart” on a product | Product is added to the cart and cart badge updates correctly | High |
| TC-007 | Remove product from cart | Product already added to cart | 1. Navigate to cart 2. Click “Remove” on selected product | Product is removed from the cart and cart badge updates correctly | High |
| TC-008 | Cart badge update check | User logged into the application | 1. Add one or more products to cart 2. Observe cart badge 3. Remove a product 4. Observe cart badge again | Cart badge reflects correct quantity after each action | Medium |
| TC-009 | Successful checkout | At least one product added to cart | 1. Navigate to cart 2. Click checkout 3. Enter valid customer information 4. Continue checkout 5. Finish purchase | Checkout process completes successfully and confirmation page is displayed | High |
| TC-010 | Empty mandatory checkout fields | At least one product added to cart | 1. Navigate to checkout page 2. Leave one or more mandatory fields empty 3. Click continue | Validation message is displayed for any missing required field and prevents continuation | Medium |
