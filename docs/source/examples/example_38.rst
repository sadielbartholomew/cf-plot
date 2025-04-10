.. _example38:

Example 38: Robinson projection
-------------------------------


.. code-block:: python
   :caption: Plotting using the Robinson projection

   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.mapset(proj="robin")

   cfp.con(f.subspace(time=15))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_38.png
