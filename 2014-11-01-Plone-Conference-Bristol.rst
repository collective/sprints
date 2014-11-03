================
Plone Conference
================

**Lots** of sprints going on during the Plone main conference.


Dates and location
==================

When: from November 1st to November 2nd.

Where: Thistle Grand Hotel, Bristol, the conference venue


Participants
============

Too many to list!


Links
=====

Conference main page: http://2014.ploneconf.org


Topics
======

Group the sprint topics by sections so is easier for everyone to get an overview and find their spot.


CI sprint
---------

- Move jenkins jobs configurations to `Jenkins Job Builder <http://ci.openstack.org/jenkins-job-builder/>`_

  What: https://trello.com/b/U14dgKcN/plone-testing-ci-sprint-bristol-2014
  Who: @gforcada, mpeeters
  Code: https://github.com/plone/jenkins.plone.org/tree/jenkins-job-builder
  Status: not finished

Basic migration of jobs are done, http://test.jenkins.plone.org can run all tests (including robot ones).
There's some manual setup still being done.


Controlpanels
-------------

- convert to z3c.form
- convert to use registry
- move out of plone.app.controlpanel and into Products.CMFPlone

  What: https://titanpad.com/0fyCHL1o6P
  Who: @ibi @MrTango @khink
  Status: in progress

Plan: https://titanpad.com/0fyCHL1o6P
Copy the controlpanels into Products.CMFPlone one by one.
Start with tests.
Then copy code from the ``plip10359-z3cform``-branch of p.a.c
Then check for commits on p.a.c master that we need to cherry-pick.

Cherry-picking p.a.c master
~~~~~~~~~~~~~~~~~~~~~~~~~~~

We list only the commits on master that we deemed necessary to cherry-pick.
We started on the first commit on the branch and moved forward in time from there.

7da32a (2012-04-10): cherry-picked
a18d4a (2012-05-07): cherry-picked
4dcd48 (2012-05-14): manually cherry-picked

collective.sendaspdf
--------------------

Who: @neajj
What: Long-delayed tweak to make sendaspdf use the latest wkhtmltopdf 
Status: Pull request submitted:
    https://github.com/zestsoftware/collective.sendaspdf/pull/18
    

Ecosystem KGS
-------------
Who: Roel Bruggink
What: Ecosystem wide KGS per Plone version
Status: Nothing done.


TTW addon installation
----------------------
Who: Roel Bruggink, Alexander Loechel, Giacomo Spettoli
What: Allow installing Plone addons TTW
Status: Going to do hangout. Alexander has a basic implementation.


Documentation
--------------

participants: Paul Roeland, Roel Bruggink, Sébastien & Coen

* styleguide (tech + english) -- only started, will be finished next week
* move all magic from plone/documentation to plone/papyrus -- done
* get versioning for papyrus to actually work -- done
* prepare for use by intranetconsortium and others -- can be used, with some guidance
* work on tickets -- three tickets closed
* fix styleguide for plone.api -- not finished
* kill Grok references!! (Sébastien & Coen) -- done!
* meta-doc: document how to do documentation for multiple branches (cherrypick by hand? If we do, that also has to be a documented process) -- update: yes, cherry-picking by hand is the way; we know how to do it but has to be documented better
* prefer plone.api in docs -- not done; this could be a nice "one at a time" task for future sprints
* prepare for real-life launch of 3.3 docs, so we gracefully retire old stuff to it -- ready for launch
