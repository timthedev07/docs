Python super efficient word scramble finder
==================================================

Introduction
############

word scramble is a python package that looks for all possibilities given a scrambled word. The package would keep updating as python itself updates to higher versions.



Installation
############
If not already, `install pip <https://pip.pypa.io/en/stable/installing/>`_.

Install the package with ``pip`` or ``pip3`` ::

    pip install word-scramble


Usage
######

Search
************

.. code-block:: python

    from wsfinder import main
    # Need to provide the language
    finder = main.Finder("english")
    scrambled_words = [
        "taurdesta",
        "achwt",
        "ilane",
        "alger",
        ]
    res = {word:finder.find(word) for word in scrambled_words}
    print(res)

Output:

.. code-block:: python

    {
    'taurdesta': ['saturated'],
    'achwt': ['watch'],
    'ilane': ['liane', 'laine', 'elian', 'anile', 'aline', 'alien'],'alger': ['regal', 'large', 'lager', 'glare', 'elgar', 'argle'],
    }

