Quick Reference
===============

.. note::

    Your note should consist of one or more paragraphs, all indented
    so that they clearly belong to the note and not to the text or
    directive that follows.

    Many other directives are also supported, including: warning,
    versionadded, versionchanged, seealso, deprecated, rubric,
    centered, hlist, glossary, productionlist


.. code-block:: python

    import numpy as np
    print("Hello World")


.. literalinclude:: ../trianglelib/shape.py
    :lines: 10-20
    :emphasize-lines: 15,16


.. module:: httplib

.. class:: Request
    
    Zero or more paragraph for class

    .. method:: send()

        Describtion of `send()` method


    .. attribute:: url

        Descripbtion of url attributes


    Many more members are possible than just method and attribute,
    and non-Python languages are supported too; see the Sphinx docs
    for more possibilities!


.. testcode::
    
    print 'The doctest extension supports code without >>> prompts!'

.. testoutput::
    
    The doctest extension supports code without >>> prompts!

.. custom-label:
.. index:: single: paragraph, targeted paragraph, indexed paragraph

This paragraph can be targeted with :ref:`custom-label`, and will also
be the :index:`target` of several index entries!

.. index:: pair: copper, wire

This paragraph will be listed in the index under both “wire, copper”
and “copper, wire.” See the Sphinx documentation for even more complex
ways of building index entries.

Many kinds of cross-reference can be used inside of a paragraph:

:ref:`custom-label`

:class:`~module.class`

:doc:`quick_reference`

:meth:`~trianglelib.shape.triangle.area()`

:mod:`~trianglelib.shape` 

:att: `~trianglelib.shape.triangle.a`

(See the Sphinx “Inline Markup” chapter for MANY more examples!)
