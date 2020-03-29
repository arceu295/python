\*args and \*\*kwargs
**********************

.. code-block:: python

    def my_func(*args, **kwargs):
        print(*args)
        print(**kwargs)

    my_func("Hello", "World", first = "f", second = "s")
    # => ("Hello", "World")
    # => {"first": "f", "second": "s"}

..

Using to call a function

.. code-block:: python

    def my_func(arg1, arg2, arg3): 
        print("arg1:", arg1) 
        print("arg2:", arg2) 
        print("arg3:", arg3) 
      
    args = ("v1", "v2", "v3") 
    my_func(*args) 
    
    kwargs = {"arg1": "v1", "arg2": "v2", "arg3": "v3"} 
    my_func(**kwargs)

..

Enumerate()
************

.. note::
    Syntax: enumerate(iterable, start=0)
..

.. code-block:: python

    str = "test"
    print(list(enumerate(str, 100)))
    # => [(100, 't'), (101, 'e'), (102, 's'), (103, 't')]

..
