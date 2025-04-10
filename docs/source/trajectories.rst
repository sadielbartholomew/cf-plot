:orphan:

.. _trajectories:

Trajectories
************

Data stored in contiguous ragged array format can be plotted using cf-plot.


.. include:: examples/example_39.rst

This a plot of relative vorticity tracks is made in the cylindrical projection.


.. include:: examples/example_40.rst

.. include:: examples/example_41.rst

.. include:: examples/example_42a.rst

In this plot the tracks between 1979-12-01 and 1979-12-30 are selected and
labelled according intensity with a colour bar.


.. include:: examples/example_42b.rst

Selecting `legend_lines=True` plots lines only and colours them according
to the sum of the start and end point divided by two. This can be a
useful option when there are lots of trajectories.
