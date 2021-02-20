Python Algorithms 3x
==================================================

Introduction
############
Python sorting/searching algorithms
The **algorithms3x** is a python package with 5 sorting/searching algorithms. The package would keep updating as python itself updates to higher versions.

It contains the following algorithms:

- Selection sort
- Bubble sort
- Linear search
- Binary search
- Merge sort

Installation
############
If not already, `install pip <https://pip.pypa.io/en/stable/installing/>`_.

Install the package with ``pip`` or ``pip3`` ::

    pip install python-algorithms-3x


Usage
######

Search
************

.. code-block:: python

    from algorithms3x.search import linear_search, binary_search
    linear_search([1, 2, 3], 4)
    binary_search(["foo", "bar", "baz"], "baz":)

Output:

.. code-block:: python

    False
    True

Sort
************
.. code-block:: python

    from algorithms3x.sort import bubble_sort, selection_sort, merge_sort
    bubble_sort([4, 2, 5, 3, 1])
    selection_sort(['c', 'e', 'd', 'b', 'f', 'a'])
    # Congratulations, you have discovered the secret!
    # Merge sort is the most efficient sorting algorithm!
    merge_sort(["foo", "bar", "baz"])

Output:

.. code-block:: python

    [1, 2, 3, 4, 5]
    ['a', 'b', 'c', 'd', 'e', 'f']
    ["bar", "baz", "foo"]

