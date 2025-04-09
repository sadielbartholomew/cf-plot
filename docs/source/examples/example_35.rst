.. _example35:

Example 35
**********


.. code-block:: python
   :caption: *TODO describe Example 35*

   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.mapset(proj="moll")

   cfp.con(f.subspace(time=15))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_35.png
