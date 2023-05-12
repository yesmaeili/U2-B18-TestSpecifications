# U2-B18-TestSpecifications
U2-Block18-Writing Test Specifications

Unit Test
Unit Test Specifications:

1. A function called "multiplication" that returns the product of the two input numbers.
Expect multiplication(2, 3) to be a number
Expect multiplication(2, 3) to be equal to 6
Expect multiplication(0, 3) to be equal to 0
Expect multiplication(-2, 3) to be equal to -6
Expect multiplication(2, "a") to be an error
Expect multiplication() to be an error


2. A function called "concatOdds" takes two arrays of integers as arguments. It should return a single array that only contains the odd numbers, in ascending order, from both of the arrays.
Expect concatOdds([3, 2, 1], [9, 1, 1, 1, 4, 15, -1]) to be an array
Expect concatOdds([3, 2, 1], [9, 1, 1, 1, 4, 15, -1]) to be equal to [-1, 1, 3, 9, 15]
Expect concatOdds([], []) to be equal to []
Expect concatOdds([2, 4], [8, 6]) to be equal to []
Expect concatOdds([1, 3, 5], [1, 3, 5]) to be equal to [1, 3, 5]
Expect concatOdds([2, 3, 5], [1, 3, 5]) to be equal to [1, 3, 5]
Expect concatOdds([2, 4], [1, 3, 5]) to be equal to [1, 3, 5]
Expect concatOdds([1, 3, 5], []) to be equal to [1, 3, 5]
Expect concatOdds([], [1, 3, 5]) to be equal to [1, 3, 5]
Expect concatOdds(["a", 3], [1, 3, 5]) to be an error
Expect concatOdds([1, 3, 5], [1, "a"]) to be an error
Expect concatOdds([1, 3, 5], [1, 3, 3, 5]) to be equal to [1, 3, 5]

Functional Tests:
Functional Tests for Shopping Cart Checkout Feature:
Test Specifications for Shopping Cart Checkout Feature:

1. When a user with an empty cart selects the checkout option:
   - Expectation: The user should be notified that their cart is empty.
   - The user should be provided with options to continue shopping or go back to the cart.

2. When a guest user proceeds to checkout without creating an account:
   - Expectation: The user should be able to enter their shipping and billing information as a guest.
   - The user should be asked if they want to create an account or log in for future purchases.
   - The user should be able to proceed to the payment step without logging in.

3. When a guest user decides to create an account during checkout:
   - Expectation: The user should be prompted to enter their email address and password to create an account.
   - The user's entered information should be associated with the newly created account.
   - The user should be able to proceed to the payment step after creating the account.

4. When a registered user logs in during checkout:
   - Expectation: The user should be prompted to enter their login credentials (email and password).
   - The user's entered credentials should be validated.
   - If the credentials are valid, the user should be logged in and their saved shipping and billing information should be pre-filled.
   - The user should be able to proceed to the payment step after logging in.

5. When a user proceeds to the payment step:
   - Expectation: The user should be able to select a payment method (credit card, PayPal, etc.).
   - The user should be able to enter their payment details securely.
   - The user's entered payment details should be validated for correctness.
   - If any errors are encountered, the user should be shown appropriate error messages.

6. When a user completes the checkout process:
   - Expectation: The user should receive an order confirmation.
   - The user should be provided with an order summary containing details such as items purchased, shipping address, billing information, and total cost.
   - The user should be given an order number or reference for future reference.

7. When the user encounters any errors or issues during the checkout process:
   - Expectation: Proper error messages should be displayed to the user indicating the cause of the error.
   - The user should be able to correct the error or take appropriate action to resolve the issue.

8. When a user abandons the checkout process at any step:
   - Expectation: The user's cart should remain unchanged.
   - The user should be able to resume the checkout process from where they left off, with all previously entered information pre-filled.

9. When the user interacts with the checkout steps:
   - Expectation: The user should be provided with clear and intuitive navigation options to move forward or backward through the checkout steps.
   - The user should be able to review and modify their entered information at any step before finalizing the purchase.

10. When the user completes the checkout process successfully:
    - Expectation: The items in the user's cart should be removed or marked as purchased.
    - The user should receive an email confirmation with the order details.
