.. _example15:

Example 15: Polar projection vector plot
----------------------------------------


.. code-block:: python
   :caption: Making a vector plot on a North Pole polar projection

   f = cf.read(f"cfplot_data/ggap.nc")
   u = f[1]
   v = f[2]
   u = u.subspace(Z=500)
   v = v.subspace(Z=500)

   cfp.mapset(proj="npstere")

   cfp.gopen(columns=2)
   cfp.vect(
       u=u,
       v=v,
       key_length=10,
       scale=100,
       stride=4,
       title="Polar plot using data grid",
   )
   cfp.gpos(2)
   cfp.vect(
       u=u,
       v=v,
       key_length=10,
       scale=100,
       pts=40,
       title="Polar plot with regular point distribution",
   )
   cfp.gclose()


.. figure:: /../../cfplot/test/reference-example-images/ref_fig_15.png
