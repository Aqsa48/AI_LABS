
# Python Classes and Objects

## Python Classes/Objects
- Python is an object-oriented programming language.
- Almost everything in Python is an object, with its properties and methods.
- A **Class** is like an object constructor, or a "blueprint" for creating objects.

---

## Create a Class
To create a class, use the keyword `class`:

### Example
Create a class named `MyClass`, with a property named `x`:

```python
class MyClass:
    x = 5
```

---

## Create an Object
Now we can use the class named `MyClass` to create objects:

### Example
Create an object named `p1`, and print the value of `x`:

```python
p1 = MyClass()
print(p1.x)
```

---

## The `__init__()` Function
The examples above are classes and objects in their simplest form, and are not really useful in real-life applications.

To understand the meaning of classes, we have to understand the built-in `__init__()` function:
- All classes have a function called `__init__()`, which is executed when the class is initiated.
- Use the `__init__()` function to assign values to object properties or perform other operations when the object is created.

### Example
Create a class named `Person`, and use the `__init__()` function to assign values for `name` and `age`:

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

p1 = Person("John", 36)

print(p1.name)
print(p1.age)
```

---

## Tasks

1. **Create a Custom Class**
   - Create a class named `Car` with properties `brand` and `model_year`.
   - Use the `__init__()` function to initialize these properties.
   - Create an object of the `Car` class and print its properties.

2. **Add a Method to the Class**
   - Extend the `Person` class to include a method named `greet` that prints `"Hello, my name is [name]!"`.
   - Call the method using the `Person` object.

3. **Explore Object Properties**
   - Add a new property `gender` to the `Person` class.
   - Create an object and access the new property.

4. **Modify Object Properties**
   - Update the `age` of the `Person` object and print the updated age.

5. **Practice with Multiple Objects**
   - Create multiple objects of the `Car` class with different values for `brand` and `model_year`.
   - Print details of each object.

6. **Write a Real-Life Class Example**
   - Design a class that represents a **Book** with properties like `title`, `author`, and `price`.
   - Include a method `book_info()` that prints all the book details.
