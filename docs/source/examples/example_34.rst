.. _example34:

Example 34: cropping the Lambert Conformal Conic (LCC) projection
-----------------------------------------------------------------


.. code-block:: python
   :caption: Plotting using the Lambert Conformal Conic (LCC) projection
             and cropping the displayed boundaries.

   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.mapset(proj="lcc", lonmin=-50, lonmax=50, latmin=20, latmax=85)

   cfp.con(f.subspace(time=15))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_34.png
