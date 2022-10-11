=======================
Midnight Commander uadf
=======================

Midnight Commander extfs plugin for handling `pycatalog`_ databases.

Description
-----------

Upycatalog is an extfs plugin suitable for reading sqlite databases created by
`pycatalog`_ program, which is used for creating file list and collect some
metadata for the files from CD/DVD/BR discs or drives/directories.

It allows to list such archive and check metadata for every entry stored in it.

Requirements
------------

It requires:

* Python (tested on python 3.10)
* `pycatalog`_
* `extfslib`_


Installation
------------

* install `extfslib`_
* copy ``upycatalog`` to ``~/.local/share/mc/extfs.d/``
* add or change entry for files handle in ``~/.config/mc/mc.ext``::

    shell/i/.catalog
        Open=%cd %p/upycatalog://


License
=======

This software is licensed under 3-clause BSD license. See LICENSE file for
details.


.. _pycatalog: https://github.com/gryf/pygtktalog
.. _extfslib: https://github.com/gryf/mc_extfslib
