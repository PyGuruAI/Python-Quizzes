# Correct Answers for Python Quizzes
Video Sources: For more insightful and educational content, check out our videos at https://www.youtube.com/@pyguruai

## Python Quiz 0001
Are the following statements valid in Python 3?

a, b = 0 ** 3, 0 / 3 <br>
print(a, b) <br>

a) Yes<br>
b) No

**The correct answer is a) Yes**

The Python statement a, b = 0 ** 3, 0 / 3 is valid because it uses tuple unpacking to assign values. 0 ** 3 is 0 (since 0 to any power is 0), and 0 / 3 is also 0 (since 0 divided by any number is 0). Thus, a and b both get assigned the value 0.

## Python Quiz 0002
In Python, which letter is used to represent imaginary numbers?

a) i<br>
b) j<br>
c) k<br>
d) x

**The correct answer is b) j**

In Python, the letter j is used to represent the imaginary unit (traditionally denoted as i in mathematics) due to a convention in electrical engineering. In electrical engineering, i often represents current, so j is used instead to avoid confusion. This convention was adopted in Python for complex numbers.

## Python Quiz 0003
In Python, 6 % 10 is 6. What's the output of following code snippet?
```python
print (6 % -10)
```

a) -6<br>
b) -4<br>

**The correct answer is b) -4**

In Python 3, the percentage symbol "%" is used as the modulo operator.
a % b = a −(b * ⌊a / b​⌋)
Note, ⌊a / b​⌋ is the floor division operation, which gives the largest integer less than or equal to the division result. ⌊6 / -10​⌋ is −1 (since the largest integer less than −0.6 is −1).
Plugging these into the equation:
6 −(−10 * −1) = 6 − 10 = −4

## Python Quiz 0004
In Python, a set can contain duplicate items.<br>
Please select 'True' if you think the statement is correct, or 'False' if it is incorrect.

a) True<br>
b) False<br>

**The correct answer is b) False**

In Python, a set is a collection type that is unordered and mutable. One of the key characteristics of a set is that it does not allow duplicate elements.<br>
```python
# Creating a set with duplicate items
my_set = {1, 2, 3, 2, 4, 1}
print(my_set) # Output will be {1, 2, 3, 4}
```

## Python Quiz 0005
Is there a way in Python to delete an element from a tuple?

a) Yes<br>
b) No<br>

**The correct answer is b) No**

Tuples in Python are immutable, which means you can't change their elements once they're created. However, you can work around this by converting the tuple to a list, removing the element, and then converting it back to a tuple.

## Python Quiz 0006
What would be the result of evaluating the following Python code?<br>
```python
my_dict = {"a": 1, "b": 2}
x = my_dict.keys()
my_dict["c"] = 3
print(x)
```

a) dict_keys(['a', 'b'])<br>
b) ['a', 'b']<br>
c) dict_keys(['a', 'b', 'c'])<br>
d) ['a', 'b', 'c']<br>

**The correct answer is c) dict_keys(['a', 'b', 'c'])**

In Python, when you call the .keys() method on a dictionary, it doesn't return a static list of keys. Instead, it returns a view object that displays the keys of the dictionary. This view object reflects any changes made to the dictionary.


## Python Quiz 0007
Do you know which command correctly lists all installed Python packages?

a) pip list<br>
b) pip --list<br>

**The correct answer is a) pip list**

Note: pip list and pip freeze provide information about installed packages, pip list is more for human-readable output, and pip freeze is designed for generating machine-readable requirements files.
ex.
```
root@localhost:~# pip list
Package    Version
------------- -------
ephem     4.1.5
geographiclib 2.0
geopy     2.4.1
pip      23.3.2
pytz     2023.4
setuptools  69.0.3
wheel     0.42.0

root@localhost:~# pip freeze
ephem==4.1.5
geographiclib==2.0
geopy==2.4.1
pytz==2023.4

root@localhost:~# pip freeze > requirements.txt

root@localhost:~# cat requirements.txt 
ephem==4.1.5
geographiclib==2.0
geopy==2.4.1
pytz==2023.4

```

`pip list` is more for human-readable output.<br>
`pip freeze` is designed for generating machine-readable requirements files.<br>
`!pip list` is a command that you would typically use in a Jupyter Notebook to list all installed Python packages. <br>


## Python Quiz 0008
What is the output of following Python code?

```python
print([1, 2, 3] + [4, 5, 6])
```

a) [5, 7, 9]<br>
b) [1, 2, 3, 4, 5, 6]<br>

**The correct answer is b) [1, 2, 3, 4, 5, 6]**

In Python, the + operator when used with lists performs list concatenation. This means it joins the two lists end-to-end. So, when you use [1, 2, 3] + [4, 5, 6], Python doesn't add the elements together numerically, but instead, it creates a new list that is the combination of the two lists.

Here's a breakdown of how it works:

You start with two lists: [1, 2, 3] and [4, 5, 6].
The + operator joins these lists, placing the elements of the second list directly after the elements of the first list.
So, the output of print([1, 2, 3] + [4, 5, 6]) is indeed option b) [1, 2, 3, 4, 5, 6].


## Python Quiz 0009
What's the output of this Python code?

```
a = True <= False
print(a)
```

a) 0<br>
b) 1<br>
c) False<br>
d) True<br>

**The correct answer is c) False**

In Python, the Boolean values True and False can also be understood as 1 and 0 respectively. So when you see True <= False, it's akin to evaluating 1 <= 0.

Now, let's evaluate the expression:

1 <= 0: This is asking, "Is 1 less than or equal to 0?"
The answer is clearly no, because 1 is greater than 0. Therefore, this expression is False.
When we assign this result to a, we get a = False.

So, when print(a) is executed, it prints False.

That's why the correct answer is C) False. It's a nifty example of how Python handles Boolean values and comparisons! 🐍✨

## Python Quiz 0010
Which Python code correctly calculates and prints the sum of two numbers?

a) `print(sum([5, 5]))`<br>
b) `print(sum(5, 5))`<br>

**The correct answer is a) `print(sum([5, 5]))`**

Option a) print(sum([5, 5])): This is the correct way to use the sum() function in Python. sum() takes an iterable (like a list) as an argument. Here, [5, 5] is a list containing two elements, both 5. sum([5, 5]) correctly adds up these elements, resulting in 10, and print() then prints this result.

Option b) print(sum(5, 5)): This is incorrect because the sum() function does not accept individual numbers as separate arguments. It expects an iterable (like a list, tuple, etc.) as the first argument and optionally, a starting point as the second argument (which is not used here). Hence, this code will throw a TypeError.


## Python Quiz 0011
What is the output of following Python code?<br>
print(bool("False"))

a) `True`<br>
b) `False`<br>
c) `1`<br>
d) `o`<br>

**The correct answer is a) `True`**

This is because in Python, a non-empty string is considered "truthy," and when passed to the bool() function, it returns True. So, bool("False") results in True.



