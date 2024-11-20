# Python Arrays

**Note:** Python does not have built-in support for Arrays, but Python Lists can be used instead.

## Arrays

**Note:** This page shows you how to use **LISTS** as **ARRAYS**. However, to work with actual arrays in Python, you will need to import a library, such as the NumPy library.

Arrays are used to store multiple values in a single variable.

### Example
Create an array containing car names:
```python
cars = ["Ford", "Volvo", "BMW"]
```

## What is an Array?

An array is a special variable that can hold more than one value at a time.

For example, if you have a list of items (such as car names), storing each car in a single variable could look like this:
```python
car1 = "Ford"
car2 = "Volvo"
car3 = "BMW"
```
However, what if you want to loop through the cars and find a specific one? Or what if you had 300 cars instead of 3?

The solution is an **array**! An array can hold multiple values under a single name, and you can access these values by referring to their index number.

## Access the Elements of an Array

You refer to an array element by its index number.

### Example
Get the value of the first array item:
```python
x = cars[0]
```

### Example
Modify the value of the first array item:
```python
cars[0] = "Toyota"
```

## The Length of an Array

Use the `len()` method to return the length of an array (the number of elements in the array).

### Example
Return the number of elements in the cars array:
```python
x = len(cars)
```
**Note:** The length of an array is always one more than the highest array index.

## Looping Through Array Elements

You can use the `for` loop to iterate through all the elements in an array.

### Example
Print each item in the cars array:
```python
for x in cars:
  print(x)
```

## Adding Array Elements

You can use the `append()` method to add an element to an array.

### Example
Add one more element to the cars array:
```python
cars.append("Honda")
```

## Removing Array Elements

You can use the `pop()` method to remove an element from the array.

### Example
Delete the second element of the cars array:
```python
cars.pop(1)
```

You can also use the `remove()` method to remove an element from the array.

### Example
Delete the element with the value "Volvo":
```python
cars.remove("Volvo")
```
**Note:** The `remove()` method only removes the first occurrence of the specified value.

## Array Methods

Python has a set of built-in methods that you can use on lists/arrays:

| Method       | Description                                                                          |
|--------------|--------------------------------------------------------------------------------------|
| `append()`   | Adds an element at the end of the list                                              |
| `clear()`    | Removes all the elements from the list                                              |
| `copy()`     | Returns a copy of the list                                                         |
| `count()`    | Returns the number of elements with the specified value                            |
| `extend()`   | Adds the elements of a list (or any iterable) to the end of the current list        |
| `index()`    | Returns the index of the first element with the specified value                    |
| `insert()`   | Adds an element at the specified position                                           |
| `pop()`      | Removes the element at the specified position                                       |
| `remove()`   | Removes the first item with the specified value                                    |
| `reverse()`  | Reverses the order of the list                                                     |
| `sort()`     | Sorts the list                                                                     |

### Example Code for Array Methods

```python
# Initial list
cars = ["Ford", "Volvo", "BMW"]

# append()
cars.append("Honda")
print("After append:", cars)

# clear()
cars.clear()
print("After clear:", cars)

# Reset list
cars = ["Ford", "Volvo", "BMW"]

# copy()
cars_copy = cars.copy()
print("Copy of list:", cars_copy)

# count()
print("Count of 'Ford':", cars.count("Ford"))

# extend()
cars.extend(["Toyota", "Nissan"])
print("After extend:", cars)

# index()
print("Index of 'BMW':", cars.index("BMW"))

# insert()
cars.insert(1, "Kia")
print("After insert:", cars)

# pop()
cars.pop(1)
print("After pop:", cars)

# remove()
cars.remove("Volvo")
print("After remove:", cars)

# reverse()
cars.reverse()
print("After reverse:", cars)

# sort()
cars.sort()
print("After sort:", cars)
```

Task: Manage a Shopping List
Write a Python program to:

Create a list called shopping_list with the initial items: "Milk", "Bread", and "Eggs".
Add "Butter" to the list.
Remove "Bread" from the list.
Print the total number of items in the list.
Display all items in the list, one per line.
