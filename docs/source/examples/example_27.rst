.. _example27:

Example 27
----------


.. code-block:: python
   :caption: *TODO describe Example 27*

   f = cf.read(f"{self.data_dir}/ggap.nc")[1]

   g = f.collapse("X: mean")

   cfp.gopen()
   cfp.lineplot(
       g.subspace(pressure=100),
       marker="o",
       color="blue",
       title="Zonal mean zonal wind at 100mb",
   )
   cfp.gclose()


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_27.png
