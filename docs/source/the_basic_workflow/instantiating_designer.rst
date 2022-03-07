..  _instantiating_a_designer:
Instantiating a Designer
########################
A typical first step in a Pydex script is to create an instance of a Pydex designer:

..  sourcecode:: python

    designer = Designer()

In more exotic scripts and/or applications, you may also instantiate multiple designers:

..  sourcecode:: python

    designer_1 = Designer()
    designer_2 = Designer()
    designer_3 = Designer()
    ...
This is relevant, for example, when setting up Pydex to use 'multiprocessing_'.

..  _multiprocessing: https://docs.python.org/3/library/multiprocessing.html
