.. _example40:

Example 40: Tracks in the polar stereographic projection
--------------------------------------------------------


.. code-block:: python
   :caption: Plotting tracks i.e. trajectories on the Northern polar
             stereographic projection

   f = cf.read(f"{self.data_dir}/ff_trs_pos.nc")[0]

   cfp.mapset(proj="npstere")

   cfp.traj(f)


.. figure:: ../../../cfplot/test/reference-example-images/ref_fig_40.png
