---
layout: default
---
# Building the project

## TL;DR

> It's likely a Visual Studio based .NET project. Load the appropriate .sln and build. 

## Long version

Some of our projects have both web and mobile components. Those will have a master solution, that builds everything. They will also have a -web solution that only builds the web based application. They may also have a -mobile solution that builds only the mobile applications. 

Load the appropriate solution, and build it.

All our projects have some unit tests. The amount of coverage varies with the origin of the projects. In all cases, we encourage contributors to help add to the unit test coverage. For those projects where we do have good coverage, we may even reject pull requests without the addition of new tests that exercise the code being developed.

