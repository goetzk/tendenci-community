.. contents::

==================
Tendenci community
==================

Every now and then the topic of community comes up in discussions around `Tendenci`_ and there is a general agreement it would be good to see more external contribution - a sentiment we probably all agree with.

Despite that Tendenci's parent company (`Tendenci (corp)`_ from here on) has struggled to build a growing community of regular contributors.

.. _Tendenci: https://github.com/tendenci/tendenci/
.. _Tendenci (corp): https://www.tendenci.com/

To try and expose areas I (@goetzk) - and others - believe should be addressed, this document has been put together to try and outline issues experienced by the community. At the same time we try to offer solutions to the problems discussed in the hope that they will lead to greater input from the developer community and make Tendenci a more attractive project to participate in.

While some of these steps will result in short term increases in effort (for example set up) or medium term effort (maintenance) it is felt the effort should pay for itself by easing contribution for potential developers and productivity for instance administrators.



Documentation is fragmented
===========================

The concern
-----------

Tendenci has a lot of documentation but it is spread far and wide. Officially, documentation can be found in `help files`_ on the corporate website and `ReadTheDocs`_. Unofficially documentation also ends up in GitHub issue discussions, the forum (now defunct) and other locations.

.. _help files: https://www.tendenci.com/help-files/
.. _ReadTheDocs: https://tendenci.readthedocs.org/en/latest/index.html

Problem outline
---------------

