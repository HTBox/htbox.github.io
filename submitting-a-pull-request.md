---
layout: default
---

# Submitting a Pull Request

## TL;DR

> When you're done with all the code for an issue, submit a pull request and we'll take a look.

## Long Version

You don't have to wait until all your work is done in order to send us a pull request. If you want the core team to look at your code, but not accept the changes yet, open a pull request, and prefix the title with 'WIP'. That tells us to review the code, but that it is not done, and is not yet ready to merge. When you are finished, and the PR is ready to merge, simply remove 'WIP' from the PR title, and we'll give it a final look, and merge it.

When you submit a pull request, an automated build (using AppVeyor) will merge your changes onto a copy of the master repository, build that configuration, and run all automated tests. If any of those steps fail, we will ask you to fix them before we accept the pull request. (We don't comment on this if you've labelled the PR 'WIP'.)

We ask you to resolve any merge conflicts because you know your code the best. This [article](http://thebillwagner.com/Blog/Item/2015-08-18-IforgottoforkbeforeIstartedworkingandhowtofixit) shows how to update your fork from master.

Ideally, you can rebase your changes on the lastest version of mster. 
