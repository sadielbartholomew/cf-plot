.. _example7:

Example 7: Latitude-pressure plot over zonal mean
-------------------------------------------------


.. code-block:: python
   :caption: Making a plot with latitude and pressure as the axes
             for a zonal mean (mean over longitude)

   f = cf.read(f"cfplot_data/ggap.nc")[1]

   cfp.con(f.collapse("mean", "longitude"))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_7.png
