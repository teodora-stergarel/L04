# Bug reports for exercise1.py

Line: 3
Problem: The function is_even returns True for odd numbers because it checks n % 2 == 1, which is incorrect. It should return True for even numbers, meaning n % 2 == 0.
Example: is_even(2) returns False, expected True.
Fix: return n % 2 == 0

Line: 8
Problem: The function rectangle_area returns the sum of width and height, but it should return the product (area) of width and height.
Example: rectangle_area(4, 5) returns 9, expected 20.
Fix: return width * height

Line: 13
Problem: The function double adds 2 to n, but it should return twice the number, i.e., n * 2.
Example: double(3) returns 5, expected 6.
Fix: return n * 2
