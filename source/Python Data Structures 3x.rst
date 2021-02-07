Python Data Structures 3x
==================================================

Introduction
############
The data_structures3x is a python package with 3 of the most basic data structures.
The package would keep updating as python itself updates to higher versions.

It contains the following data structures:

- Binary Tree
- Linked List
- Hash table


Installation
############
If not already, `install pip <https://pip.pypa.io/en/stable/installing/>`_.

Install the package with ``pip`` or ``pip3`` ::

    pip install data-structures3x


Usage
######

Binary Tree
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

    from algorithms3x.sort import bubble_sort, selection_sort
    bubble_sort([4, 2, 5, 3, 1])
    selection_sort([c, e, d, b, f, a])

Output:

.. code-block:: python

    [1, 2, 3, 4, 5]
    [a, b, c, d, e, f]
