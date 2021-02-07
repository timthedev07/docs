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
******************

Initialize and print the binary tree:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The Node object contains 3 attributes:

- val (The actual value of the node, could be an integer, string, ect or even )
- left (A pointer to the one of its child)
- right (A pointer to the other one of its child)

.. code-block:: python

    # Import the required packages
    from dt_structures3x.binarytree import Node as Node
    # Creates the tree, the Node class initialization taks 3 parameters
    # One is #1 is its value, #2
    tree  = Node(3, Node(1, Node(1), Node(5)), Node(4, Node(9), Node(2, Node(6))))
    # Finally prints the tree
    tree.print_tree()

Output:

.. code-block:: bash

      _3_
     /   \
     1   4_
    / \ /  \
    1 5 9   2
        /
        6

Get Children
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To get the children of a node, use:

.. code-block:: python

    foo = Node("O")
    bar = Node("O", foo)
    baz = Node("O", foo, bar)
    print(f"Foo's children: {foo.get_children()}")
    print(f"Bar's children: {bar.get_children()}")
    print(f"Baz's children: {baz.get_children()}")

Output:

.. code-block:: python

    "Foo's children: (None, None)"
    "Bar's children: (<Node object at 0x7fc24f88ad30>, None)"
    "Baz's children: (<Node object at 0x7fc24f88ad30>, <Node object at 0x7fc24f88ad90>)"

Notice that the node foo, just has a value, but does not have any children, so the return value is a set of two Nones.
Whereas bar, has foo on its left, but nothing on the right, so the right attribute is None.
Finally, baz have both the two children filled with either foo and bar, so it returs a set of them.

Linked list
***********
``
