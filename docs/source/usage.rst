Usage
=====

.. _installation:

Installation
------------

To use SaphyCore, first install it using pip:

.. code-block:: console

   (.venv) $ pip install SaphyCore

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``SaphyCore.get_random_ingredients()`` function:

.. autofunction:: SaphyCore.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`SaphyCore.get_random_ingredients`
will raise an exception.

.. autoexception:: SaphyCore.InvalidKindError

For example:

>>> import SaphyCore
>>> SaphyCore.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

