*********************
cf-plot documentation
*********************

**cf-plot: code-light plotting for earth science and aligned research**

.. Define external links to use in the docs here

.. _matplotlib:  https://matplotlib.org/
.. _Cartopy:     https://scitools.org.uk/cartopy/docs/latest/
.. _cf-python:   https://ncas-cms.github.io/cf-python/
.. _NCAS-CMS:    https://cms.ncas.ac.uk/index.html
.. _NCAS:        https://ncas.ac.uk/

.. TODO update these to internal links once can go through and reference each page
.. _gallery page:         https://ncas-cms.github.io/cf-plot/build/gallery.html
.. _installation page:    https://ncas-cms.github.io/cf-plot/build/download.html
.. _guidance page here:   https://ncas-cms.github.io/cf-plot/build/issues.html

########
Overview
########

.. image:: images/cf_gallery_image.png
   :scale: 75%
   :target: gallery.html

cf-plot allows you to produce and customise publication-quality contour, vector,
line and more plots with the power of Python, `matplotlib`_,
`Cartopy`_ and `cf-python`_ in as few lines of code as possible.

It is designed to be a useful visualisation tool for environmental, earth and
aligned sciences, for example to facilitate climate and meteorological research.
cf-plot is developed and maintained by the `NCAS-CMS`_ group, part of `NCAS`_.


###################
Brief Demonstration
###################

In as little as four lines of Python including imports and file reading, using
cf-plot you can for example produce a contour plot showing a 2D subspace of a
netCDF dataset:

.. code-block:: python

   import cf
   import cfplot as cfp
   f = cf.read('<dataset name>.nc')[0]  # picks out a read-in field of the dataset
   cfp.con(f.subspace(time=<chosen time value>))  # creates a contour plot of the field at that time value


################
Examples Gallery
################

A gallery of outputs made with cf-plot, showcasing a range of plotting
possibilities with links to relevant documentation pages and to example code,
can be found on the `gallery page`_, as also linked to the static image
of the gallery at the to of this page.


############
Installation
############

To install cf-plot with its required dependencies, you can use pip:

.. code-block:: bash

   pip install cf-python cf-plot

or you can use conda (or similar package managers such as mamba) as follows
(or equivalent):

.. code-block:: bash

   conda install -c ncas -c conda-forge cf-python cf-plot udunits2

More detail about installation is provided on the
`installation page`_ of the documentation.

############
Contributing
############

Everyone is welcome to contribute to cf-plot in the form of bug reports,
documentation, code, design proposals, and more.

Contributing guidelines will be added to the repository shortly.

###############################################
Help: Issues, Questions, Feature Requests, etc.
###############################################

For any queries, see the `guidance page here`_.


#########################
Contents of documentation
#########################

.. toctree::
   :maxdepth: 1

   add_cyclic
   advanced
   all-examples
   axes_plot
   axes
   bfill
   calculate_levels
   cbar
   cf_data_assign
   cf_var_name
   check_data
   colour_scales
   compare_arrays
   compare_images
   con
   cscale_get_map
   cscale
   cylindrical
   download
   find_pos_in_array
   fix_floats
   gallery
   gclose
   gopen
   gpos
   graphs
   gset
   gvals
   hovmuller
   index
   internal_routines
   issues
   levs
   license
   lineplot
   mapaxis
   mapset
   map_title
   max_ndecs_data
   multiple_plots
   ndecs
   older_documentation
   pcon
   plot_map_axes
   polar_regular_grid
   polar
   pressure
   process_color_scales
   projections
   regression_tests
   regrid
   reset
   rgaxes
   rotated_pole
   routines
   set_map
   setvars
   stipple_plots
   stipple_points
   stipple
   stream
   supscr
   timeaxis
   training
   trajectories
   traj
   unstructured
   user_defined
   user_guide
   vectors
   vect
   version_1.3
   version_1.5
   version_1.6
   version_1.7
   version_1.8
   version_1.9
   version_2.0
   version_2.1
   version_2.2
   version_2.3
   version_2.4
   version_3.0
   version_3.1
   version_3.2
   version_3.3
   version3_changes
   versions
   vloc
   wrf


----

################
Index and search
################

* :ref:`genindex`
* :ref:`Search <search>`

