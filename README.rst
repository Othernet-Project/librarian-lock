==============
librarian-lock
==============

Provides functions to enforce a global lock over the entire application on all
routes, until it is released.

Installation
------------

The component has the following dependencies:

- librarian-core_

To enable this component, add it to the list of components in librarian_'s
`config.ini` file, e.g.::

    [app]
    +components =
        librarian_lock

Configuration
-------------


``lock.file``
    Path to the lock file, which is used as a flag indicating whether the lock
    is active or not. Example::

        [lock]
        file = /path/to/lock.file

.. _librarian: https://github.com/Outernet-Project/librarian
.. _librarian-core: https://github.com/Outernet-Project/librarian-core
