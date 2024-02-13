# A study in gitflow

## Three levels of branches

- main
- develop
- feature

## Why gitflow?

To secure main, by almost never pushing directly to main. Instead, we use a feature level where we write new code, then merge that feature into the develop branch. When that is fully tested, we can merge it into main.

## Issues

A good way to communicate without the need of an external tool, is to use issues in github.

1. Click "issues"
1. Click "New issue"
1. Give it a title and some info.
1. Click "Submit new issue"
1. If you want, assign some member to the issue (or yourself)
1. Click link "Create a branch"
1. Click "Change branch source" and choose **develop**
1. Click "Create branch"
1. In terminal, run "git fetch origin" and "git checkout #-branchname" (the branch now has a number connecting to the issue)
1. Do changes, add & commit & push.
1. On github, you have a green button "Compare & pull request" linked to the issue.
1. Change base to "develop" before clicking "Create pull request"
1. Assert that you're merging into the correct branch, before clicking "Merge pull request" and "Confirm merge".
1. Afterwards, you can delete the feature branch.