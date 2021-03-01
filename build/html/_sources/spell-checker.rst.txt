Python Spell Checker - Faster than your blinking speed.
=======================================================

Introduction
############
The **spell checker** is a python package that can check your spelling. It supports 5 languages!
For someone who is considering interating the entire dictionary to find a single word, this package will save your life! (I mean so that you won't get carpal tunnel when coding the big boi, you might not get the joke, alright, whatever, nevermind...)

It contains the following languages:

- English
- German
- Spanish
- French
- Italian

Installation
############
If not already, `install pip <https://pip.pypa.io/en/stable/installing/>`_.

Install the package with ``pip`` or ``pip3`` ::

    pip install spell-checker


Usage
######

Example:
************

.. code-block:: python

    from speller3x.checker import Checker
    text = "The... ! quick browmn fox jumps-over the lazi doug"
    checker = Checker(text, "english")
    checker.check()

Output:

.. code-block:: python

    Total words: 9
    Number of misspelled words: 2
    Number of words in dictionary: 194433
    Misspelled words: ['browmn', 'lazi']
    Lookup time(s): 0.0005731582641601562

