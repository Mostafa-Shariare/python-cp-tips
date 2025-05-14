## 📥 INPUT TECHNIQUES

### 1. Standard Input (Single Line)

```python
x = input()              # Reads a single line as string
n = int(input())         # Reads a single integer
```

### 2. Multiple Space-Separated Integers in One Line

```python
a, b = map(int, input().split())
```

### 3. List of Integers in One Line

```python
arr = list(map(int, input().split()))
```

### 4. Reading N Lines of Input (e.g. 2D array)

```python
n = int(input())
arr = [list(map(int, input().split())) for _ in range(n)]
```

### 5. Fast Input Using `sys.stdin`

```python
import sys
input = sys.stdin.readline

n = int(input())
arr = list(map(int, input().split()))
```

Useful for large inputs in online judges.

---

## 📤 OUTPUT TRICKS

### 6. Print Elements Space-Separated

```python
print(*arr)  # arr = [1, 2, 3] → prints: 1 2 3
```

### 7. Join Elements into a String

```python
print(" ".join(map(str, arr)))
```

---

## 🧠 USEFUL PYTHON TRICKS FOR CP

### 8. Swapping Two Values

```python
a, b = b, a
```

### 9. Reversing a List

```python
arr[::-1]  # returns a reversed copy
arr.reverse()  # reverses in-place
```

### 10. Sorting

```python
sorted_arr = sorted(arr)      # returns new sorted list
arr.sort(reverse=True)        # sorts in-place descending
```

### 11. Frequency Count (Using `collections`)

```python
from collections import Counter
counter = Counter(arr)
```

### 12. Using Default Dictionary

```python
from collections import defaultdict
d = defaultdict(int)
d["apple"] += 1
```

### 13. One-Line 2D List Initialization

```python
grid = [[0]*m for _ in range(n)]
```

Avoid `grid = [[0]*m]*n` (buggy reference behavior).

### 14. Transposing a Matrix

```python
transposed = list(zip(*grid))
```

---

## 🧮 MATH AND STRING TRICKS

### 15. Checking for Prime

```python
def is_prime(n):
    if n <= 1: return False
    for i in range(2, int(n**0.5)+1):
        if n % i == 0:
            return False
    return True
```

### 16. String Reversal

```python
s[::-1]
```

### 17. ASCII Value

```python
ord('a') → 97
chr(97) → 'a'
```

---

## 🔁 LOOPING SMARTER

### 18. Enumerate for Index + Value

```python
for i, val in enumerate(arr):
    print(i, val)
```

### 19. Loop in Reverse

```python
for i in range(n-1, -1, -1):
    print(arr[i])
```

---

## 🛠️ DEBUGGING TRICKS

### 20. Pretty Print with f-Strings

```python
x, y = 10, 20
print(f"x = {x}, y = {y}")
```


