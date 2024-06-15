.. test-sphinx-publish documentation master file, created by
   sphinx-quickstart on Tue May 28 21:49:56 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to test-sphinx-publish's documentation!
===============================================

This is some additional text.

- Some bullet points
- Some bullet points
- Some bullet points

This is Great!
--------------
Or maybe it's just so-so.

.. code-block::
    :caption: An example of code-block options
    :linenos:
    :emphasize-lines: 2,4,5

    @pytest.fixture
    def date_input():
        now = datetime.datetime.now()
        current_date_string = f"{now.year}-{now.month}-{now.day}"
        return current_date_string

You can also control code highlighting. The default mode is to
highlight Python code but don't give an error if a language is
not recognized:

Some Python code:

::

   def main():
      print("Hello, world!")

Followed by some C code

::

   void main() {
      printf("Hello, world!");
   }

----------

If we insert the directive:

.. code-block::

    .. highlight:: C

Then C code will be highlighted.

.. highlight:: C

Some Python code:

::

   def main():
      print("Hello, world!")

Followed by some C code

::

   void main() {
      printf("Hello, world!");
   }

----------

You can also turn off code highlighting completely by using ``none``:

.. code-block::

    .. highlight:: none

.. highlight:: none

Some Python code:

::

   def main():
      print("Hello, world!")

Followed by some C code

::

   void main() {
      printf("Hello, world!");
   }

----------

And then go back to default highlighting (Python with silent failures).

.. code-block::

    .. highlight:: default

.. highlight:: default

And some plain text.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   About <about>


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
