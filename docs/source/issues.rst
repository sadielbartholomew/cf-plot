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
we will end up asking you this first):

* The version of the software and the environment in which you are
  encountering an issue, by sharing the output of
  ``cf.environment(paths=False)``.

* A description of the issue with, if possible:

  * what you expected to happen and what did actually happen;
  * the steps needed to reproduce it (ideally from copying the original
    code you ran which produced the issue);
  * the data you were using when the issue occurred, either as a
    data file to send or by sharing the output of ``f.dump()`` for the
    field ``f`` which displays the issue (or the same for multiple fields
    if applicable), as close as possible to the
    code line where the issue manifests.

* Outputs showcasing the issue, if available:
    
  * any traceback information;
  * any plots that emerge (plus correct plots to compare this to, if you have
    those from using different software or environments).
