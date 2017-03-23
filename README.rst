node_vm2
========

.. image:: https://api.codacy.com/project/badge/Grade/fb30c7193b6b43cf818457e3ff23e60c
   :target: https://www.codacy.com/app/eight04/node_vm2?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=eight04/node_vm2&amp;utm_campaign=Badge_Grade

.. image:: https://readthedocs.org/projects/node-vm2/badge/?version=latest
   :target: http://node-vm2.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status

A Python 3 to Node.js + vm2 binding, helps you execute JavaScript safely.

Install
-------

You need Node.js

https://nodejs.org/

Install from pypi wheel.

.. code-block::

   pip install node_vm2

Also make sure you have ``node`` executable in ``PATH``, or you can specify the executable with environment variable ``NODE_EXECUTABLE``.

Additionally, you will need ``npm`` to build node_vm2 from source.

Usage
-----

Most of the APIs are compatible with `vm2 <https://github.com/patriksimek/vm2>`__.

.. code-block:: python

   from node_vm2 import VM
   
   with VM() as vm:
      result = vm.run("""
         var sum = 0, i;
         for (i = 0; i < 10; i++) sum += i;
         sum;
      """)
      print(result)
      
API reference
-------------

http://node-vm2.readthedocs.io/

Changelog
---------

-  Next

   -  First release
   