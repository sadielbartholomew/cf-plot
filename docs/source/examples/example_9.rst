.. _example9:

Example 9
*********


.. code-block:: python
   :caption: *TODO describe Example 9*
   f = cf.read(f"{self.data_dir}/ggap.nc")[0]

   cfp.con(f.collapse("mean", "latitude"))


.. figure:: images/fig9.png
