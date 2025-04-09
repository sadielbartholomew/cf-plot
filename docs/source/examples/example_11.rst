.. _example11:

Example 11
**********


.. code-block:: python
   :caption: *TODO describe Example 11*
   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.gset(-30, 30, "1960-1-1", "1980-1-1")
   cfp.levs(min=280, max=305, step=1)
   cfp.cscale("plasma")

   cfp.con(f.subspace(longitude=0), lines=0)


.. figure:: images/fig11.png
