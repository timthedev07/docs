Python And-Or-Not Concept Helper for beginners
==================================================

Introduction
############
The **and-or-not** is a python package that teaches you the basic concepts of the logical operators(and, or and not). The package would keep updating as python itself updates to higher versions.

Contains the following logical operators:

- And
- Or
- Not


Installation
############

If not already, `install pip <https://pip.pypa.io/en/stable/installing/>`_.

Install the package with ``pip`` or ``pip3`` ::

    pip install and-or-not


Usage
######

**ATTENTION**

*Beginners don't have to worry about the syntax, you can simply copy and paste the following code and replace the expressions.
PLEASE NOTE THAT IT ONLY SUPPORTS == AND != OPERATOR JUST TO GET YOU A SENSE OF LOGICAL OPERATORS(cos i'm lazy:) )*

And
************

Initialize and Display
^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

  from and_or_not.main import And # Import the package
  # Initialize object with 3 expressions
  myAnd = And("1 != 4", "FOO == Bar", "baz != BAZ")
  # Display the expression in a pythonic way
  myAnd.display()

Output:

.. code-block:: python

    1 != 4 and FOO == Bar and baz != BAZ

Print out the explanation
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

  # Print out the explanation
  myAnd.explain()

The output would be a bunch of explanation, install to see more.

Return the final result (If familiar with return values)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

  print(myAnd.result())

.. code-block:: bash

  False

Or
****

Initialize and Display
^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

  from and_or_not.main import Or # Import the package
  # Initialize object with 3 expressions
  myOr = Or("1 != 4", "FOO == Bar", "baz != BAZ")
  # Display the expression in a pythonic way
  myOr.display()

Output:

.. code-block:: python

    1 != 4 and FOO == Bar and baz != BAZ

Print out the explanation
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

  # Print out the explanation
  myOr.explain()

The output would be a bunch of explanation, install to see more.

Return the final result (If familiar with return values)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

  print(myOr.result())

.. code-block:: bash

  True


Not
****

Initialize and show the expression
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: py

  # Print out the expression in a pythonic way
  myAnd.show()

Explanation
^^^^^^^^^^^^^^

.. code-block:: py

  # Print out the explanation
  myAnd.explain()
