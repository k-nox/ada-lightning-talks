# The Ternary Operator in Python

By: Lux Barker (they/them)

---

##### What Is It?

- inline if/else statement
- lowest priority of all Python operators
- alternative name: conditional expression

---

##### Syntax

```python
evaluate_this_value if this_condition_is_true else evaluate_this_instead

# the above is the same as:
if this_condition_is_true:
    evaluate_this_value
else:
    evaulate_this_instead
```

---

##### Using the Ternary Operator in Return Statements

```python
def return_lower_num(num1, num2):
    return num1 if num1 < num2 else num2

# the above is the same as:
def return_lower_num(num1, num2):
    if num1 < num2:
        return num1
    else:
        return num2
```

---

##### Using the Ternary Operator in Variable Assignments

```python
gay = True

me = "gay" if gay else "not gay"
# the above is the same as:
if gay:
    me = "gay"
else:
    me = "not gay"
```

---

##### Using the Ternary Operator with Default Parameters

```python
# this is super useful when you want to assign a list, dictionary, etc as a default parameter
class Car:
    def __init__(self, features=None):
        self.features = features if features else []
        
# the above is the same as:
class Car:
    def __init__(self, features=None):
        if features:
            self.features = features
        else:
            self.features = []

```

---

##### Learn More

- [Geeks For Geeks - Ternary Operator in Python](https://www.geeksforgeeks.org/ternary-operator-in-python/)
- [Python Tips - Ternary Operatory](https://book.pythontips.com/en/latest/ternary_operators.html)
- [Python Docs - Conditional Expression](https://docs.python.org/3/reference/expressions.html#conditional-expressions)

