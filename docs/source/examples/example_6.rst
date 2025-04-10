.. _example6:

Example 6: Latitude-pressure plot at set longitude
--------------------------------------------------


.. code-block:: python
   :caption: Making a plot for a given longitude value with latitude and
             pressure as the axes

   f = cf.read(f"{self.data_dir}/ggap.nc")[3]
 
   cfp.con(f.subspace(longitude=0))


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_6.png
