# select2 packages
Packages repo of select2 (https://select2.org)

this is a repo to hold different versions of select2 you may need
and also to make them available for the application as default

# Quick setup for new versions
    - git checkout master
    - git checkout -b v1-2-3 (Your new version to add or check for
      existing: git branch -a)
    - download your version somewhere
    - mkdir v1.2.3
    - cd v1.2.3/
    - Place your new files here
    - git add --all
    - git commit -m 'Adds version v1.2.3'
    - git push
    - done!
    - Make application wide available?
    - git checkout packages
    - git merge v1.2.3
    - git push
    - done!


# select2 ready to run files
Downloaded from select2.org and set to the "packages" branch.

Checkout the single version (branch) you need or
create a new branch starting at the master branch and add your version as follow
    git co master
    git co -b myNewVersion (eg. v3-1-2; branches with slashes, folders with dots)
    mkdir ./v3.1.2/
and put your files here ./v3.1.2/*
For select2 i just use the "dist" folder from github select2 releases.

The master branch should only contain the README to guide you/
developers, the "packages" branch contains all versions to be used
(old and new once to always have a fallback if older applications
are not upgraded!).
The versions branches to modify for bug or improvements or to use
just as single branch for other projects.

if you need your version application wide? then merge your version
to the "packages" branch.
NEVER to the master!
at any time you should merge this readme to your branch to also get
updated informations

# Example:
## Packages branch
    ./v1.8.3/_some_files_of_version_1.8.3
    ./v2.0.0-Beta/_some_files_of_version_v2.0.0-Beta
    ./README.txt <- this readme

# Changelog
    Adds version 4.0.3
    Adds version 4.0.4

