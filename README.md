### Python Operators

Python provides several types of **operators** used to perform operations on variables and values. Here's a breakdown of the main ones:

---

### 1. **Arithmetic Operators**

Used for numeric calculations:

| Operator | Description    | Example         |
| -------- | -------------- | --------------- |
| `+`      | Addition       | `3 + 2` → `5`   |
| `-`      | Subtraction    | `3 - 2` → `1`   |
| `*`      | Multiplication | `3 * 2` → `6`   |
| `/`      | Division       | `3 / 2` → `1.5` |
| `//`     | Floor Division | `3 // 2` → `1`  |
| `%`      | Modulus        | `3 % 2` → `1`   |
| `**`     | Exponentiation | `2 ** 3` → `8`  |

---

### 2. **Assignment Operators**

Used to assign values to variables:

| Operator | Description             | Example                        |
| -------- | ----------------------- | ------------------------------ |
| `=`      | Assign                  | `x = 5`                        |
| `+=`     | Add and assign          | `x += 2` (same as `x = x + 2`) |
| `-=`     | Subtract and assign     | `x -= 1`                       |
| `*=`     | Multiply and assign     | `x *= 3`                       |
| `/=`     | Divide and assign       | `x /= 2`                       |
| `//=`    | Floor divide and assign | `x //= 2`                      |
| `%=`     | Modulus and assign      | `x %= 3`                       |
| `**=`    | Power and assign        | `x **= 2`                      |

---

### 3. **Comparison Operators**

Used to compare values:

| Operator | Description      | Example            |
| -------- | ---------------- | ------------------ |
| `==`     | Equal to         | `3 == 3` → `True`  |
| `!=`     | Not equal to     | `3 != 2` → `True`  |
| `>`      | Greater than     | `4 > 2` → `True`   |
| `<`      | Less than        | `4 < 5` → `True`   |
| `>=`     | Greater or equal | `5 >= 5` → `True`  |
| `<=`     | Less or equal    | `3 <= 2` → `False` |

---

### 4. **Logical Operators**

Used to combine conditional statements:

| Operator | Description | Example                    |
| -------- | ----------- | -------------------------- |
| `and`    | Logical AND | `True and False` → `False` |
| `or`     | Logical OR  | `True or False` → `True`   |
| `not`    | Logical NOT | `not True` → `False`       |

---

### 5. **Bitwise Operators**

Used to work on binary numbers:

| Operator | Description | Example         |     |         |
| -------- | ----------- | --------------- | --- | ------- |
| `&`      | AND         | `5 & 3` → `1`   |     |         |
| \`       | \`          | OR              | \`5 | 3`→`7\` |
| `^`      | XOR         | `5 ^ 3` → `6`   |     |         |
| `~`      | NOT         | `~5` → `-6`     |     |         |
| `<<`     | Left Shift  | `5 << 1` → `10` |     |         |
| `>>`     | Right Shift | `5 >> 1` → `2`  |     |         |

---

### 6. **Membership Operators**

Used to check membership in a sequence:

| Operator | Description | Example                       |
| -------- | ----------- | ----------------------------- |
| `in`     | Is in       | `'a' in 'apple'` → `True`     |
| `not in` | Is not in   | `'x' not in 'apple'` → `True` |

---

### 7. **Identity Operators**

Compare memory locations (not just values):

| Operator | Description     | Example      |
| -------- | --------------- | ------------ |
| `is`     | Same object     | `x is y`     |
| `is not` | Not same object | `x is not y` |

---

In Python, **operator precedence** determines the order in which operations are evaluated. Operators with higher precedence are evaluated before those with lower precedence.

Here’s the **operator precedence table** (from highest to lowest):

---

### 🔝 **Highest Precedence to Lowest**

| Precedence | Operators                                                        | Description                                  |            |
| ---------- | ---------------------------------------------------------------- | -------------------------------------------- | ---------- |
| 1          | `()`                                                             | Parentheses                                  |            |
| 2          | `**`                                                             | Exponentiation                               |            |
| 3          | `+x`, `-x`, `~x`                                                 | Unary plus, minus, bitwise NOT               |            |
| 4          | `*`, `/`, `//`, `%`                                              | Multiplication, division, floor div, modulus |            |
| 5          | `+`, `-`                                                         | Addition, subtraction                        |            |
| 6          | `<<`, `>>`                                                       | Bitwise shifts                               |            |
| 7          | `&`                                                              | Bitwise AND                                  |            |
| 8          | `^`                                                              | Bitwise XOR                                  |            |
| 9          | \`                                                               | \`                                           | Bitwise OR |
| 10         | `==`, `!=`, `>`, `<`, `>=`, `<=`, `is`, `is not`, `in`, `not in` | Comparisons                                  |            |
| 11         | `not`                                                            | Logical NOT                                  |            |
| 12         | `and`                                                            | Logical AND                                  |            |
| 13         | `or`                                                             | Logical OR                                   |            |
| 14         | `if ... else`                                                    | Ternary conditional                          |            |
| 15         | `=`, `+=`, `-=`, etc.                                            | Assignment                                   |            |
| 16         | `lambda`                                                         | Lambda expressions                           |            |

---

### 🧠 **Example to Show Precedence:**

```python
result = 3 + 4 * 2 ** 2
# Step-by-step:
# 2 ** 2 → 4
# 4 * 4 → 16
# 3 + 16 → 19
print(result)  # Output: 19
```

You can **override precedence** using parentheses:

```python
result = (3 + 4) * 2 ** 2
# (3 + 4) = 7
# 2 ** 2 = 4
# 7 * 4 = 28
print(result)  # Output: 28
```

---

