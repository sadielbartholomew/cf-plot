.. _example7:

Example 7
*********


.. code-block:: python
   :caption: *TODO describe Example 7*

   f = cf.read(f"{self.data_dir}/ggap.nc")[1]

   cfp.con(f.collapse("mean", "longitude"))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_7.png
