.. _example13:

Example 13: Basic vector plot
-----------------------------


.. code-block:: python
   :caption: Making a basic vector plot

   f = cf.read(f"{self.data_dir}/ggap.nc")

   u = f[1].subspace(pressure=500)
   v = f[3].subspace(pressure=500)

   cfp.vect(u=u, v=v, key_length=10, scale=100, stride=5)


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_13.png
