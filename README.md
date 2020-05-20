# Branched off

## Story

You've been using git for a while now. With this project you will put your knowledge to a test, by using only the terminal. You will need to keep switching branches, so try to not to fall!

## What are you going to learn?

You will learn:

- Git basics
- Git branching
- Git rebase
- shell basics

## Tasks


1. Create your exercises by running the init script - `./helper/init`

    - Running command: `git branch`
Results in:
    ```
    conflict-feature

    conflict-rebase-feature

    demo

    x master

    merge-conflict

    merge-simple

    merge-undo-last

    rebase-branch

    rename-commit

    simple-feature

    undo-last

    undo-last-but-one

    undo-last-feature
    ```

2. Edit your local `undo-last` branch's history by undoing the last commit.

    - Switch to branch: `undo-last`
Running command: `./helper/print_log`
Results in:
    ```
    # No output
    ```

3. Edit your local `rename-commit` branch's history by fixing the typo in the last commit.

    - Switch to branch: `rename-commit`
Running command: `./helper/print_log`
Results in:
    ```
    f5c8307 (HEAD -> rename-commit) Important message
    ```

4. Go back in your local history on `demo` branch to a previous commit. This will be useful if you want to demo a working version.

    - Switch to branch: `demo`
Running command: `./helper/print_changed_files`
Results in:
    ```
    just-works-tm.js
    ```

5. Integrate changes into the local `merge-simple branch` from the `merge-simple branch` local branch, it should go smoothly.

    - Switch to branch: `merge-simple-branch`
Running command: `./helper/print_log`
Results in:
    ```
    348f321 (HEAD -> merge-simple, simple-feature) New feature works
    ```

6. Integrate changes into the `merge-conflict` branch from the `conflict-feature` local branch - there will be a conflict - but you should be familiar with this by now.

    - Switch to branch: `merge-conflict`
Running command: `./helper/print_log`
Results in:
    ```
    0bcda64 (HEAD -> merge-conflict) Merge branch 'conflict-feature' into merge-conflict

    e20c235 Old feature fix

    deaf171 (conflict-feature) New feature works
    ```

7. Integrate changes into the `merge-undo-last` local branch from `undo-last-feature` local branch, but before that you need to undo the last commit as it is redundant and would cause problems.

    - Switch to branch: `merge-undo-last`
Running command: `./helper/print_log`
Results in:
    ```
    d83e3e7 (HEAD -> merge-undo-last, undo-last-feature) New feature works
    ```

8. Integrate changes into `rebase-branch` branch from `conflict-rebase-feature` local branch. Use rebase.

    - Switch to branch: `rebase-branch`
Running command: `./helper/print_log`
Results in:
    ```
    30d0536 (HEAD -> rebase-branch) Old feature fix

    2999d91 (conflict-rebase-feature) New feature works
    ```

9. Edit your the `undo-last-but-one` branch's history, keeping the last commit and removing the one before it.

    - Switch to branch: `undo-last-but-one`
Running command: `./helper/print_log`
Results in:
    ```
    51243ac (HEAD -> undo-last-but-one) WIP some progress with security
    ```


## General requirements


None

## Starting repository

Follow [this link](https://journey.code.cool/v2/project/solo/blueprint/branched-off/general) to create your project repository.

## Hints

- Examine the contents of the repository. There are examples of git usage in the scripts checked in here.
- You will push and pull a lot and it gets annoying if you have to retype your password all the time. Read the linked materials!
- If you feel that you made a mistake during an exercise use: `./helper/reset` to get back to the original state.
- Your git hash - the first few characters of the `./helper/print_log` - will be different from the one here.
- Always make sure that you are on the correct branch when working on an exercise

## Background materials

- :exclamation: [Git without password](../pages/git/git-passwordless.md)
- :exclamation: [Undo things in git](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History)
- :exclamation: [Branches in a nutshell](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)
- :exclamation: [Branching and merging](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)
- :exclamation: [Branch management](https://git-scm.com/book/en/v2/Git-Branching-Branch-Management)
- [Git branching and workflows](https://learn.code.cool/full-stack/#/../pages/git/git-branching)
- [Merge vs rebase](https://learn.code.cool/full-stack/#/../pages/git/merge-vs-rebase)
- [Mastering git](https://learn.code.cool/full-stack/#/../pages/git/mastering-git)
- :open_book: [Rebasing](https://git-scm.com/book/en/v2/Git-Branching-Rebasing)
- :open_book: [Bash guide](https://mywiki.wooledge.org/BashGuide)
