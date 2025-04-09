.. _example5:

Example 5
*********


.. code-block:: python
   :caption: *TODO describe Example 5*

   f = cf.read(f"{self.data_dir}/ggap.nc")[1]

   cfp.mapset(proj="spstere", boundinglat=-30, lon_0=180)

   cfp.con(f.subspace(pressure=500))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_5.png
