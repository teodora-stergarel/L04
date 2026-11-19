# Bug reports for exercise2.py

Line: 3
Problem: The docstring says "True if the grade is 5 or more", which means grade >= 5, but the function uses grade > 5, making it False for grade exactly 5.
Example: is_passing(5) returns False, expected True.
Fix: return grade >= 5
