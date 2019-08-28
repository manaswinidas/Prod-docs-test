# Prod-docs-test

This project requires git subtrees. Make sure you have it configured:

Type `git subtree` to check whether it is already supported in your git. If yes, we are good to go. If no, please go through [How To Install Git Subtree on Mac and Ubuntu](https://codeengineered.com/blog/how-to-install-git-subtree/)

# Steps to reproduce

If you go to the `.gittrees` file, you can see a "DMN" subtree. The DMN repository has been created for test purposes. Following are the steps to add a subtree:

`git remote add -f DMN git@github.com:manaswinidas/DMN.git`

`git subtree add --prefix=kie-docs/doc-content/drools-docs/src/main/asciidoc/DMN git@github.com:manaswinidas/DMN.git master`

The latter adds a subtree to `.gittrees` and adds a folder in the given path.

In order to fetch from all subtrees in the root repository, run `git subtree pull-all`.