.. _example5:

Example 5: South Pole polar projection contour plot with bounding latitude
--------------------------------------------------------------------------


.. code-block:: python
   :caption: Changing the view area of a contour plot in the South Pole
             polar stereographic projection by setting the latitude limit to
             30 degrees south

   f = cf.read(f"cfplot_data/ggap.nc")[1]

   cfp.mapset(proj="spstere", boundinglat=-30, lon_0=180)

   cfp.con(f.subspace(pressure=500))


.. figure:: /../../cfplot/test/reference-example-images/ref_fig_5.png
