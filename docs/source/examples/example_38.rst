.. _example38:

Example 38
**********


.. code-block:: python
   :caption: *TODO describe Example 38*
   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.mapset(proj="robin")

   cfp.con(f.subspace(time=15))


.. figure:: images/fig38.png
