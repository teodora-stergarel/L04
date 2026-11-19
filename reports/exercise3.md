# Bug reports for exercise3.py

Line: 3
Problem: The function returns division by zero when the input list is empty, but the docstring states that an empty list has an average of 0.
Example: average([]) returns ZeroDivisionError, expected 0.
Fix: return sum(numbers) / (len(numbers) if numbers else 1)

Line: 8
Problem: The function returns the first word, but if the text has no words (e.g., empty string or only whitespace), it returns an empty string, which is correct. However, if the text contains only whitespace, split() returns an empty list, and [0] will raise an IndexError. The docstring says to return "" if the text is empty, but it doesn't specify behavior on whitespace-only text.
Example: first_word("   ") returns IndexError, expected "".
Fix: return text.split()[0] if text.strip() else ""

Line: 12
Problem: The function returns division by zero when total is 0, but the docstring says the result is 0 when total is 0. Currently, it raises a ZeroDivisionError.
Example: percent(5, 0) returns ZeroDivisionError, expected 0.
Fix: return part / total * 100 if total != 0 else 0
