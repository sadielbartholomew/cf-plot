.. _example8:

Example 8: Latitude against log of pressure over longitude zonal mean
---------------------------------------------------------------------


.. code-block:: python
   :caption: Making a semilog plot with latitude and the log of the
             pressure as the axes for a zonal mean over longitude

   f = cf.read(f"cfplot_data/ggap.nc")[1]

   cfp.con(f.collapse("mean", "longitude"), ylog=1)


.. figure:: /../../cfplot/test/reference-example-images/ref_fig_8.png
