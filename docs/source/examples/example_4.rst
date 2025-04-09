.. _example4:

Example 4
*********


.. code-block:: python
   :caption: *TODO describe Example 4*

   f = cf.read(f"{self.data_dir}/ggap.nc")[1]

   cfp.mapset(proj="npstere")

   cfp.con(f.subspace(pressure=500))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_4.png
