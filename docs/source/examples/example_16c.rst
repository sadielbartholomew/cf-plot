.. _example16c:

Example 16c
***********


.. code-block:: python
   :caption: *TODO describe Example 16c*
   f = cf.read(f"{self.data_dir}/ggap.nc")

   u = f[1].subspace(pressure=500)
   v = f[2].subspace(pressure=500)
   u = u.anchor("X", -180)
   v = v.anchor("X", -180)

   magnitude = (u**2 + v**2) ** 0.5
   mag = np.squeeze(magnitude.array)

   cfp.levs(0, 60, 5, extend="max")
   cfp.cscale("viridis", ncols=13)
   cfp.gopen()
   cfp.stream(u=u, v=v, density=2, color=mag)
   cfp.cbar(
       levs=cfp.plotvars.levels,
       position=[0.12, 0.12, 0.8, 0.02],
       title="Wind magnitude",
   )
   cfp.gclose()

.. figure:: images/fig16c.png
