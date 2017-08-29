# fpbuilder
FreeBSD Port Builder - distributed system to allow port maintainers
to request for builds

The FreeBSD Port Builder is intended to allow a ports maintainer to have a
mechanism to request for builds for supported architectures.

## Why fpbuilder?
Redports was a great service available but ever since it has gone down, there is
a big void to fill.

## How it works
+ Small-ish web application running on a master
+ Multiple builders - can be on the same host - these can support certain
  FreeBSD releases and architectures
+ Builders pick up jobs from the master and inform once done
+ Depends on github - users provide their specific port directories in a certain
  git repo
+ A builder picks up the repo from github, performs the build and reports
  outcome.

