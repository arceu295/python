*************
Dictionaries
*************

Can't access an element of the dictionary by a number

.. code-block: python

    dic = {}
    dic["key"] = "value";

    dic2 = {'b': 1, 'b': 2} # => {'b': 2}
    k in dic2 # check k exists in dictionary dic2 or not
    dic2.pop("key") # remove element and return the corresponding value
    # raise a KeyError if key doesn't exist
    dic2.pop("key", "default value") # return default value if key doesn't exist

..

popitem() method
*****************

+ Remove and return a 2-tuple
+ Raise KeyError if dictionary is empty

Check existence of a key
*************************

.. code-block:: python

    if "key" in dictionary: pass # do something
    dictionary.get("key") # not raising an error, return None
    dictionary.get("key", "default_value")

..

copy() method
**************

.. code-block:: python

    w = works.copy() # this copy is shallow
    w.clear() # => {}

..

update() method
****************

Merge the keys and values of one dictionary into another, overwriting values of the same key

.. code-block:: python

    dict1 = {"key": "value"}
    dict2.update(dict1)

..

Iterating over a dictionary
****************************

.. code-block:: python

    for key in d: # for key in d.keys()
        pass
    for value in d.values():
        pass
    for k, v in d.items():
        pass

..

Creating list from dictionary
******************************

.. code-block:: python

    list(d.items())
    list(d.keys())
    list(d.values())

..

Turn list into dictionary
**************************

.. code-block:: python

    list01 = ["a1", "a2"]
    list02 = ["b1", "b2"]
    zip_list = list(zip(list01, list02)) # list of tuples
    dic = dict(zip_list)
    # or
    dic = dict(zip(list01, list02))

..
