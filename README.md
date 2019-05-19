# Table of Contents

- [Sort a dictionary by value](#sort-dict-by-value)

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

### Important References Used

- [realpython.com](https://realpython.com/)
-
