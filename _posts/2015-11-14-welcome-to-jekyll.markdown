---
layout: post
title:  "Contributing to HTBox projects"
date:   2015-11-15 16:19:02 -0500
categories: general contributing
---
Introduction
All of our projects are Open Source, and released under the MIT license. Before you do anything,
ensure that working on our projects does not conflict with any of your employee agreements. 

We manage project workflow using a form of 'volunteer scrum' process. It's essentially scrum,
but because we know everyone is a volunteer, we expect large flucuations in velocity. We
also know that our volunteers have other committments, and may need to pull away from an
assigned task before it's completed. Later 

The remainder of this document explains how our projects are organized, how to assign 
yourself work, and how to sumbit that work for review. We'll also explain how to submit ideas
for work that you want to do to enhnce our projects.

Finding A Task

TL;DR version:

Look at the issues page for a project, select the Milestones tabl, and select the current
milestone. Those are the items for the current sprint. If this is your first time helping us,
look for issues tagged with the 'JumpIn' label. When you find one you like, write a comment saying 
"I'll work on this". One of the team will reach out to you, and see if you have any questions.

More details:

We use Github issues to manage work. This could be proposed features, tasks under a feature, bugs,
and suggestions. We manage the backlog by using Milestones. Every project has a current milestone, and a
backlog milestone. Issues assigned to the current milestone represent priority items in the current 
sprint. Issues assigned to the backlog milestone have been triaged and accepted, but have not been assigned any
specific milestone.

Some projects have other upcoming milestones, based on customer needs, upcoming pilots, or upcoming
releases.

In addition, we label issues to provide some additional guidance. Withing a milestone, we will use the 'P1',
'P2' and 'P3' milestones to mark the priority of a task or feature. (P1 is the highest, P3 is the lowest.) 
In addition, we use the 'JumpIn' label (which is always green on our projects) to denote issues that would 
be suitable for someone not yet familiar with the project. The 'JumpIn' issues may not always represent 
simple fixes, but they do represent work that does not require a deep knowlege of the code base, or a deep
knowledge of the business workflow for a project.

Other labels are project-specific and will be documented for that project.

Tag yourself in a comment saying that you're working on an issue, and we'll start the converation. 

You may notice that you can't assign yourself to work on an issue. That privilege is limited to the 
core team. Also, we can only assign issues to registered team members. If you enjoy
working on our projects, we'll add you to the team, and we will assign tasks when you tag yourself.

Getting the Code

TL;DR version

Fork the repository. Clone your fork using your favorite Git client tool

Long version:

We use the Github Flow process on all our projects (link). That means you are not commiting your 
changes directly to our repositories. Instead, you will submit a Pull Request for one of the 
lead committers to pull your changes into our repository. That enables us to review your 
changes, and discuss them with you. We even use this process ourselves: other core team members
review our changes and pull them into the repository.

The first step in this process is to get the code onto your machine, configured with a 
github repository where you can commit your changes. You do that by creating a fork of
the project repository in your account. You (and only you) have write access to your fork.

Now, you can clone your fork onto your desktop. You'll commit your changes locally, and 
then push them to your fork on github.

Building the project

TL;DR version

It's likely a Visual Studio based .NET project. Load the appropriate .sln and buld. 

Longer version:

Some of our projects have both web and mobile components. Those will have a master solution,
that builds everything. They will also have a -web solution that only builds the web based
application. They may also have a -mobile solution that builds only the mobile applications.

Load the appropriate solution, and build it.

All our projects have some unit tests. The amount of coverage varies with the origins
of the projects. In all cases, we encourage contributors to help add to the unit test coverage.at whatever adfadf
For those projects where we do have good coverage, we may even reject pull requests without 
the addition of new tests that exercise the code being developed.

Doing the work

TL;DR version

Work as you normally would, commit and push your changes at the cadence that works for you.
Please make one Pull Request for one Issue, rather than fixing several issues in on PR. It's much 
easier for us to review and merge when a PR is focused on one issue.

Long Version:

There are a few steps here that can help us review your pull request and ensure a smooth process 
when we take your code. All the tips described here make it easier for us to merge your changes
with changes being made by other developers.

On at least a daily basis, rebase the changes you are making on the master branch <link>. This 
ensures that when you have completed your work, it merges easily into the master branch.

We recommending rebasing instead of merging the master branch into your fork because thaA creates a 
cleaner pull request.

Consider squash commits. A squash commit combines several original commit actions into one commit.
The result is a single commit that shows all your changes. This isn't necessary, but if you are 
comfortable doing it, please do.

Submitting a Pull Request

TL;DR;

When you're doing with an issue, submit a pull request and we'll take a look.

Long Version;

You don't have to wait until all your work is done in order to send us a pull request. If you want
the core team to look at your code, but not accept the changes yet, open a pull request, and prefix the
title with 'WIP'. That tells us to review the code, but that it is not done, and is not yet ready to merge.
When you are finished, and the PR is ready to merge, simply remove 'WIP' from the PR tktle, and we'll
give it a final look, and merge it.

When you submit a pull request, an automated build (using AppVeyor) will merge your changes onto
a copy of the master repository, build that configuration, and run all automated tests.

If any of those steps fail, we will ask you to fix them before we accept the pull request. (We don't 
comment on this if you've labelled the PR 'WIP'.)

We ask you to resolve any merge conflicts because you know your code the best. This article <link>
shows how to update your fork from master.

Ideally, you can rebase your changes on the lastest version of mster. Here's a quick video that 
shows how to do that.

Responding to Reviews

TL;DR;

If you update your code, and push to your fork, github automatically updates the PR. We'll see the
changes. If you disagree with the review, please comment on the code, and tell us why your 
approach is better. We may or may not approve it, but we will listen.

Long Version

Reviews are especially important when you are making your first PR for us. It's a way to have
a conversation about the code as you make it. We appreciate the volunteer contributions we receive, and 
we value your time. We'd rather help comment early then reject work.

We review PRs (even WIP PRs) once a day, and we will give actionable feedback. Please respond in the 
same tone we use. We want great projects, and we respect your time and contribution. The people reviewing
code are also volunteers and expect to receive the same respect.

