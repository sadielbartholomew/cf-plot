.. _example16b:

Example 16b
-----------


.. code-block:: python
   :caption: *TODO describe Example 16b*

   f = cf.read(f"{self.data_dir}/ggap.nc")
   u = f[1].subspace(pressure=500)
   v = f[2].subspace(pressure=500)

   u = u.anchor("X", -180)
   v = v.anchor("X", -180)

   cfp.stream(u=u, v=v, density=2)


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_16b.png
