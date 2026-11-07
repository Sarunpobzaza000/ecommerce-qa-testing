1. Login
TC-LOGIN-001 — Valid Login
| Field | Value |
|---|---|
| **Test Case ID** | TC-LOGIN-001 |
| **Test Scenario** | Verify that a user can log in with valid credentials |
| **Preconditions** | User is on the SauceDemo login page |
| **Test Data** | Valid SauceDemo username and password |
| **Test Steps** | 1. Enter a valid username.<br>2. Enter a valid password.<br>3. Click the **Login** button. |
| **Expected Result** | The user should be successfully logged in and the Products page should be displayed. |
| **Actual Result** | User successfully logged in, and the Products page was displayed. |
| **Status** | PASS |

TC-LOGIN-002 — Invalid Username
| Field | Value |
|---|---|
| **Test Case ID** | TC-LOGIN-002 |
| **Test Scenario** | Verify that login fails with an invalid username |
| **Preconditions** | User is on the SauceDemo login page |
| **Test Data** | Invalid username and valid password |
| **Test Steps** | 1. Enter an invalid username.<br>2. Enter a valid password.<br>3. Click the **Login** button. |
| **Expected Result** | The user should not be successfully logged in, and the Products page should not be displayed. |
| **Actual Result** | Login was unsuccessful, and the Products page was not displayed. |
| **Status** | PASS |

TC-LOGIN-003 — Invalid Password
| Field | Value |
|---|---|
| **Test Case ID** | TC-LOGIN-003 |
| **Test Scenario** | Verify that login fails with an invalid password |
| **Preconditions** | User is on the SauceDemo login page |
| **Test Data** | Valid username and invalid password |
| **Test Steps** | 1. Enter a valid username.<br>2. Enter an invalid password.<br>3. Click the **Login** button. |
| **Expected Result** | The user should not be successfully logged in, and the Products page should not be displayed. |
| **Actual Result** | Login was unsuccessful, and the Products page was not displayed. |
| **Status** | PASS |

TC-LOGIN-004 — Missing Username
| Field | Value |
|---|---|
| **Test Case ID** | TC-LOGIN-004 |
| **Test Scenario** | Verify that login fails when the username is missing |
| **Preconditions** | User is on the SauceDemo login page |
| **Test Data** | Empty username and valid password |
| **Test Steps** | 1. Leave the username field empty.<br>2. Enter a valid password.<br>3. Click the **Login** button. |
| **Expected Result** | The user should not be logged in, the Products page should not be displayed, and an appropriate validation/error message should be displayed. |
| **Actual Result** | Login was rejected, an error message was displayed, and the Products page was not displayed. |
| **Status** | PASS |

TC-LOGIN-005 — Missing Password
| Field | Value |
|---|---|
| **Test Case ID** | TC-LOGIN-005 |
| **Test Scenario** | Verify that login fails when the password is missing |
| **Preconditions** | User is on the SauceDemo login page |
| **Test Data** | Valid username and empty password |
| **Test Steps** | 1. Enter a valid username.<br>2. Leave the password field empty.<br>3. Click the **Login** button. |
| **Expected Result** | The user should not be logged in, the Products page should not be displayed, and an appropriate validation/error message should be displayed. |
| **Actual Result** | Login was rejected, an error message was displayed, and the Products page was not displayed. |
| **Status** | PASS |

TC-LOGIN-006 — Both Fields Empty
| Field | Value |
|---|---|
| **Test Case ID** | TC-LOGIN-006 |
| **Test Scenario** | Verify that login fails when username and password are missing |
| **Preconditions** | User is on the SauceDemo login page |
| **Test Data** | Empty username and empty password |
| **Test Steps** | 1. Leave the username and password fields empty.<br>2. Click the **Login** button. |
| **Expected Result** | The user should not be successfully logged in, the Products page should not be displayed, and an appropriate validation/error message should be displayed. |
| **Actual Result** | Login was rejected, an error message was displayed, and the Products page was not displayed. |
| **Status** | PASS |


2. Product Catalog
TC-PRODUCT-001 — Display Products
| Field | Value |
|---|---|
| **Test Case ID** | TC-PRODUCT-001 |
| **Test Scenario** | Verify that products are displayed correctly on the Products page |
| **Preconditions** | User is successfully logged in and on the Products page |
| **Test Data** | No specific test data required |
| **Test Steps** | 1. Log in with valid credentials.<br>2. Navigate to the Products page.<br>3. Verify that each product displays a name, description, price, and image. |
| **Expected Result** | Each product should display its name, description, price, and image correctly. |
| **Actual Result** | The name, description, price, and image were displayed correctly for each product. |
| **Status** | PASS |

