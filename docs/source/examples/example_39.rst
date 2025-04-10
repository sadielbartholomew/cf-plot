.. _example39:

Example 39: Basic track plotting
--------------------------------


.. code-block:: python
   :caption: A basic example of plotting a track i.e. trajectory

   f = cf.read(f"{self.data_dir}/ff_trs_pos.nc")[0]

   cfp.traj(f)


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_39.png
