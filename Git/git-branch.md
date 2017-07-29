## Git Branch

Git's branching functionality lets you to create new branches off a project to test ideas, isolate new features, and experiment without impacting the main project.

### View and Create Branches
To view all branches in a Git repository, run the command `git branch`. There will be an asterisk (\*) next to the branch that you're currently on.

To create a new branch, run the command:
```shell
git branch <newBranchName>
```

There's a shortcut to create and checkout a new branch with one command when you pass the `-b` option (for branch) with `git checkout`:
```shell
git checkout -b <newBranchName>
```
