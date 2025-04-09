.. _example18:

Example 18
**********


.. code-block:: python
   :caption: *TODO describe Example 18*
   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   g = f.subspace(time=15)

   cfp.gopen()
   cfp.cscale("magma")
   cfp.mapset(proj="npstere")
   cfp.con(g)
   cfp.stipple(f=g, min=265, max=295, size=100, color="#00ff00")
   cfp.gclose()


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_18.png
