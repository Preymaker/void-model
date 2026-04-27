.. _installing:

**********
Installing
**********

.. highlight:: bash

.. note::

    Using :term:`Virtualenv` is recommended when evaluating or running locally.

Installation is simple with `poetry <https://python-poetry.org/>`__::

    poetry install

.. _installing/source:

Installing from source
======================

You can also install manually from the source for more control. First obtain a
copy of the source by either downloading the `zipball
<https://github.com/Preymaker/void-model/archive/main.zip>`_
or cloning the public repository::

    git clone git@github.com:Preymaker/void-model.git

Then you can build and install the package into your current Python
environment::

    poetry install

Alternatively, just build locally and manage yourself::

    poetry build

.. _installing/source/doc:

Building documentation from source
----------------------------------

Then you can build the documentation with the command::

    poetry run sphinx-build -b html doc build/doc/html

View the result in your browser at::

    file:///path/to/void-model/build/doc/html/index.html

.. _installing/source/test:

Running tests against the source
--------------------------------

Then run the tests as follows::

    poetry run pytest

You can also generate a coverage report when running tests::

    poetry run pytest --cov --cov-report=html

View the generated report at::

    file:///path/to/void-model/htmlcov/index.html

