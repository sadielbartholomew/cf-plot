.. _example36:

Example 36
**********


.. code-block:: python
   :caption: *TODO describe Example 36*
   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.mapset(proj="merc")

   cfp.con(f.subspace(time=15))


.. figure:: images/fig36.png
