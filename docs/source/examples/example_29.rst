.. _example29:

Example 29
**********


.. code-block:: python
   :caption: *TODO describe Example 29*
   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   temp = f.subspace(time=cf.wi(cf.dt("1900-01-01"), cf.dt("1980-01-01")))
   temp_annual = temp.collapse("T: mean", group=cf.Y())
   temp_annual_global = temp_annual.collapse("area: mean", weights="area")
   temp_annual_global.Units -= 273.15

   cfp.lineplot(
       temp_annual_global,
       title="Global average annual temperature",
       color="blue",
   )


.. figure:: images/fig29.png
