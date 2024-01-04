# How do I return to an old commit?
It's simple! You just use the `git reset [commit hash] --[hard | soft | mixed]` command!
But beware! There are ways to execute this reset, each varying from the levels of code fog! Take a look at them:

1. `soft`: Resets, but puts the files from post commits in the **STAGED** state;
2. `mixed`: Resets, but puts the files from post commits as **UNTRACKED**;
3. `hard`: Resets Everythin! It deletes everything from post commits! Only when the code is terrible;

I tested it all.

# Useful commands
Some commands that can help me not lose a bunch of time!

1. `git fetch`: Fetches future alterations made in the `remote` branch and creates a local branch representing it! It differs from `git pull`, which fetches and merges this branch;
2. `git stash`: Are you occupied solving a problem in a branch, but a bug appeared from another one? This command saves all alterations made to the current branch **WITHOUT COMMITTING**. This save your unfinished work for you!

## About `git stash`
There are two ways to **stash**: **APPLY** and  **POP**. The latter *applyes* the alterations stashed in your current branch, but mantains the content stashed. The former, your alterations are aplied in the current branch, but it's deleted from the stash. 

> We can create a stash in a branch named *X* and use it in another branch named *Y*!