TC-PRODUCT-002 — Product Details
| Field | Value |
|---|---|
| **Test Case ID** | TC-PRODUCT-002 |
| **Test Scenario** | Verify that a user can view details of a selected product |
| **Preconditions** | User is successfully logged in and on the Products page |
| **Test Data** | Select any available product |
| **Test Steps** | 1. Select a product from the Products page.<br>2. Verify the details of the selected product. |
| **Expected Result** | The selected product should display its name, description, price, and image correctly, and the information should match the selected product. |
| **Actual Result** | The selected product's name, description, price, and image were displayed correctly and matched the selected product. |
| **Status** | PASS |

TC-PRODUCT-003 — Sort Name A to Z
| Field | Value |
|---|---|
| **Test Case ID** | TC-PRODUCT-003 |
| **Test Scenario** | Verify that products can be sorted correctly by name |
| **Preconditions** | User is successfully logged in and on the Products page |
| **Test Data** | Sort option: **Name (A to Z)** |
| **Test Steps** | 1. Select **Name (A to Z)** from the sorting dropdown.<br>2. Verify the order of product names. |
| **Expected Result** | Products should be displayed in alphabetical order from A to Z. |
| **Actual Result** | Products were displayed in alphabetical order from A to Z. |
| **Status** | PASS |

TC-PRODUCT-004 — Sort Name Z to A
| Field | Value |
|---|---|
| **Test Case ID** | TC-PRODUCT-004 |
| **Test Scenario** | Verify that products can be sorted correctly by name |
| **Preconditions** | User is successfully logged in and on the Products page |
| **Test Data** | Sort option: **Name (Z to A)** |
| **Test Steps** | 1. Select **Name (Z to A)** from the sorting dropdown.<br>2. Verify the order of product names. |
| **Expected Result** | Products should be displayed in reverse alphabetical order from Z to A. |
| **Actual Result** | Products were displayed in alphabetical order from Z to A. |
| **Status** | PASS |

TC-PRODUCT-005 — Sort Price Low to High
| Field | Value |
|---|---|
| **Test Case ID** | TC-PRODUCT-005 |
| **Test Scenario** | Verify that products can be sorted correctly by price |
| **Preconditions** | User is successfully logged in and on the Products page |
| **Test Data** | Sort option: **Price (low to high)** |
| **Test Steps** | 1. Select **Price (low to high)** from the sorting dropdown.<br>2. Verify the order of product prices. |
| **Expected Result** | Products should be displayed in ascending order of price from low to high. |
| **Actual Result** | Products were displayed in ascending price order, from the lowest price to the highest price. |
| **Status** | PASS |

TC-PRODUCT-006 — Sort Price High to Low
| Field | Value |
|---|---|
| **Test Case ID** | TC-PRODUCT-006 |
| **Test Scenario** | Verify that products can be sorted correctly by price |
| **Preconditions** | User is successfully logged in and on the Products page |
| **Test Data** | Sort option: **Price (high to low)** |
| **Test Steps** | 1. Select **Price (high to low)** from the sorting dropdown.<br>2. Verify the order of product prices. |
| **Expected Result** | Products should be displayed in descending order of price from high to low. |
| **Actual Result** | Products were displayed in descending price order, from the highest price to the lowest price. |
| **Status** | PASS |

TC-PRODUCT-007 — Add Product to Cart
| Field | Value |
|---|---|
| **Test Case ID** | TC-PRODUCT-007 |
| **Test Scenario** | Verify that products can be added to the shopping cart |
| **Preconditions** | User is successfully logged in and on the Products page |
| **Test Data** | Select any product |
| **Test Steps** | 1. Select a product from the Products page.<br>2. Click **Add to cart** for the selected product.<br>3. Open the shopping cart.<br>4. Verify that the selected product is displayed. |
| **Expected Result** | The selected product should be displayed in the shopping cart. |
| **Actual Result** | The button changed from "Add to cart" to "Remove", the shopping cart icon displayed a count of "1", and the selected product was displayed in the shopping cart. |
| **Status** | PASS |

