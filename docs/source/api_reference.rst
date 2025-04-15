:orphan:

API Reference
*************


User-facing API
---------------

These functions *are* intended for user use.


.. toctree::
   :maxdepth: 2

   add_cyclic
   axes
   axes_plot
   calculate_levels
   cbar
   cf_var_name
   cf_var_name_titles
   check_well_formed
   con
   cscale
   ext_candidates
   find_dim_names
   find_pos_in_array
   find_z
   fix_floats
   gclose
   generate_titles
   gopen
   gpos
   gset
   irregular_window
   is_exe
   levs
   lineplot
   map_grid
   mapset
   max_ndecs_data
   ndecs
   orca_check
   pcon
   polar_regular_grid
   reset
   rgaxes
   setvars
   stipple
   stipple_points
   stream
   traj
   vect
   vloc

   
Internal API
------------

These functions *are not* intended for user use.

.. toctree::
   :maxdepth: 2

   _bfill
   _bfill_ugrid
   _cf_data_assign
   _check_data
   _cscale_get_map
   _dim_titles
   _gvals
   _map_title
   _mapaxis
   _plot_map_axes
   _process_color_scales
   _set_map
   _supscr
   _timeaxis


Deprecations
------------

These functions *are not* intended for user use and will be removed in the next
version. In most cases these have no use in the codebase as of v3.3.0.

.. toctree::
   :maxdepth: 2

   regrid

Note the functions ``compare_arrays`` and ``regression_tests`` (version 3.3.0
and earlier) related to testing only so have been moved out of the
functional codebase.
