# Table of Contents

- [Sort a dictionary by value](#sort-dict-by-value)
- [Split string into char array](#split-string-into-char-array)
- [Default argument of get method of dictionary](#default-argument-of-get-method-of-dictionary)
- [Loop over a list and retrieve both index and value](#loop-over-a-list-and-retrieve-both-index-and-value)
- [Enumerate with given starting index](#enumerate-with-given-starting-index)

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

## Default argument of get method of dictionary

1. get() checks if the given key exists in dict. If it
   _does exist_, the value for that key is returned. Otherwise, the value of the _default argument_ is returned

   ```python
   product_for_id = {
       101: "Orange",
       202: "Butter",
   }

   product_for_id.get(101, "Default Value")
   # 'Orange'
   product_for_id.get(303, "Default Value")
   # 'Default Value'
   ```

---

## Loop over a list and retrieve both index and value

1. Using range of length

   ```python
   fruits = ['Orange', 'Banana', 'Apple', 'Pineapple']
   for i in range(len(fruits)):
       print(i, fruits[i])

   # 0 Orange
   # 1 Banana
   # 2 Apple
   # 3 Pineapple
   ```

2. Using enumerate

   ```python
   for idx, fruit in enumerate(fruits):
       print(idx, fruit)

   # 0 Orange
   # 1 Banana
   # 2 Apple
   # 3 Pineapple
   ```

---

### Important References Used

- [realpython.com](https://realpython.com/)
