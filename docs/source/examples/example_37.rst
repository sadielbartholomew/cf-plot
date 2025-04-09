.. _example37:

Example 37
**********


.. code-block:: python
   :caption: *TODO describe Example 37*

   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.mapset(proj="ortho")

   cfp.con(f.subspace(time=15))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_37.png
