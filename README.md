# Table of Contents

- [Sort a dictionary by value](#sort-dict-by-value)
- [Split string into char array](#split-string-into-char-array)

---

## Sort dict by value

1. Using lambda

   ```python
   my_dict = {'a': 4, 'b': 3, 'c': 2, 'd':1}

   sorted(my_dict.items(), key=lambda x: x[1])
   #[('d': 1), ('c': 2), ('b': 3), ('a' : 4)]
   ```

2. Using operator

   ```python
   import operator
   sorted(my_dict.items(), key=operator.itemgetter(1))
   #[('d', 1), ('c', 2), ('b', 3), ('a', 4)]
   ```

---

## Split string into char array

1. You need to use list

```python
str = "mylist"
list(str)
# ['m', 'y', 'l', 'i', 's', 't']
```

---

### Important References Used

- [realpython.com](https://realpython.com/)
