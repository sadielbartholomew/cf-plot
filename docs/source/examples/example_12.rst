.. _example12:

Example 12
**********


.. code-block:: python
   :caption: *TODO describe Example 12*
   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.cscale("plasma")

   cfp.con(f.subspace(latitude=0), lines=0)


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_12.png
