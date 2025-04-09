.. _example32:

Example 32
**********


.. code-block:: python
   :caption: *TODO describe Example 32*
   f = cf.read(f"{self.data_dir}/ukcp_rcm_test.nc")[0]

   cfp.mapset(proj="UKCP", resolution="50m")
   cfp.levs(-3, 7, 0.5)
   cfp.setvars(grid_colour="grey")

   cfp.con(
       f,
       lines=False,
       blockfill=True,
       # Centered over UK region with spacing of 1 each
       xticks=np.arange(14) - 11,
       yticks=np.arange(13) + 49,
   )


.. figure:: images/fig32.png
