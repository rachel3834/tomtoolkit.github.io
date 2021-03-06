---
title: Contribute to the TOM Toolkit
---

The page will go over the process for reporting issues, requesting features, getting
support, and contributing to the TOM Toolkit.

## Reporting Issues

Issue reporting can be done via the [Github issues page](https://github.com/TOMToolkit/tom_base/issues)
of the tom_base project. Reporting an issue requires a Github account, but provides an easy way for
developers to ask follow-up questions about an issue in order to resolve it.

Please include as much detail as possible, as well as the steps taken that trigger the issue, and be sure to tag it with the "bug" tag!

## Requesting Features

Like issues, feature and enhancement requests should be done via the same [Github issues page](https://github.com/TOMToolkit/tom_base/issues) of the tom_base project.

## Support

If you're looking for help with some aspect of your TOM, the [Github issues page](https://github.com/TOMToolkit/tom_base/issues) is once again the place to go. The "question" or "help wanted" tags should be very useful when looking for support, and the TOM Toolkit developers are more than happy to provide the help necessary to get your TOM running. You may also want to peruse the [Closed Issues](https://github.com/TOMToolkit/tom_base/issues?q=is%3Aissue+is%3Aclosed), where someone may have already had (and solved!) your problem.

## Contributing Code/Documentation

If you're interested in contributing code to the project, thank you! For those unfamiliar with the process of contributing to an open-source project, you may want to read through Github's own short informational section on [how to submit a contribution](https://opensource.guide/how-to-contribute/#how-to-submit-a-contribution).

### Identifying a starting point

The best place to begin contributing is by first looking at the [Github issues page](https://github.com/TOMToolkit/tom_base/issues), to see what's currently needed. Issues that don't require much familiarity with the TOM Toolkit will be tagged appropriately.

### Familiarizing yourself with Git

If you are not familiar with git, we encourage you to briefly look at the [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics) page.

### Git Workflow

The workflow for submitting a code change is, more or less, the following:

1. Fork the TOM Toolkit repository to your own Github account.
![Forking example](../assets/img/fork.png)
2. Clone the forked repository to your local working machine.
  ```
    git clone git@github.com:<Your Username>/tom_base.git
  ```
3. Add the original "upstream" repository as a remote.
  ```
  git remote add upstream https://github.com/TOMToolkit/tom_base.git
  ```
4. Ensure that you're synchronizing your repository with the "upstream" one relatively frequently.
  ```
  git fetch upstream
  git merge upstream/master
  ```
5. Create and checkout a branch for your changes (see [Branch Naming](#branch-naming)).
  ```
  git checkout -b <New Branch Name>
  ```
6. Commit frequently, and push your changes to Github. Be sure to merge master in before submitting your pull request.
  ```
  git push origin <Branch Name>
  ```
7. When your code is complete and tested, create a pull request from the upstream TOM Toolkit repository.
![Pull request](../assets/img/pull-request.png)

8. Be sure to click "compare across forks" in order to see your branch!

![Compare across forks](../assets/img/compare-across-forks.png)

8. We may ask for some updates to your pull request, so revise as necessary and push when revisions are complete. This will automatically update your pull request.

### Branch Naming<a name="branch-naming"></a>

Branch names should be prefixed with the purpose of the branch, be it a bugfix or an enhancement, along with a descriptive title for the branch.

```
  bugfix/fix-typo-target-detail
  feature/reticulating-splines
  enhancement/refactor-planning-tool
```