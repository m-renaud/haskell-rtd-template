``TODO_PACKAGE_NAME`` Introduction
==================================

The ``TODO_PACKAGE_NAME`` package provides TODO.

More description of package.

Once you know the basics, or if you're looking for a specific function, you can
head over to the :haddock:`TODO_PACKAGE_NAME` Haddocks to check out the full API
documentation!

Provided Components
-------------------

- :doc:`moduleA`: support for A

.. NOTE::
   You'll need ``PACKAGE >= 0.1.2`` for a few of the examples. See
   `Version Requirements`_ for info on how to check which version you have and
   how to upgrade.


Related Packages
----------------

- :haddock:`TODO_RELATED_PACKAGE_1` - frobnicates the A's from this package


Looking for more resources?
---------------------------

If you've worked your way through the documentation here and you're looking for
more examples or tutorials you should check out:

TODO:

- Links to other documentation
- Links to other tutorials

.. _installing:

Installing and using the ``TODO_PACKAGE_NAME`` package
------------------------------------------------------

Version Requirements
^^^^^^^^^^^^^^^^^^^^

For some of the examples you'll need ``PACKAGE >= 0.1.2``.

You can check to see which version you have installed with:

TODO: Instructions for how to see what version you have.



Importing modules
^^^^^^^^^^^^^^^^^

All of the modules in ``TODO_PACKAGE_NAME`` should be imported ``qualified``
(TODO: maybe they shouldn't be) since they use names that conflict with the
standard Prelude.

::

    import qualified TodoPackage.A as A


In GHCi
^^^^^^^

Start the GHCi `REPL
<https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop>`_ with
``ghci`` or ``stack ghci``. Once the REPL is loaded import the modules you want
to use and you're good to go!


In a `Cabal <https://cabal.readthedocs.io>`_ or `Stack <https://www.haskellstack.org>`_ project
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Add ``TODO_PACKAGE_NAME`` to the ``build-depends:`` stanza for your library,
executable, or test-suite::

    library
        build-depends:
	    base >= 4.3 && < 5,
	    TODO_PACKAGE_NAME >= 0.1.2 && < 0.2

and ``import`` any modules you need in your Haskell source files.
