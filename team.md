---
title: "Team"
permalink: /team
---
[Home](/Overview/) |  [Project](/Overview/project) | [Team](/Overview/team) | [Journal](/Overview/journal) | [Deliverables](/Overview/deliverables)

## Contributors

- Teddy Randby:   [kerandby@live.unc.edu](mailto:kerandby@live.unc.edu)
  - Project Manager
  - Webmaster
  - Tech Lead
  - Frontend Lead
- Muyan Pan:      [muyan@live.unc.edu](mailto:muyan@live.unc.edu)
  - Client Manager
  - Design Lead
- Thomas Le:      [elsamoht@live.unc.edu](mailto:elsamoht@live.unc.edu)
  - Backend Lead
  - Infrastructure Lead

## Rules

-	Should a team member miss a meeting, he should notify other team members ASAP; best if other members are notified 24 hours in advance
-	Main source of communication among team members will be GroupMe
-	Try to check GroupMe at least twice a day (weekends included)
-	If there is a no response from a team member; other members will decide on the best action, and they might move on 

### Coding Style
-   Use JavaScript linter [ESLint](https://eslint.org/)
-   Use [JavaScript Standard Style](https://standardjs.com/)
-   Video discussing how to use Standard and ESLint together [here](https://www.youtube.com/watch?v=kuHfMw8j4xk)

### Git Collaboration
In general, following [OneFlow](https://www.endoflineblog.com/oneflow-a-git-branching-model-and-workflow) model and workflow with only `master` branch in remote repository
-   Using Github
-   Only master branch in remote repository
-   Every new commit to master branch must be reviewed by at least **one** team member. Will use Pull Requests to do so.
-   Team members should look at the PR and review it within 48 hours; let team know if you can't get to it in time
-   **How to add new feature**
    1. Create new branch from master
```bash
$ git checkout master
$ git pull  # Ensure local master branch is up-to-date with remote before branching
$ git checkout -b feature/my-feature
```
        - Use `--rebase` flag for pulling if necessary
    2. After finishing feature, push branch to remote and create pull request for code review
```bash
$ git checkout feature/my-feature # If you aren't already on the feature branch
$ git push origin feature/my-feature
```
        - Steps on creating pull request on Github [here](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request#creating-the-pull-request)
        - Make sure you request reviewers
    3. If changes are requested, simply add changes to local branch, commit them, and push to origin using `git push origin feature/my-feature`
    4. After review, if there are no conflicts with `master` simply press the merge button in the PR.
    5. After review, if there *are* conflicts with `master`
        - You can either use the `Resolve conflicts` button in the Github pull request, or if the conflict is too complex (or you want to use command line)
```bash
$ git checkout master
$ git pull  # Ensure local master branch is up-to-date with remote
$ git checkout feature/my-feature
$ git rebase -i master
# resolve any conflicts, use `git status` to check
$ git push origin feature/my-feature   # use -u flag to track remote if necessary
```
        - Use `--rebase` flag for pulling if necessary
        - Now you can press the merge button in the PR, or you can merge directly using the command line and the PR will automatically pick it up by doing
```bash
# to merge to master using command line
$ git checkout master
$ git merge feature/my-feature
$ git push origin master
```
    6. After merging to master, you can clean up branch locally (remote branch will be deleted automatically if repo setting is set)
```bash
$ git branch -d feature/my-feature
```
