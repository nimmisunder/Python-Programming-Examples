# **Python List Comprehensions**

A **list comprehension** is a shorter and cleaner way to create a new list from an existing iterable (list, range, string, etc.).

Instead of writing a `for` loop and using `append()`, we can create a list in a single line.

## **1. Normal for loop vs List comprehension**

**Traditional approach:**

```
numbers = [1, 2, 3, 4, 5]
squares = []
for num in numbers:
 squares.append(num * num)
print(squares)
```

Output:

```
[1, 4, 9, 16, 25]
```

**Using list comprehension:**

```
numbers = [1, 2, 3, 4, 5]
squares = [num * num for num in numbers]
print(squares)
```

Output:

```
[1, 4, 9, 16, 25]
```

Same result, less code!

## **2. Syntax**

```
new_list = [expression for item in iterable]
```

Understand each part:

| Part       | Meaning                   |
| ---------- | ------------------------- |
| expression | What you want to store    |
| for        | Iteration                 |
| item       | Current element           |
| iterable   | List, range, string, etc. |

## **3. List comprehension with conditions (if)**

Suppose you want only even numbers.

```
numbers = [1, 2, 3, 4, 5, 6, 7, 8]
even = [num for num in numbers if num % 2 == 0]
print(even)
```

Output:

```
[2, 4, 6, 8]
```

Here:

- `num` → value to store.
- `for num in numbers` → loops through numbers.
- `if num % 2 == 0` → checks whether the number is even.

Syntax:

```
[expression for item in iterable if condition]
```

## **4. Using if-else**

Suppose you want to label numbers as Even or Odd.

```
numbers = [1, 2, 3, 4, 5]result =
 ["Even" if num % 2 == 0 else "Odd"
for num in numbers]print(result)
```

Output:

```
['Odd', 'Even', 'Odd', 'Even', 'Odd']
```

Notice the difference:

- `if` at the end filters elements.
- `if-else` before `for` decides what value to store.

## **5. Working with strings**

```
name = "python"result = [letter.upper() for letter in name]print(result)
```

Output:

```
['P', 'Y', 'T', 'H', 'O', 'N']
```

## **6. Nested loops**

You can also use multiple loops.

```
result = [(x, y) for x in [1, 2] for y in [3, 4]]print(result)
```

Output:

```
[(1, 3), (1, 4), (2, 3), (2, 4)]
```

This is equivalent to:

```
result = []for x in [1, 2]:    for y in [3, 4]:        result.append((x, y))
```

## **7. Practice exercises**

Let's test your understanding. Try these without looking at the answers.

**Python practice**


**Q1. Create a list containing squares of numbers from 1 to 10.**

sq=[num\*\*2 for num in range(1,11)]\<br>print(sq)



**Q2. Extract numbers greater than 5 from this list.**

num=[num for num in sq if num>5]




**Q3. Convert all names to uppercase.**

uppernae=[name.upper for name in names]


**Q4. Replace negative numbers with 0, keeping positive numbers unchanged.**



## **Interview tips / Important points to remember**

1. List comprehension creates a new list.
2. It is generally more concise than a traditional loop with `append()`.
3. You can use conditions to filter elements.
4. You can use if-else to transform elements.
5. Nested list comprehensions support multiple loops.
6. Avoid overly complicated comprehensions because readability matters.

**Next topic:** Dictionary comprehensions — creating dictionaries using a similar approach.