TC-PRODUCT-008 — Remove Product
| Field | Value |
|---|---|
| **Test Case ID** | TC-PRODUCT-008 |
| **Test Scenario** | Verify that products can be removed from the shopping cart |
| **Preconditions** | User is successfully logged in and a product is already in the shopping cart |
| **Test Data** | Any product already added to the shopping cart |
| **Test Steps** | 1. Open the shopping cart.<br>2. Click the **Remove** button for the selected product.<br>3. Verify that the product is removed. |
| **Expected Result** | The product should be removed from the shopping cart. |
| **Actual Result** | The button changed from "Remove" to "Add", the shopping cart icon displayed a count of "0", and the selected product was removed from the shopping cart. |
| **Status** | PASS |


3. Shopping Cart
TC-CART-001 — Product Information, Quantity, and Price
| Field | Value |
|---|---|
| **Test Case ID** | TC-CART-001 |
| **Test Scenario** | Verify that the cart shows the correct product information, quantity, and price |
| **Preconditions** | User is successfully logged in and a product is already in the shopping cart |
| **Test Data** | Any product already added to the shopping cart |
| **Test Steps** | 1. Open the shopping cart.<br>2. Find the added product.<br>3. Verify that the product information, quantity, and price match the product that was added. |
| **Expected Result** | The product information, quantity, and price should match the product that was added to the cart. |
| **Actual Result** | — |
| **Status** | — |

TC-CART-002 — Remove Product
| Field | Value |
|---|---|
| **Test Case ID** | TC-CART-002 |
| **Test Scenario** | Verify that a selected product can be removed from the shopping cart |
| **Preconditions** | User is successfully logged in and a product is already in the shopping cart |
| **Test Data** | Any product already added to the shopping cart |
| **Test Steps** | 1. Open the shopping cart.<br>2. Click the **Remove** button for the selected product.<br>3. Verify that the product is removed. |
| **Expected Result** | The product should be removed from the shopping cart. |
| **Actual Result** | — |
| **Status** | — |

TC-CART-003 — Continue Shopping
| Field | Value |
|---|---|
| **Test Case ID** | TC-CART-003 |
| **Test Scenario** | Verify that the user can continue shopping from the shopping cart |
| **Preconditions** | User is successfully logged in and is on the shopping cart page |
| **Test Data** | None |
| **Test Steps** | 1. Open the shopping cart.<br>2. Click the **Continue Shopping** button.<br>3. Verify that the user is returned to the Products page. |
| **Expected Result** | The user should be returned to the Products page. |
| **Actual Result** | — |
| **Status** | — |

TC-CART-004 — Proceed to Checkout
| Field | Value |
|---|---|
| **Test Case ID** | TC-CART-004 |
| **Test Scenario** | Verify that the user can proceed to checkout from the shopping cart |
| **Preconditions** | User is successfully logged in and a product is already in the shopping cart |
| **Test Data** | None |
| **Test Steps** | 1. Open the shopping cart.<br>2. Click the **Checkout** button.<br>3. Verify that the user is navigated to the Checkout page. |
| **Expected Result** | The user should be navigated to the Checkout page. |
| **Actual Result** | — |
| **Status** | — |

TC-CART-005 — Cart Updates
| Field | Value |
|---|---|
| **Test Case ID** | TC-CART-005 |
| **Test Scenario** | Verify that the shopping cart is updated correctly when products are added or removed |
| **Preconditions** | User is successfully logged in and is on the Products page |
| **Test Data** | Any two products |
| **Test Steps** | 1. Add Product A to the shopping cart.<br>2. Open the shopping cart and verify that Product A is displayed.<br>3. Return to the Products page.<br>4. Add Product B to the shopping cart.<br>5. Open the shopping cart and verify that Product A and Product B are displayed.<br>6. Remove Product A from the shopping cart.<br>7. Verify that Product A is removed and Product B remains in the cart. |
| **Expected Result** | After each add or remove action, the shopping cart should display the correct products. Product A should appear after it is added, Product B should appear after it is added, and Product A should no longer appear after it is removed while Product B remains in the cart. |
| **Actual Result** | — |
| **Status** | — |


