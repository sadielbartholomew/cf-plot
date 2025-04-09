.. _example22other:

Example 22 Other
****************


.. code-block:: python
   :caption: *TODO describe Example 22 Other*
   f = cf.read(f"{self.data_dir}/rgp.nc")[0]

   cfp.cscale("plasma")
   cfp.mapset(proj="rotated")

   cfp.con(f)


.. figure:: images/fig22other.png
