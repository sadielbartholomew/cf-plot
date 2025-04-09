.. _example3:

Example 3
*********


.. code-block:: python
   :caption: *TODO describe Example 3*
   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.mapset(lonmin=-15, lonmax=3, latmin=48, latmax=60)
   cfp.levs(min=265, max=285, step=1)

   cfp.con(f.subspace(time=15))


.. figure:: images/fig3.png
