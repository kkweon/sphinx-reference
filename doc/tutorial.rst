Example: tutorial.rst -- The trianglelib tutorial
==================================================

    .. index:: single: Euclid

    *“There is no royal road to geometry.”* — Euclid

Summary
-------

This module makes triangle processing fun! The beginner will enjoy how the :mod:`~trianglelib.utils` module lets
you get started quickly.


>>> from trianglelib import utils
>>> utils.is_isosceles(5, 5, 7)
True

But fancier programs can use the :class:`~trianglelib.shape.Triangle` class to create an actual triangle *object* upon
which they can then perform lots of operations. For example, consider this Python program:

.. testcode::

    from trianglelib.shape import Triangle
    t = Triangle(5, 5, 5)
    print("Equilateral? ", t.is_equilateral())
    print("Isosceles? ", t.is_isosceles())

Since methods like :meth:`~trianglelib.utils.is_equilateral` return boolean values, this program will produce the following output:


.. testoutput::

    Equilateral? True
    Isosceles? False

Read :doc:`guide` to learn more !


..  warning::

    This module only handles three-sided polygons;
    five-sided figures are right-out.
