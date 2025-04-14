.. _example23b:

Example 23b: Overlaying vectors over a rotated pole data plot
-------------------------------------------------------------


.. code-block:: python
   :caption: *TODO describe Example 23 Other*

   f = cf.read(
       f"cfplot_data/20160601-05T0000Z_INCOMPASS_km4p4_uv_RH_500.nc"
   )
   cfp.mapset(50, 100, 5, 35)
   cfp.levs(0, 90, 15, extend="neither")

   cfp.gopen()
   cfp.con(f[0], lines=False)
   cfp.vect(u=f[1], v=f[2], stride=40, key_length=10)
   cfp.gclose()


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_23b.png
