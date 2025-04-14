.. _example9:

Example 9: Longitude-pressure plot over latitude mean
-----------------------------------------------------


.. code-block:: python
   :caption: Making a plot with longitude and pressure as the axes
             for a mean over latitude

   f = cf.read(f"cfplot_data/ggap.nc")[0]

   cfp.con(f.collapse("mean", "latitude"))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_9.png
