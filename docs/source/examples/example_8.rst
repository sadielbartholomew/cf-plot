.. _example8:

Example 8
*********


.. code-block:: python
   :caption: *TODO describe Example 8*
   f = cf.read(f"{self.data_dir}/ggap.nc")[1]

   cfp.con(f.collapse("mean", "longitude"), ylog=1)


.. figure:: images/fig8.png
