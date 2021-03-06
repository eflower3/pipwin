===============================
pipwin
===============================

[*UNMAINTAINED*]
^^^^^^^^^^^^^^

**There is an issue with wheel urls. Download wheels directly from the website http://www.lfd.uci.edu/~gohlke/pythonlibs/ till the issue is resolved. Also PRs are accepted.**


.. image:: https://img.shields.io/pypi/v/pipwin.svg?style=flat-square
    :target: https://pypi.python.org/pypi/pipwin/
    :alt: Latest Version
    
.. image:: https://img.shields.io/pypi/dm/pipwin.svg?style=flat-square
    :target: https://pypi.python.org/pypi/pipwin/
    :alt: Downloads
  
.. image:: https://img.shields.io/pypi/l/pipwin.svg?style=flat-square
    :target: https://pypi.python.org/pypi/pipwin/
    :alt: License

**pipwin** is a complementary tool for **pip** on Windows.
**pipwin** installs unofficial python package binaries for windows provided by Christoph Gohlke here `http://www.lfd.uci.edu/~gohlke/pythonlibs/ <http://www.lfd.uci.edu/~gohlke/pythonlibs/>`_

**Version 0.2.X changes the structure of cache file. Make sure to run `pipwin refresh` if updated.**

QuickStart
^^^^^^^^^^

.. code-block::

   >> pip install pipwin
   >> pipwin search cv

   Did you mean any of these ?

     * cvxopt
     * opencv-python
     * abcview
     * cvxpy

   >> pipwin install opencv-python


Details
^^^^^^^

- On first run, **pipwin** builds a cache of available package list in ``~/.pipwin``.

- You can force a cache rebuild using : ``pipwin refresh``

- List all available packages : ``pipwin list``

- Search packages : ``pipwin search <partial_name/name>``

- Install packages : ``pipwin install <package>``

- Download only (to ~/pipwin) : ``pipwin download <package>``

- Install from pipwin requirements file : ``pipwin install -file requirements.txt``

- Download only from pipwin requirements file : ``pipwin download -file requirements.txt``

- Uninstall packages (Can directly use **pip** for this) : ``pipwin uninstall <package>``

**Free software: BSD license**
