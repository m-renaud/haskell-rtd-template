A
=

.. highlight:: haskell

TODO: A one paragraph description of what this module does/provides at a high
level.


::

    -- TODO: Data declarations of any key constructs you need to work with this
    -- module.
    data A x y = ...

TODO: Any important things to keep in mind when using stuff in this module. A
few examples are included below.

.. IMPORTANT::
   ``A`` relies on the type ``x`` having instances of the ``Eq`` and
   ``Ord`` typeclass for its internal representation. These are already defined
   for builtin types, and if you are using your own data type you can use the
   `deriving
   <https://en.wikibooks.org/wiki/Haskell/Classes_and_types#Deriving>`_
   mechanism.


All of these implementations are *immutable* which means that any update
functions do not modify the A that you passed in, they creates a new A. In
order to keep the changes you need to assign it to a new variable. For example::

    let a1 = A.make "a" 1
    let a2 = A.frobnicate a1
    print a1
    > A (Just "a") (Just 1)
    print a2
    > A (Just "a") (Just 200)


Short Example
-------------

TODO: 5-10 short examples of using ``A``.

The following GHCi session shows some of the basic ``A`` functionality::

    import qualified Data.A as A

    let a1 = A.make "a" 1

    ...

TODO: Tips that apply when using this module but aren't necessary. This could
include useful language extensions. We've included an example taken from the
``containers`` docs.

.. TIP:: You can use the `OverloadedLists
	 <https://ghc.haskell.org/trac/ghc/wiki/OverloadedLists>`_ extension so
	 you don't need to write ``fromList [1, 2, 3]`` everywhere; instead you
	 can just write ``[1, 2, 3]`` and if the function is expecting a map it
	 will be converted automatically! The code here will continue to use
	 ``fromList`` for clarity though.


Importing A
-----------

TODO: How to import your module (example paragraph for qualified imports below)

When using ``A`` in a Haskell source file you should always use a ``qualified``
import because these modules export names that clash with the standard Prelude
(you can import the type constructor on its own though!). You can always import
any specific identifiers you want unqualified. Most of the time, that will
include the type constructor (``A``).

::

    import Data.A (A)
    import qualified Data.A as A


Common API Functions
--------------------

TODO: Any applicable tips/notes about the module. For example, noting difference
between Strict/NonStrict versions of data structures.


Construction and Conversion
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Create an empty A
"""""""""""""""""

::

    A.empty :: A x y
    A.empty = ...

:haddock_short:`/Data.A#empty` creates an ``A`` with no data.

::

    A.empty
    > A Nothing Nothing

Create an A with data
"""""""""""""""""""""

::

    A.make :: x -> y -> A x y
    A.make x y = ...

:haddock_short:`/Data.A#make` creates an ``A`` with a valid ``x`` and ``y``.

::

    A.make "a" 1
    > A (Just "a") (Just 1)

    A.make "containers" ["base"]
    > A (Just "containers") (Just ["base"])

TODO: Other ways to construct an A
""""""""""""""""""""""""""""""""""

Querying
^^^^^^^^

TODO: Lookup/read-only operations.


Modification
^^^^^^^^^^^^

TODO: Modifying operations


Serialization
-------------

TODO: How to serialize an ``A`` (if that's a reasonable operation)


Performance
-----------

TODO: Link to more information on performance of the module.


Looking for more?
-----------------

TODO: Links to follow-up reading.

Didn't find what you're looking for? This tutorial only covered the most common
``A`` functions, for a full list of functions see the
:haddock_short:`/Data.A#A` API documentation.
