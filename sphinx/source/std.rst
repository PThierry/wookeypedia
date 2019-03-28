EwoK Standard library
=====================

.. image:: img/ewok.png
   :height: 250px
   :width: 250 px
   :scale: 100 %
   :alt: ewok icon
   :align: center


.. contents::

Introduction
------------

EwoK standard library is the EwoK microkernel userspace small libc implementation, hosting:

   * The userspace syscall part
   * The various embedded-specific utility functions (such as registers manipulation helpers)
   * Some various basic functions for string manipulation, etc.


libstd API
----------

The libstd API is decomposed in various and small foot-print specific components.

   * libstream: the I/O pretty printing API, such as printf API
   * libstring: string manipulation API
   * libarpa: endianess manipulation for protocol stacks
   * libembed: various embedded-related API, including data storage API and various others
   * liballoc: the memory allocator

libstd **does not aim** to be a POSIX compliant library. Nevertheless, for functions that behave
like POSIX ones, libstd try to keep the POSIX conformant API.

Each component is described bellow.

.. toctree::
  :maxdepth: 2

  EwoK libstd's libstring <std/libstring>
  EwoK libstd's libembed <std/libembed>
  EwoK libstd's libstream <std/libstream>
  EwoK libstd's libarpa <std/libarpa>
  EwoK libstd API FAQ <std/faq>

