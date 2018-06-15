=======================
tendenci community paper cuts
=======================

Every now and then the topic of community comes up in discussions around Tendenci and there is a general agreement it would be good to see more external contribution (a sentiment I doubt anyone will disagree with).
Despite that, in the last two years I haven't seen any change in how Tendenci's parent company ('T's parent' from here on) tries to encourage or facilitate greater contribution.

I have put together the following document to try and expose areas I believe can (and should) be addressed in the hope that they will lead to greater input from the developer community and make Tendenci a more attractive project to participate in.


I also want to state up front that I appreciate I am asking more of the small number of already busy people behind the project and that none of the stuff below is thoughtlessly easy to implement. However I do believe they are important and that many of them should be relatively easy to cater to.


Participation needs to be easy
======================

Having a public bug tracker and accepting merge requests is important and I can say from personal experience that it is an excellent thing to be able to make submissions. Thanks!

I would like to suggest some other ways in which participation can be made easier

Forum notifications
--------------------

I believe in order to achieve its full potential the forum needs to provide notifications. Why? because being required to check something means it will be forgotten. An email (or RSS feed or whatever) brings the activity to the subscriber and essentially prompts them to take part in the conversation.

I would like to see the ability to subscribe to:
- posts I made
- posts I reply to
- specific sub forums
- the entire forum

This is, coincidentally, roughly the same levels as GitHub provides.


T's parent only documentation
-------------------------------

Lots of documentation is on the Tendenci (organisation) website and is not editable to casual contributors (presumably only available to T's parent staff). Some of the documentation is correct, comprehensive and current. Some of it is irrelevant and wrong. Some of it sits in the middle and is good, but needs an update. I will cite my recent PRs supplying documentation for Stripe integration as an example of working around the lack of editing ability - if i was able to edit the documentation directly I would have been able to add my new information there.

As an example of the problematic nature of the T's parent only pages I reported this issue in 2015 which is still unfixed:
* Your developers page (https://www.tendenci.com/developers/) has a number of broken links. [...]  Github Newsfeed (https://github.com/organizations/tendenci) goes to the Github home page
There are other easy fixes on that page too:
* "Find out about Tendenci Open Source Hosting Requirements" should point directly to Read the docs, not to a page on tendenci.org which links to rtd.
* "Getting Started hosting Tendenci on Rackspace Open Stack Cloud Hosting" links to a page that says it is outdated and look at read the docs


I believe the split documentation schism is one reason that searching for Tendenci help can be very hit and miss, its docs often don't seem to come up in my searches (perhaps i'm weird?).


Future plans
-------------

There is not - that I know of - a published roadmap for Tendenci providing information at _any_ level. This means community CANT proactively fix things which will help T's parent, unless they decide the need is so real they'll risk the changes sitting idle (I refer to the recent Python 3/Django 1.11/2.0 branches as examples).

    - https://github.com/tendenci/tendenci/issues/660 . If we know what is desired someone might be willing to chip in and either write the docs (or whatever) or at least start them


Contributions need to be matched
================================

The time of external contributors is scarce and unpredictable. Because of that, I believe it is important to ensure they are not left waiting

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

	- having people vanish mid conversation is really off putting, see fe https://github.com/tendenci/tendenci/issues/570 ,
	- people try and 'trigger' engagement, get nothing https://github.com/tendenci/tendenci/issues/613 , https://github.com/tendenci/tendenci/issues/685#issuecomment-394572592 me trying to engage


Respond to feedback
-------------------

Many moons ago I responded to a survey - probably received via emailed newsletter. I never received an answer to the issues I raised and many of my comments (related to community) don't appear to have been actioned - in many cases they are the same as those I'm providing now.

While working on this letter I asked for my survey responses (on 2018-06-09), a week later I have yet to receive a reply of any description.



Contributors want recognition
=============================

Many contributors don't receive anything for their efforts (except perhaps their own lives being a little easier), so recognition of their contribution is all they will see.

I think it is important that the credits document (or an equivalent) is updated to include those who have made a "substantial" contribution, *without them needing to ask*

- https://github.com/tendenci/tendenci/blob/master/docs/credits.md this  has not changed for 4 years.

Thinking on my feet, I wonder if some public thanks in the newsletter for people/orgs who have made "substantial" contributions since the previous newsletter? It might help show off their communities, company, or otherwise help give the impression of greater community.


- this might help https://github.com/tendenci/tendenci/issues/692, app / contributions bazaar
		- this tangentially relates to 'community contributed support tooling', for example ansible or puppet scripts to manage tendenci. Where can those be noted/publicised to the community? forum kind of




- Outstanding notes:
- https://www.tendenci.com/developers/ makes a call out for contributors (of various kinds), but then issues like https://github.com/tendenci/tendenci/issues/692 make contributions harder (TBC: does it?)

TODO: open bug on tendenci: ship all available docs (known to be relevant to a release) in project installs? build a -doc package which includes it? the current shipped docs are pretty sparse.


