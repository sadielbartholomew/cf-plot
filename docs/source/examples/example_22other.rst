.. _example22other:

Example 22 Other
****************


.. code-block:: python
   :caption: *TODO describe Example 22 Other*
   f = cf.read(f"{self.data_dir}/rgp.nc")[0]

   cfp.cscale("plasma")
   cfp.mapset(proj="rotated")

   cfp.con(f)


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_22other.png