4. Checkout
TC-CHECKOUT-001 — Valid Checkout Information
| Field | Value |
|---|---|
| **Test Case ID** | TC-CHECKOUT-001 |
| **Test Scenario** | Verify that the user can enter valid checkout information |
| **Preconditions** | User is successfully logged in, a product is already in the shopping cart, and the user is on the Shopping Cart page |
| **Test Data** | Valid first name, last name, and postal code |
| **Test Steps** | 1. Open the shopping cart.<br>2. Click the **Checkout** button.<br>3. Verify that the user is navigated to the Checkout page.<br>4. Enter a valid first name, last name, and postal code.<br>5. Click the **Continue** button.<br>6. Verify that the user is navigated to the Checkout Overview page. |
| **Expected Result** | The checkout information should be accepted, and the user should be navigated to the Checkout Overview page. |
| **Actual Result** | — |
| **Status** | — |

TC-CHECKOUT-002 — Missing First Name
| Field | Value |
|---|---|
| **Test Case ID** | TC-CHECKOUT-002 |
| **Test Scenario** | Verify that required checkout fields are validated when the first name is missing |
| **Preconditions** | User is successfully logged in, a product is already in the shopping cart, and the user is on the Checkout page |
| **Test Data** | Empty first name, valid last name, and valid postal code |
| **Test Steps** | 1. Leave the **First Name** field empty.<br>2. Enter a valid last name.<br>3. Enter a valid postal code.<br>4. Click the **Continue** button. |
| **Expected Result** | The checkout information should be rejected, and an appropriate validation/error message should be displayed. |
| **Actual Result** | — |
| **Status** | — |

TC-CHECKOUT-003 — Missing Last Name
| Field | Value |
|---|---|
| **Test Case ID** | TC-CHECKOUT-003 |
| **Test Scenario** | Verify that required checkout fields are validated when the last name is missing |
| **Preconditions** | User is successfully logged in, a product is already in the shopping cart, and the user is on the Checkout page |
| **Test Data** | Valid first name, empty last name, and valid postal code |
| **Test Steps** | 1. Enter a valid **First Name**.<br>2. Leave the **Last Name** field empty.<br>3. Enter a valid postal code.<br>4. Click the **Continue** button. |
| **Expected Result** | The checkout information should be rejected, and an appropriate validation/error message should be displayed. |
| **Actual Result** | — |
| **Status** | — |

TC-CHECKOUT-004 — Missing Postal Code
| Field | Value |
|---|---|
| **Test Case ID** | TC-CHECKOUT-004 |
| **Test Scenario** | Verify that required checkout fields are validated when the postal code is missing |
| **Preconditions** | User is successfully logged in, a product is already in the shopping cart, and the user is on the Checkout page |
| **Test Data** | Valid first name, valid last name, and empty postal code |
| **Test Steps** | 1. Enter a valid **First Name**.<br>2. Enter a valid **Last Name**.<br>3. Leave the **Postal Code** field empty.<br>4. Click the **Continue** button. |
| **Expected Result** | The checkout information should be rejected, and an appropriate validation/error message should be displayed. |
| **Actual Result** | — |
| **Status** | — |

TC-CHECKOUT-005 — Checkout Overview
| Field | Value |
|---|---|
| **Test Case ID** | TC-CHECKOUT-005 |
| **Test Scenario** | Verify that the Checkout Overview displays the correct products and prices |
| **Preconditions** | User is successfully logged in, a product is already in the shopping cart, checkout information has been entered successfully, and the user is on the Checkout Overview page |
| **Test Data** | Any product added to the shopping cart |
| **Test Steps** | 1. Verify that the product name, description, quantity, and price match the selected product.<br>2. Verify that the subtotal equals the sum of the product prices.<br>3. Verify that the displayed tax is calculated correctly.<br>4. Verify that the total equals the subtotal plus the tax. |
| **Expected Result** | The Checkout Overview should display the correct product information, quantity, and price. The subtotal, tax, and total should also be calculated and displayed correctly. |
| **Actual Result** | — |
| **Status** | — |

TC-CHECKOUT-006 — Complete Order
| Field | Value |
|---|---|
| **Test Case ID** | TC-CHECKOUT-006 |
| **Test Scenario** | Verify that the user can successfully complete an order from the Checkout Overview page |
| **Preconditions** | User is successfully logged in, a product is already in the shopping cart, checkout information has been entered successfully, and the user is on the Checkout Overview page |
| **Test Data** | Any product added to the shopping cart |
| **Test Steps** | 1. Click the **Finish** button.<br>2. Verify that the user is navigated to the **Checkout Complete** page. |
| **Expected Result** | The Checkout Complete page should be displayed with an order confirmation message. |
| **Actual Result** | — |
| **Status** | — |