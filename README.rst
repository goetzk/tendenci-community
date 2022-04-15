.. contents::

==================
Tendenci community
==================

Every now and then the topic of community comes up in discussions around `Tendenci`_ and there is a general agreement it would be good to see more external contribution - a sentiment we probably all agree with.

Despite that Tendenci's parent company (`Tendenci (corp)`_ from here on) has struggled to build a growing community of regular contributors.

.. _Tendenci: https://github.com/tendenci/tendenci/
.. _Tendenci (corp): https://www.tendenci.com/

To try and expose areas I (@goetzk) - and others - believes should be addressed, this document has been put together to try and outline issues experienced by the community. At the same time we try to offer solutions to the problems discussed in the hope that they will lead to greater input from the developer community and make Tendenci a more attractive project to participate in.

While some of these steps will result in short term increases in effort (for example set up) or medium term effort (perhaps maintenance) it is felt the effort should pay for itself in easing contribution for potential developers and productivity for instance administrators.


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

A bazaar like that mentioned in `issue 692`_ might be a target for such contributions, unless there is an intent that all offered plugins and themes will be merged in to a Tendenci repository somewhere.

.. _issue 692: https://github.com/tendenci/tendenci/issues/692

Tendenci (corp) only documentation
-----------------------------

Lots of documentation is on the Tendenci (corp) website and is not editable to casual contributors (presumably only available to Tendenci (corp) staff). Some of the documentation is correct, comprehensive and current. Some of it is irrelevant and wrong. Some of it sits in the middle and is good, but needs an update.

I (@goetzk) will cite my recent PRs supplying documentation for Stripe integration as an example of working around the lack of editing ability - if @I was able to edit the documentation directly those PRs would have been able to add new information directly.

As an example of the problematic nature of the Tendenci (corp) only pages I reported this issue in 2015 which is still unfixed:
 * The `developers page`_ has a number of broken links. [...]  Github Newsfeed (https://github.com/organizations/tendenci) goes to the Github home page
There are other easy fixes on that page too:
 * "Find out about Tendenci Open Source Hosting Requirements" should point directly to Read the docs, not to a page on tendenci.org which links to RTD.
 * "Getting Started hosting Tendenci on Rackspace Open Stack Cloud Hosting" links to a page that says it is outdated and look at read the docs.

I believe the split documentation schism is one reason that searching for Tendenci help can be very hit and miss, its docs often don't seem to come up in my searches (perhaps I'm weird?).

.. _developers page: https://www.tendenci.com/developers/

Future plans
-------------

There is not - that @goetzk know of - a published roadmap for Tendenci providing information at _any_ level. This means community CANT proactively fix things which will help Tendenci (corp), unless they decide the need is so real they'll risk the changes sitting idle (I refer to the recent Python 3/Django 1.11/2.0 branches as examples).

Related to that is detail in tickets. A recent example (at time of writing) of a ticket which isn't very detailed is `issue 660`_ . If the community know what is desired someone might be willing to chip in and either write the docs or start developing a feature.

.. _issue 660: https://github.com/tendenci/tendenci/issues/660

Contributions need to be matched
================================

The time of external contributors is scarce and unpredictable. Because of that, I (@goetzk) believe it is important to ensure they are not left waiting

Code and questions
------------------

 - Submitted PRs/ need /something/ within 48 hours, ideally 24 hours (something could be feedback or merging)
 - Even attempts like this which aren't a merge but are a POC should have the same treatment https://github.com/tendenci/tendenci/issues/684
 - Incomplete/WIP PRs are no exception, if anything they are more important because someone WANTS to work on it
 - Bugs need /something/ within 72 hours, ideally 24 hours

Just because an issue is hard doesn't mean it should be ignored. A little bit of feedback might help unblock a problem


Participation needs to be engaged with
======================================

Incomplete engagement
---------------------

Several times recently I've seen comments which were engaged with but which were left hanging shortly after.

 - Having people vanish mid conversation is really off putting, see fe https://github.com/tendenci/tendenci/issues/570
 - People try and 'trigger' engagement, get nothing in response, for example https://github.com/tendenci/tendenci/issues/613#issuecomment-392497823 where Adam created a Matrix chat or https://github.com/tendenci/tendenci/issues/685#issuecomment-395043657 where @goetzk replied to a very enthusiastic response but saw nothing thereafter.

Incidentally the Matrix channel can be found at https://matrix.to/#/#tendenci-dev:matrix.org

Many moons ago I (@goetzk) responded to a survey - probably received via emailed newsletter. Never received an answer to the issues raised and many of my comments (related to community) don't appear to have been actioned - in many cases they are the same as those I'm providing now.
While working on this letter I asked for my survey responses (on 2018-06-09), they were never recieved.


Contributors want recognition
=============================

Many contributors don't receive anything for their efforts (except perhaps their own lives being a little easier), so recognition of their contribution is all they will see.

Thinking on my feet, I (@goetzk) wonder if some public thanks in the newsletter for people/orgs who have made "substantial" contributions since the previous newsletter? It might help show off their communities, company, or otherwise help give the impression of greater community.


Improvements / fixes which have been made
=========================================

Updated credits
---------------

@eschipul updated the credits not long after he found this document. They (Tendenci) haven't been consistent in updating but the complaint as written was addressed.

Removed forum
-------------

Although technically the forum is still there (causing a bit of confusion I expect) it has no contents and I suspect is no longer in use. As such complaining about its contents and usage seems unfair so removed that section.
