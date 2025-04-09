.. _example24c:

Example 24c
***********


.. code-block:: python
   :caption: *TODO describe Example 24c*

   f = cf.read("cfplot_data/lfric_initial.nc")
   pot = f.select_by_identity("air_potential_temperature")[0]

   g = pot[0, :]
   cfp.con(g, lines=False)


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_24c.png
