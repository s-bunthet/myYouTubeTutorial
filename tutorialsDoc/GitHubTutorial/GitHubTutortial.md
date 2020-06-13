# GitHub tutorial

[Advanced Git Tutorial](https://www.atlassian.com/git/tutorials/advanced-overview)

1. Github: a code hosting platform for version control and collaboration.
2. Github Essentials:
   - repositories
   - branches
   - commits
   - Pull Requests workflow
3. Merging vs Rebasing
   - rebasing get a much cleaner project history (linear project history )
   - git merge --squash
4. Resetting, Checking Out and Reverting
5. Advanced Git Log
6. Git Hooks
7. Refs and the Reflog
8. HEAD : is where the last commit locate
9. Head Detached
10. git log,git log --stat git bisect, gitk
11. rebasing trade-off: safety and traceability
12. the golden rule of rebasing
13. Incorporating Upstream Changes
14. Reviewing a Feature With a Pull Request
15. git hooks
16. git LFS
17. git submodules
18. git subtree
19. git gc
20. git prune
21. git bash
22. git cherry Pick
23. git-show
24. git checkout `commit id` vs git reset --hard `commit id`
25. commit: is the `stage` or `version` of change in the repository
26. `git checkout -- .` : go back to the last commit and get rid of the unstaged changes
27. git branch -D branch-name : delete the branch-name branch (after merging maybe :))
28. git add: to `stage` the change
29. git commit : to commit the staged change
30. remote repository
31. git remote add origin 'remote-repo-url':
    - remote add: etablish a connection between local repository and local repository
    - origin : is the name of the remote repository. By convention, we call it 'origin'. Actually, we can name it what we want.
    - `Note`: By doing this command, there is nothing happen at the remote repository, because we just only make connection. However, if we type: `git remote`: we will see the `origin` as name of the remote repository.
32. - git branch
    - git branch -r
33. git fetch: get the code from the remote repository to the `The remote tracking branch`(it is just like the connection between the remote and local repository)
34. git merge: get the code from `The remote tracking branch` to the local branch
35. we have two solution to get the code from the remote repository to the local repository:
    - `git fetch`, then `git merge`
    - `git pull`
36. git remote rm origin: delete the remote repository
37. git stash, git stash push -m "", git stash list, git stash apply, git stash drop, git stash pop (go to that stash and delete that stash from the stashes list)
38. git keeps track of the code history that has been snapshoted at each change by each user.
39. Staging area or Index is where the code snapshots are store reday to commit.
40. git commit --amend -m "new name of the last commit": change the name of the last commit.
41. commit hash or commit id : is the id that identifier each commit. If we change the name of the commit, its hash **also changed**.
42. git cherry-pick: get a commit from another branch
43. git clean -df: clean the untracted or unstaged directories or files
44. `git reflog` vs `git log`
45. `git reflog` : can get the repository back to the removed commits(after git reset for example.). How? -> look on the internet.
46. git diff 'commit-1-hash' 'commit-2-hash': compare the difference between two commits.
47. .gitignore: excludes files from being tracked with Git.
48. git show
49. Why staging? => imagine the days of making two logically unrelated modifications to a file before you realized that you forgot to commit one of them. Now you can just stage the change you need for the current commit and stage the other change for the next commit.
50. Working directory vs repository:
    - working directory: is the directory that you are working on and that might include the git repository
    - git repository: is
51. workspace: local checkout
52. commit = checkin
53. staging area = cache = staged files = current directory cache
54. git repository (.git) is a folder that contain the information about the changes(index, commit, logs, ...,etc) made in the directory in which the git repository is init.
55. workspace: is the set of git repositories in the machine

## TODO

1. search how to cache the github password
