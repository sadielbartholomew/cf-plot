Installation
************

Is cf-plot already installed?
=============================

cf-plot my already be avaiable to you, if you have access to a some tier of
HPC system. For example (though note these commands may be out of date and
will be checked for updates in the near future):

.. code-block:: console
   :caption: On JASMIN

   $ export PATH=/home/users/ajh/anaconda3/bin:$PATH
   $ ln -s /home/users/ajh/cfplot_data ~


.. code-block:: console
   :caption: On ARCHER

   $ export PATH=/home/n02/n02/ajh/anaconda3/bin:$PATH
   $ export QT_XCB_NO_XI2=true
   $ ln -s /home/n02/n02/ajh/cfplot_data ~


.. code-block:: console
   :caption: On Reading Academic Computing Cluster (RACC)
             
   $ module load ncas_anaconda3
   $ ln -s /share/apps/NCAS/cfplot_data ~


To install cf-plot
==================

Linux and Mac OSX
#################

cf-plot is supported for Linux and Mac. There are multiple ways to install
from such systems, as detailed below.

Via conda
+++++++++

To install cf-plot on a Linux PC or Mac, get access to the ``conda``
command through an
`Anaconda or 'miniconda' distribution (etc.) <https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html>`_
and run:

.. code-block:: console
   :caption: Installing cf-plot and its dependencies with ``conda``

   $ conda install -c conda-forge cf-python cf-plot udunits2
   $ conda install -c conda-forge "esmpy>=8.7.0"  # if you need to use regridding functionality


The first line installs cf-python and cf-plot (``udunits`` is a dependency
of cf-python). The second line is optional and installs ``esmpy``,
together which cf-python uses for regridding data.


Via PyPI
++++++++

You can use `pip` to install from `PyPI <https://pypi.org/>`_:

.. code-block:: console
   :caption: Installing cf-plot and its dependencies with ``pip``
             
   $ pip install cf-python cf-plot


If you are upgrading the version of cf-python or cf-plot to the latest
ones then add the ``--upgrade`` after the install above. A specific
version can be installed using pip install ``cf-plot==3.3.0`` for example.


From source via GitHub
++++++++++++++++++++++

.. code-block:: console
   :caption: Installing cf-plot from source via ``git`` and GitHub
             
   $ git clone https://github.com/NCAS-CMS/cf-plot.git
   $ cd cf-plot
   $ python setup.py install  # or 'pip install -e .'

Note you will need to ensure all dependencies are avialable, such as
cf-python. See below for guidance on this.


Windows
#######

Only Linux and Mac operating systems are directly supported, but if you
wish to use Windows there are a couple of options whereby you can run
Linux from Windows and use cf-plot that way:

1) Install the Microsoft Windows Subsystem for Linux (WSL). Once this is
   working install cf-python and cf-plot as per the Linux instructions above.

2) Installing a Linux Virtual Machine. Installation instructions and a
   Mint Linux Virtual Machine are available at
   http://gws-access.ceda.ac.uk/public/ncas_climate/ajh/data_analysis_tools/VM.


Dependencies
############

cf-plot has the following dependencies:

* `cf-python <https://ncas-cms.github.io/cf-python/installation.html>`_, ``'cf-python >= 3.9.0'``
* `Matplotlib <https://matplotlib.org/stable/install/index.html>`_, ``'matplotlib >=3.1.0'``
* `SciPy <https://scipy.org/install/>`_, ``'scipy >= 1.4.0'``
* `Cartopy <https://scitools.org.uk/cartopy/docs/latest/installing.html>`_, ``'cartopy >= 0.17.0'``

With package/environment managers such as ``conda`` and ``pip`` you
can install all dependencies
along with the package, but you can also find information on installing
these dependencies separately on the links in the list above to the relevant
documentation pages of each dependency library.


Sample data sets
################

Sample data sets, which are used for instance in the examples throughout
this documentation, are
`available for download generally from this link <http://gws-access.ceda.ac.uk/public/ncas_climate/ajh/data_analysis_tools/cfplot_data.tar>`_.

If you have access to JASMIN or RACC, they are also available already in
directories named ``cfplot_data`` in each location,
which can be linked as follows:

.. code-block:: console
   :caption: Locations of sample datasets on JASMIN
             
   $ ln -s /home/users/ajh/cfplot_data ~


.. code-block:: console
   :caption: Locations of sample datasets on the Reading Academic Computing Cluster (RACC)
             
   $ ln -s /share/apps/NCAS/cfplot_data ~