I believe the split between the two official sources of documentation is one reason that searching for Tendenci help can be very hit and miss (its docs often don't come up in searches when @goetzk is looking) and having documentation split up like this has a couple of drawbacks which affect use, but also hinder contribution. Importantly:

* Effort required to find the documentation (which location is it in?)
* Contribution consistency (how is it edited)
* Different editing permissions and review process for each documentation source (who can edit?).

Proposed solution
-----------------

Enabling greater collaboration in the official help files would allow consolidating all user facing documentation there. readthedocs could then be used exclusively for development related topics.


Tendenci (corp) only documentation
==================================

The concern
------------

Lots of documentation is on the Tendenci (corp) website and is not editable to casual contributors (presumably only available to Tendenci (corp) staff). Some of the documentation is correct, comprehensive and current. Some of it is irrelevant and wrong. Some of it sits in the middle and is good, but needs an update.

I (@goetzk) will cite my recent PRs supplying documentation for Stripe integration ("`Mention recurring payments`_" and "`Expand recurring payments documentation`_") as an example of working around the lack of editing ability. If I was able to edit the documentation those PRs would have been able to add new information directly to the help files, saving my time, the Tendenci developers time, and future users.

.. _Mention recurring payments: https://github.com/tendenci/tendenci/pull/645
.. _Expand recurring payments documentation: https://github.com/tendenci/tendenci/pull/652


As an example of the problematic nature of the Tendenci (corp) only pages I reported this issue in 2015 which is still unfixed:
 * The `developers page`_ has a number of broken links. [...]  Github Newsfeed (https://github.com/organizations/tendenci) goes to the Github home page
There are other easy fixes on that page too:
 * "Find out about Tendenci Open Source Hosting Requirements" should point directly to ReadTheDocs, not to a page on tendenci.com which links to RTD.
 * "Getting Started hosting Tendenci on Rackspace Open Stack Cloud Hosting" links to a page that says it is outdated and look at read the docs.

There is also `issue 845`_ reported in August 2020 requesting access to fix documentation which didn't see a response until it was pinged several years later.

.. _developers page: https://www.tendenci.com/developers/
.. _issue 845: https://github.com/tendenci/tendenci/issues/845

Proposed solution
-----------------

The suggestion for this issue is to permit community members editing ability over Tendenci's documentation site. The specifics are (of course) the part which decides the complexity but I can see two main options:

* People contact an address to request access to edit the docs site and are granted it on a case by case basis
* People log in to the site using their GitHub logins via oath and those who are already contributors are able to edit documentation right away.

These solutions (and others like them) will require some administrative overhead but facilitate several advantages including enhanced contributions to the documentation and a possible documentation split between documentation for users/administrators (going to `tendenci.com`_) and developers (pointed at `readthedocs.org`).

.. _tendenci.com: https://www.tendenci.com/help-files/
.. _readthedocs.org: https://tendenci.readthedocs.org/en/latest/index.html


Future plans are opaque
=======================

The concern
-----------

There is not - that we know of - a published roadmap for Tendenci providing future plans at _any_ level.


Problem outline
---------------

Sometimes a community members needs line up with a projects medium or long term goals - when a roadmap or feature planning information is accessible members are able to proactively contribute features (or fix thing) which will help Tendenci. When working without that information a community member must decide the need is so real they will do the work but risk the changes sitting idle (this has happened in the past).

Related to that is detail in tickets. A recent example (at time of writing) of a ticket which isn't very detailed is `issue 660`_ . If the community know what is desired someone might be willing to chip in and either write the docs or start developing a feature.

.. _issue 660: https://github.com/tendenci/tendenci/issues/660


Proposed solution
-----------------

It would be great to see more information in this space, for example a page in the documentation with a high level roadmap linking to GitHub projects for each release (note that this does not mean linking to individual issues).

If that is considered too high maintenance, having projects for projected major releases and having issues tagged for target releases would help provide visibility for potential contributors.


Participation needs to be easy
==============================

Having a public bug tracker and accepting merge requests is important and I can say from personal experience that it is an excellent thing to be able to make submissions. Thanks!

I would like to suggest some other ways in which participation can be made easier.


Developers developers developers
--------------------------------

https://www.tendenci.com/developers/ makes a call out for contributors (of various kinds), but doesn't provide much to help them get started in non coding contributions.

For example:
 - Design Tendenci Themes does not link to anywhere themes can be shared
 - Build Tendenci Plugins does not link to ANY documentation at all

There are also other kinds of contribution that are not tracked or proffered in any way: 'community contributed tooling', for example Ansible or Puppet scripts to manage Tendenci. Where can those be noted/publicised to the community at large?


Proposed solution
-----------------

Firstly, this would be helped by allowing community members to edit all documentation - these links and related pages could be fixed to provide proper assistance to interested parties.

A bazaar like that mentioned in `issue 692`_ might be a mechanism to enable tracking 'community contributed tooling', unless there is an intent that all offered plugins and themes will be merged in to a Tendenci repository somewhere.

.. _issue 692: https://github.com/tendenci/tendenci/issues/692


Contributions need to be matched
================================

The time of external contributors is scarce and unpredictable. Because of that, I (@goetzk) believe it is important to ensure they are not left waiting

Code and questions
------------------

 - Submitted PRs need /something/ within 48 hours, ideally 24 hours (the something could be feedback or merging)
 - Tickets which aren't a merge but are a POC should have the same treatment. In 2018 someone tried to ask a question providing psudocode and `the question is still outstanding`_
 - Incomplete/WIP PRs are no exception, if anything they are more important because someone WANTS to work on it
 - Bugs need /something/ within 72 hours, ideally 24 hours

Just because an issue is hard doesn't mean it should be ignored. A little bit of feedback might help unblock a problem.

.. _the question is still outstanding: https://github.com/tendenci/tendenci/issues/684


Participation needs to be engaged with
======================================

Incomplete engagement
---------------------

Several times recently I've seen comments which were engaged with but which were left hanging shortly after.

 - Having people vanish mid conversation is really off putting, see fe `issue 578`_ or `issue 684`_
 - People try and 'trigger' engagement and `get nothing in response`_, for example when Adam created a Matrix chat or where @goetzk `replied to a very enthusiastic response`_ but saw nothing thereafter.

.. _issue 578: https://github.com/tendenci/tendenci/issues/570
.. _issue 684: https://github.com/tendenci/tendenci/issues/684
.. _get nothing in response: https://github.com/tendenci/tendenci/issues/613#issuecomment-392497823
.. _replied to a very enthusiastic response: https://github.com/tendenci/tendenci/issues/613#issuecomment-392497823

Incidentally the Matrix channel can be found at https://matrix.to/#/#tendenci-dev:matrix.org

Many moons ago I (@goetzk) responded to a survey - probably received via emailed newsletter. Never received an answer to the issues raised and many of my comments (related to community) don't appear to have been actioned - in many cases they are the same as those I'm providing now.
While working on this letter I asked for my survey responses (on 2018-06-09), they were never received.


Contributors want recognition
=============================

Many contributors don't receive anything for their efforts (except perhaps their own lives being a little easier), so recognition of their contribution is all they will see.

Thinking on my feet, I (@goetzk) wonder if some public thanks in the newsletter for people/orgs who have made "substantial" contributions since the previous newsletter? It might help show off their communities, company, or otherwise help give the impression of greater community. This could also apply to contributors LinkedIn/Twitter/other profiles.


Update: I have seen a contribute receiving credit in the Tendenci newsletter. If it continues I will move this to resolved.


Tendenci's codebase has too much included
=========================================

While this point can reasonably be debated it is included as the complexity of Tendenci does carry a cost.
There are two forms this takes:
* Redundancy in application behaviours
* `too many things`_ for the new administrator to grapple with.

.. _too many things: https://github.com/goetzk/tendenci-community/issues/2

Application redundancy
----------------------

I've recently encountered this again because News, Pages and Articles are all very similar in what they do. They take one or two blocks of text and display them on a site.

This causes confusion to users (about where a particular post should be made) and appears to result in development mismatches between the modules.

Articles and events have a single group selectable while news supports multiple groups. The code for Articles looks from the code like it should be multi select (models.ManyToManyField). Firstly the relationship used to be an ForeinKey but was migrated to ManyToMany. Second the groups list is copied by code internally (ie when duplicating an event) so multiple groups is meant to be supported. There are also various "if groups count > 0" tests in the codebase. Its possible the UI was just never updated to match the new DB modeling so it has to be created with one group and others added after the fact (I'm yet to test that though).

I propose that situations like this have a single application and a selectable field to hint Tendenci in how best to display the content.

This leads in to the next item.


Too many things
---------------

`too many things`_ was posted as a suggestion for this document and I include the posters thoughts largely unedited below.

.. _too many things: https://github.com/goetzk/tendenci-community/issues/2

Tendenci needs to be simplified, there are at the moment too many functions. This is an unnecessary burden on everyone and everything. Developers, maintainers, documentation, deployment.

Some apps should be removed and offered as plugins.

Core functions that should be available:

 * Newsletter
 * User management
 * Events
 * Calendar (improved)
 * Forms
 * News

To be disabled. But left in the installation for the user to activate.

 * Forums
 * Directories
 * Staff
 * Jobs
 * Resumes
 * Industries

Others can be really removed and left as plugins.

 * Videos (this can be really deprecated)
 * Redirects
 * Careers
 * Educations (what is this?)
 * Stories Pages and news are already there. No point to have an extra app for stories. There are also articles and cases. Is that all really needed?
 * And some more.


Improvements / fixes which have been made
=========================================

Updated credits
---------------

@eschipul updated the credits not long after he found this document. They (Tendenci) haven't been consistent in updating but the complaint as written was addressed.

Removed forum
-------------

Although technically the forum is still there (causing a bit of confusion I expect) it has no contents and I suspect is no longer in use. As such complaining about its contents and usage seems unfair so removed that section.

Pull requests being actioned
----------------------------

Since the first versions of this document pull requests are being actioned in a much more timely manner. Thanks @jennyq!

