.. _Clothoid:

Clothoid
========

Type: Composite Entity

Clothoid curves are approximated by :ref:`POLYLINE`.

For an explanation of clothoid curves see Wikipedia:

http://en.wikipedia.org/wiki/Clothoid

.. method:: DXFEngine.clothoid(start=(0, 0), rotation=0., length=1., paramA=1.0, mirror="", segments=100, **kwargs)

    :param start: insert point as 2D points (float-tuples)
    :param float rotation: in degrees
    :param loat length: length of curve in drawing units
    :param float paramA: clothoid parameter A
    :param str mirror: ``'x'`` for mirror curve about x-axis,
      ``'y'`` for mirror curve about y-axis,
      ``'xy'`` for mirror curve about x- and y-axis
    :param int segments: count of line segments for polyline approximation
    :param str linetype: linetype name, if not defined = `BYLAYER`
    :param str layer: layer name
    :param int color: range [1..255], 0 = `BYBLOCK`, 256 = `BYLAYER`

Example
-------

.. literalinclude:: ../../examples/clothoid.py
   :lines: 20-38

.. image:: clothoid.png

