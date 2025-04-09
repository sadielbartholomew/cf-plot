.. _example31:

Example 31
**********


.. code-block:: python
   :caption: *TODO describe Example 31*
   f = cf.read(f"{self.data_dir}/ukcp_rcm_test.nc")[0]

   cfp.mapset(proj="UKCP", resolution="50m")
   cfp.levs(-3, 7, 0.5)
   cfp.setvars(grid_x_spacing=1, grid_y_spacing=1)

   cfp.con(f, lines=False)

.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_31.png
