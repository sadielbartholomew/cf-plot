.. _example2:

Example 2
*********


.. code-block:: python
   :caption: *TODO describe Example 2*
   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.con(f.subspace(time=15), blockfill=True, lines=False)


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_2.png
