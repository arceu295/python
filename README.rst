***************
README FILE 00
***************

README FILE 01
***************

README FILE 02
###############

README FILE 03
==============

Lambda operator
****************

.. code-block:: python

    sum = lambda x, y : x + y

..

map() function
***************
Python 3, map() returns an iterator
map() applies the function `func` to all elements of the sequence seq (e.g. a list)

.. code-block:: python

    r = map(func, seq)

    def f(T):
        return ((float(9)/5)*T + 32)
    def c(T):
        return (float(5)/9)*(T-32)
    temperatures = (37, 38, 39)
    F = map(f, temperatures)
    C = map(c, temperatures)
    list(map(f, temperatures))
..

map() can be applied to more than one list (same length)
If one list has fewer elements than the others, map will stop when the shortest list has been consumed

.. code-block:: python

    a = [1, 2]
    b = [10, 11]
    list(map(lambda x, y : x + y, a, b))
    # => [11, 13]

..

Check if an object is an integer or not:
x = 200
print(isinstance(x, int))

Some values are False
empty values, such as (), [], {}, "", the number 0 and the the value None.

Filtering
**********

.. code-block:: python

    numbers = [0, 1, 1, 2, 3, 5, 8]
    list(filter(lambda x: x % 2, numbers))

..

List comprehension
*******************

.. code-block:: python

    colours = [ "red", "green", "yellow", "blue" ]
    things = [ "house", "car", "tree" ]
    [(x,y) for x in colours for y in things]

    # => [('red', 'house'), ('red', 'car'), ('red', 'tree'), ...]

..

Refer this for more details `(list comprehension) <https://www.python-course.eu/python3_list_comprehension.php>`__
