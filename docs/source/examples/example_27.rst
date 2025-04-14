.. _example27:

Example 27: Basic line plot
---------------------------


.. code-block:: python
   :caption: Making a basic line plot

   f = cf.read(f"cfplot_data/ggap.nc")[1]

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
