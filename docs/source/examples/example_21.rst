.. _example21:

Example 21
**********


.. code-block:: python
   :caption: *TODO describe Example 21*

   f = cf.read(f"{self.data_dir}/Geostropic_Adjustment.nc")[0]

   cfp.con(
       f.subspace[9],
       title="test data",
       xticks=np.arange(5) * 100000 + 100000,
       yticks=np.arange(7) * 2000 + 2000,
       xlabel="x-axis",
       ylabel="z-axis",
   )


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_21.png
