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

Initialize and print the binary tree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The Node object contains 3 attributes:

- val (The actual value of the node, could be an integer, string, ect or even )
- left (A pointer to one of its child)
- right (A pointer to the other one of its child)

.. code-block:: python

    # Import the required packages
    from dt_structures3x.binarytree import Node as Node
    # Creates the tree, the Node class initialization taks 3 parameters
    # val, right, and left
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

Get children
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

    Foo's children: (None, None)
    Bar's children: (<Node object at 0x7fc24f88ad30>, None)
    Baz's children: (<Node object at 0x7fc24f88ad30>, <Node object at 0x7fc24f88ad90>)

Notice that the node foo, just has a value, but does not have any children, so the return value is a set of two Nones.
Whereas bar, has foo on its left, but nothing on the right, so the right attribute is None.
Finally, baz have both the two children filled with either foo and bar, so it returs a set of them.


Linked list
***********

A linked list in our case, is implemented using a object that is somehow similar to a node
It uses a class called ``Item``

An Item has two attributes, value and pointer, where the value is the same as before, and the pointer is the next node in the linked list.

Initialize and print the linked list.
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

  from dt_structures3x.linkedlist import Item
  # linked list
  root = Item(10)
  root.appendChild(Item(17), Item(19))
  root.display()

Output:

.. code-block:: shell

  10 -> 17 -> 19

Next node
^^^^^^^^^^^^^^


If you go to the next node using the getNextNode() method:

.. code-block:: python
  next = root.getNextNode()
  print(next)

We get:

.. code-block:: python

  17

Because the value of the next node is 17

Now if we try to display the linked list:

.. code-block:: python

  next.display()

We get:

.. code-block:: shell

  Linked list:
  17 -> 19

Append children
^^^^^^^^^^^^^^^^

We can append element(s) to the linkedlist using the method appendChild().
If the current item's pointer is none, it would set the pointer to the new node,
but if there is one, it would go all the way to the end of the linked list and append the item.

See the example below:

.. code-block:: python

  <code>

  root.appendChild(Item("Foo"))
  root.display()

The output would be:

.. code-block:: shell

  Linked list:
  10 -> 17 -> 19 -> Foo
