.. _example21other:

Example 21 Other: Plot of rotated pole data
-------------------------------------------


.. code-block:: python
   :caption: Making a plot of data defined on a rotated pole coordinate
             system

   f = cf.read(f"{self.data_dir}/rgp.nc")[0]

   cfp.cscale("plasma")

   cfp.con(f)

.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_21other.png
