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

1. Test Case: Checkout as a guest
Expectation: A user can check out as a guest without creating an account. The system should not require the user to log in.

Specifications:
- Open the website and add items to the shopping cart.
- Click on the checkout button and select "checkout as a guest" option.
- Verify that the system prompts for the necessary information like shipping address, billing address, and payment information.
- Verify that after submitting the checkout information, the system displays a confirmation message and a summary of the order.
- Verify that the user receives an order confirmation email with the details of the order.

Edge Cases:
- If the user enters invalid or incomplete information, the system should display an error message.
- If the user enters a non-existent or invalid email address, the system should display an error message.

2. Test Case: Checkout as a logged-in user
Expectation: A user can check out as a logged-in user by using their existing account information.

Specifications:
- Open the website and add items to the shopping cart.
- Log in with an existing user account.
- Click on the checkout button and verify that the system pre-populates the user's saved shipping address, billing address, and payment information.
- Verify that the user can edit or update the checkout information if necessary.
- Verify that after submitting the checkout information, the system displays a confirmation message and a summary of the order.
- Verify that the user receives an order confirmation email with the details of the order.

Edge Cases:
- If the user's saved information is invalid or incomplete, the system should prompt the user to update the information.
- If the user enters invalid or incomplete information, the system should display an error message.

3. Test Case: Empty Cart
Expectation: If the cart is empty, the user should not be able to proceed with the checkout process.

Specifications:
- Open the website and verify that the shopping cart is empty.
- Click on the checkout button and verify that the system displays an error message indicating that the cart is empty.

Edge Cases:
- If the user tries to add an out-of-stock item to the cart, the system should display an error message.

4. Test Case: Account Creation or Login Prompt
Expectation: If the user checks out as a guest, the system should prompt the user to create an account or log in.

Specifications:
- Open the website and add items to the shopping cart.
- Click on the checkout button and select "checkout as a guest" option.
- Verify that the system prompts the user to create an account or log in.
- Verify that the user can choose to ignore the prompt and proceed with the checkout process as a guest.

Edge Cases:
- If the user already has an existing account, the system should prompt the user to log in instead of creating a new account.
- If the user is already logged in, the system should skip the account creation or login prompt.
