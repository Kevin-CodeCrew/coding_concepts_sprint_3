###### TOP
# Coding Concepts Sprint 3 Materials - Software Deployment Principles, Github for Team Development
<!-- 
* [Team-based Software Development](teamBasedSoftwareDevelopment.md)
* [Github and Teams](githubAndTeams.md)
* [Pulls and Pull Requests](pullsAndPullRequests.md)
* [Branching](branching.md)
* [Conflict Resolution](conflcitResolution.md)
* [Tags and Releases](tagsAndReleases.md)
* [Stashing](stashing.md) -->
### Team Based Software Development

<img src="img/agileSDLC.png" width="auto" height="300"/>

[Back to Top](#TOP)
### GitHub and Teams

[Back to Top](#TOP)
### Pulls and Pull Requests

[Back to Top](#TOP)
### Branching
A branch represents an independent line of development. Branches serve as an abstraction for the edit/stage/commit process. You can think of them as a way to request a brand new working directory, staging area, and project history. New commits are recorded in the history for the current branch, which results in a fork in the history of the project.

<img src="img/01.svg" width="auto" height="400"/>

Create a new branch called `<branch>`. This does not check out the new branch.
````
git branch <branch>
````

In Git terms, a "checkout" is the act of switching between different versions of a target entity. The git checkout command operates upon three distinct entities: files, commits, and branches.
````
git checkout -b <new-branch>
````
The above example simultaneously creates and checks out `<new-branch>`. The -b option is a convenience flag that tells Git to run git branch `<new-branch>` before running git checkout `<new-branch>`.


<img src="img/Branch-1.png" width="auto" height="400"/>

Merging is Git's way of putting a forked history back together again. The `git merge` command lets you take the independent lines of development created by git branch and integrate them into a single branch.

[Branching Source](https://www.atlassian.com/git/tutorials/using-branches) |  [Merging Source](https://www.atlassian.com/git/tutorials/using-branches/git-checkout)

[Back to Top](#TOP)
### Conflict Resolution

Version control systems are all about managing contributions between multiple distributed authors ( usually developers ). Sometimes multiple developers may try to edit the same content. If Developer A tries to edit code that Developer B is editing a conflict may occur. To alleviate the occurrence of conflicts developers will work in separate isolated branches. The git merge command's primary responsibility is to combine separate branches and resolve any conflicting edits.
```
<<<<<<< HEAD
=======
>>>>>>> new_branch_to_merge_later
```
Think of these new lines as "conflict dividers". The ======= line is the "center" of the conflict. All the content between the center and the <<<<<<< HEAD line is content that exists in the current branch master which the HEAD ref is pointing to. Alternatively all content between the center and >>>>>>> new_branch_to_merge_later is content that is present in our merging branch.

[Merging Source](https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts)

[Back to Top](#TOP)
### Tags and Releases

[Back to Top](#TOP)
### Stashing

### Assignments
* Lecture Gist : [placeholder](github.com)
* In Class Assignment Link : [placeholder](github.com)
* In Class Assignment Answer Gist : [placeholder](github.com)
* Classwork Assignment Link : [placeholder](github.com)
* Classwork Assignment Answer Gist : [placeholder](github.com)
* Classwork Assignment Video Walk through : [placeholder](github.com)

### [Back to Top](#TOP)