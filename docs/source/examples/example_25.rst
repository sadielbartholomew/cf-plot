.. _example25:

Example 25
**********


.. code-block:: python
   :caption: *TODO describe Example 25*
   f = cf.read("cfplot_data/orca2.nc")

   # Get an Orca grid and flatten the arrays
   lons = f.select_by_identity("ncvar%longitude")[0]
   lats = f.select_by_identity("ncvar%latitude")[0]
   temp = f.select_by_identity("ncvar%sst")[0]

   lons.flatten(inplace=True)
   lats.flatten(inplace=True)
   temp.flatten(inplace=True)

   # Mask NaN else the plot will fail with:
   # Traceback (most recent call last):
   #   File "/home/slb93/git-repos/cf-plot/cfplot/test/test_examples.py", line 1030, in test_example_unstructured_orca_1
   #     cfp.con(f=temp, x=lons.array, y=lats.array, ptype=1)
   #   File "/home/slb93/git-repos/cf-plot/cfplot/cfplot.py", line 3297, in con
   #     _cf_data_assign(f, colorbar_title, verbose=verbose)
   #   File "/home/slb93/git-repos/cf-plot/cfplot/cfplot.py", line 1379, in _cf_data_assign
   #     myz = find_z(f)
   #           ^^^^^^^^^
   #   File "/home/slb93/git-repos/cf-plot/cfplot/cfplot.py", line 10748, in find_z
   #     mycoords = find_dim_names(f)
   #                ^^^^^^^^^^^^^^^^^
   #   File "/home/slb93/git-repos/cf-plot/cfplot/cfplot.py", line 10720, in find_dim_names
   #     if field.coord(coords[i]).X:
   #                    ~~~~~~^^^
   # IndexError: list index out of range
   # TODO apply this at relevant place in code, instead
   temp = np.ma.masked_invalid(temp)

   cfp.con(f=temp, x=lons.array, y=lats.array, ptype=1)


.. figure:: images/fig25.png
