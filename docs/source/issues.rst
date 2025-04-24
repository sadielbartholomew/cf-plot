:orphan:

Support and contributing
************************

Ways to contact us
------------------

If you find an apparent issue with cf-plot or have a question or feature
request etc., the *preferred* method of contact is via the
`GitHub Issue Tracker for the cf-plot repository <https://github.com/NCAS-CMS/cf-plot/issues>`_.
You will need a GitHub account to do this, but it is free to
`sign up <https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github>`_.

If you don't want to use the Issue Tracker then you can also either:

* send an email to Sadie Bartholomew at `sadie.bartholomew@ncas.ac.uk` (or
  if based on the University of Reading campus you may find her in-office
  HP113, noting she often works from home);
* post on the `NCAS-CMS Helpdesk <https://cms-helpdesk.ncas.ac.uk/>`_.

If you are reporting an issue, please follow the guidelines below so that
we have enough information to attempt to recreate the problem.


Issue reporting guidelines
--------------------------

If you find a problem with cf-plot, please ensure you provide all of the
information below so we can investigate properly as soon as possible (else
we will end up asking you this first).

Please email with the following:

|   (i) the cf-python and cf-plot version numbers used:
|       print('cf-python version', cf.__version__)
|       print('cf-plot version', cfp.__version__)
|   (i) A short piece of code showing the problem
|   (iii) The data needed to make the plot


i.e. if you make a plot using:

::

   f=cf.read('cfplot_data/ggap.nc')[1]
   cfp.con(f.collapse('mean','longitude'))

Then use cf-python to write out the data used to make the plot and then send the data (newfile.nc) and plotting line to me.

::

   f=cf.read('cfplot_data/ggap.nc')[1]
   g=f.collapse('mean','longitude')
   cf.write(g, 'newfile.nc')


Send the data (newfile.nc) and plotting lines as per below example to me:

::

   g=cf.read('newfile.nc')
   cfp.con(g)


If you are using arrays of data use numpy to write out the relevant data:

::

   np.save('lons.npy', lons)
   np.save('lats.npy', lats)
   np.save('field.npy', field)

