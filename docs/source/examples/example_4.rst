.. _example4:

Example 4: North Pole polar stereographic projection contour plot
-----------------------------------------------------------------


.. code-block:: python
   :caption: Plotting a contour plot in the North Pole polar
             stereographic projection

   f = cf.read(f"cfplot_data/ggap.nc")[1]

   cfp.mapset(proj="npstere")

   cfp.con(f.subspace(pressure=500))


.. figure:: /../../cfplot/test/reference-example-images/ref_fig_4.png
