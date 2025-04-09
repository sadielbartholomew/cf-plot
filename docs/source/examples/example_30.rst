.. _example30:

Example 30
**********


.. code-block:: python
   :caption: *TODO describe Example 30*

   tol = cf.RTOL(1e-5)

   fl = cf.read(f"{self.data_dir}/ggap.nc")
   f = fl[1]

   u = f.collapse("X: mean")
   u1 = u.subspace(Y=cf.isclose(-61.12099075))
   u2 = u.subspace(Y=cf.isclose(0.56074494))

   g = fl[0]
   t = g.collapse("X: mean")
   t1 = t.subspace(Y=cf.isclose(-61.12099075))
   t2 = t.subspace(Y=cf.isclose(0.56074494))

   cfp.gopen()
   cfp.gset(-30, 30, 1000, 0)
   cfp.lineplot(u1, color="r")
   cfp.lineplot(u2, color="r")
   cfp.gset(190, 300, 1000, 0, twiny=True)
   cfp.lineplot(t1, color="b")
   cfp.lineplot(t2, color="b")
   cfp.gclose()


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_30.png
