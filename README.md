# U2-B18-TestSpecifications
U2-Block18-Writing Test Specifications

Unit Test
1. A function called "multiplication" that returns the product of the two input numbers.

Expect multiplication(num1, num2) to return the product of two input numbers.
Expect multiplication(2, 3) to be equal to 6
Expect multiplication(-2, 3) to be equal to -6
Expect multiplication(0, 3) to be equal to 0
Expect multiplication("2", 3) to be NaN
Expect multiplication(2, Infinity) to be Infinity
Expect multiplication(1.5, 2.5) to be equal to 3.75
Expect multiplication(1e+25, 1e+25) to be equal to 1e+50


2. A function called "concatOdds" takes two arrays of integers as arguments. It should return a single array that only contains the odd numbers, in ascending order, from both of the arrays.

Test Specifications:

Test Case 1: concatOdds([3, 2, 1], [9, 1, 1, 1, 4, 15, -1]) should return [-1, 1, 3, 9, 15]
Test Case 2: concatOdds([], []) should return []
Test Case 3: concatOdds([2, 4, 6], [1, 3, 5]) should return [1, 3, 5]
Test Case 4: concatOdds([1, 2, 3, 4, 5], [6, 7, 8, 9, 10]) should return [1, 3, 5, 7, 9]
Test Case 5: concatOdds([1, 1, 1, 1], [3, 3, 3, 3]) should return [1, 3]
Test Case 6: concatOdds([2, 4, 6], [8, 10, "a", "b", 13, 15, 17]) should return [13, 15, 17]
Test Case 7: concatOdds([-5, -3, -1, 0, 1, 3, 5], [2, 4, 6]) should return [-5, -3, -1, 1, 3, 5]

Functional Tests:
1. A shopping cart checkout feature that allows a user to check out as a guest (without an account), or as a logged-in user. They should be allowed to do either, but should be asked if they want to create an account or log in if they check out as a guest.

Here are some functional test specifications for the shopping cart checkout feature:

1. Test for empty cart:
- Expect user to see a message indicating that their cart is empty when they try to checkout.
- Expect user to be redirected to the cart page when they click on the "Back to Cart" button.

2. Test for guest checkout:
- Expect user to see an option to checkout as a guest on the checkout page.
- Expect user to be prompted to enter their shipping and billing information.
- Expect user to be asked if they want to create an account or log in if they choose to checkout as a guest.
- Expect the guest user's information to be saved in the system if they choose to create an account.

3. Test for logged-in user checkout:
- Expect user to see an option to login on the checkout page if they are not already logged in.
- Expect user to be redirected to the login page if they click on the "Login" button.
- Expect user to be prompted to enter their shipping and billing information if they are not already saved in the system.
- Expect user to be given the option to save their information for future use.

4. Test for displaying information:
- Expect user to see a summary of their order (items, quantity, price) on the checkout page.
- Expect user to see the shipping and billing information they entered or previously saved.
- Expect user to see the total cost of their order (including tax and shipping fees) before they confirm their order.

5. Test for completing the order:
- Expect user to be prompted to confirm their order before it is processed.
- Expect user to see a message indicating that their order has been successfully placed.
- Expect user to receive an email confirmation of their order.
- Expect the items in the user's cart to be removed after the order is completed.

6. Test for error handling:
- Expect user to see an error message if there is an issue with their payment information.
- Expect user to see an error message if there is an issue with their shipping or billing information.
- Expect user to see an error message if there is an issue with the system processing their order.

These tests cover the basic functionality of the shopping cart checkout feature, including handling empty carts, guest checkout, logged-in user checkout, displaying order information, completing the order, and error handling.
