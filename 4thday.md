In Python, both `sorted()` and `.sort()` are used to sort lists. The main difference is **whether they modify the original list or create a new list.**


- Works with any iterable (list, tuple, string, set, etc.).
- Does not modify the original list.
- Returns a new sorted list.

```
numbers = [5, 2, 8, 1, 3]result = sorted(numbers)print(result)print(numbers)
```

**Output:**

```
[1, 2, 3, 5, 8]
[5, 2, 8, 1, 3]
```

Notice that the original list remains unchanged.

## **2.&#x20;**`.sort()`**&#x20;– Modifies the original list**

- Works only with lists.
- Modifies the original list directly.
- Returns `None`.

```
numbers = [5, 2, 8, 1, 3]result = numbers.sort()print(numbers)print(result)
```

**Output:**

```
[1, 2, 3, 5, 8]
None
```

Notice that the original list itself is sorted.

## **3. Key differences**

| Feature            | `sorted()`         | `.sort()`      |
| ------------------ | ------------------ | -------------- |
| Type               | Built-in function  | List method    |
| Returns            | New sorted list    | None           |
| Original list      | Unchanged          | Modified       |
| Works with tuples  | Yes                | No             |
| Works with strings | Yes                | No             |
| Memory             | Creates a new list | Sorts in place |

## **4. Both support&#x20;**`reverse=True`

```
numbers = [5, 2, 8, 1, 3]print(sorted(numbers, reverse=True))
```

Output:

```
[8, 5, 3, 2, 1]
```

Using `.sort()`:

```
numbers.sort(reverse=True)print(numbers)
```

Output:

```
[8, 5, 3, 2, 1]
```



**Easy way to remember:**

- `sorted()` → New list.
- `.sort()` → Same list, modified.
