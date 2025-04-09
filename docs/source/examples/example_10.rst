.. _example10:

Example 10
**********


.. code-block:: python
   :caption: *TODO describe Example 10*

   f = cf.read(f"{self.data_dir}/tas_A1.nc")[0]

   cfp.cscale("plasma")

   cfp.con(f.subspace(longitude=0), lines=0)


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_10.png
