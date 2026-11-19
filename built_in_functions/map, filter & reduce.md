map() – transforms every element.



filter() – selects elements based on a condition.



reduce() – combines all elements into a single result.


These are Python functional programming tools used to process collections.
A. map() – Transform every element
Example: Square every number.
numbers = [1, 2, 3, 4, 5]result = list(map(lambda x: x * x, numbers))print(result)



Output:
[1, 4, 9, 16, 25]


Remember: map() applies a function to every element.
B. filter() – Select elements based on a condition
Example: Find even numbers.
numbers = [1, 2, 3, 4, 5, 6]result = list(filter(lambda x: x % 2 == 0, numbers))print(result)



Output:
[2, 4, 6]


Remember: filter() selects elements that satisfy a condition.
C. reduce() – Combine elements into one result
reduce() is available in the functools module.

Example: Calculate the sum of all numbers.
from functools import reducenumbers = [1, 2, 3, 4, 5]result = reduce(lambda x, y: x + y, numbers)print(result)



Output:
15
