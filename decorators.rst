***********
Decorators
***********

Decorators are very powerful and useful tool in Python since it allows programmers
to modify the behavior of function of class. Decorators allow us to wrap another function
in order to extend the behavior of wrapped function, without permanently modifying it.
Functions are taken as the argument into another function and then
called inside the wrapper function.
This is also called **metaprogramming**

.. code-block:: python

    def my_decorator(x):
        def inner_func(x):
            return cal(x)
        return inner_func

    @my_decorator
    def cal(x):
        return x + 3

..

Using a class as a decorator
*****************************

.. code-block:: python

    class decorator2:
    
        def __init__(self, f):
            self.f = f
        
        def __call__(self):
            print("Decorating", self.f.__name__)
            self.f()

    @decorator2
    def foo():
        print("inside foo()")

    foo()

..

Refer to these documents:
https://www.programiz.com/python-programming/decorator
https://www.geeksforgeeks.org/decorators-in-python/
https://realpython.com/primer-on-python-decorators/
