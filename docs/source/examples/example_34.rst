.. _example34:

Example 34
**********


.. code-block:: python
   :caption: *TODO describe Example 34*
   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.mapset(proj="lcc", lonmin=-50, lonmax=50, latmin=20, latmax=85)

   cfp.con(f.subspace(time=15))


.. figure:: images/fig34.png
