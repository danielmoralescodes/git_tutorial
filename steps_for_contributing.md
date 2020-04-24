If you have write access
========================

Clone repository you want to contribute to:
`git clone URL`

Create a new branch with a descriptive name:
`git branch adding_my_functionality`

Check that branch was created:
`git branch`
The output should look something like this:
```
  adding_my_functionality
* master
```
The star indicates that we are currently working on the master branch.

Change to our new branch:
`git checkout adding_my_functionality`

Now the output of `git branch` should be:
```
* adding_my_functionality
  master
```

Create a file with some content.

Check gits status with `git status`:
```
On branch adding_my_functionality
Untracked files:
    (use "git add <file>..." to include in what will be committed)

        hello_world.py

nothing added to commit but untracked files present (use "git add" to track)
```
Check that you are on the branch you created for your changes (first line) and
the file you just created shows up as an untracked file.

If everything looks fine you can commit the new file, i.e. create a 'snapshot' of it that you will be able to
go back to later.
To do so we first have to tell git which files it should take the 'snapshot' of:
`git add hello_world.py`

Lets check that we staged the file for commit with `git status`:
Output:
```
On branch adding_my_functionality
    (use "git reset HEAD <file>..." to unstage)

        new file:   hello_world.py
```
It makes sense to add multiple files if the changes you made are logically linked and the program only works when all files are changed.

Let's commit our file:
`git commit -m "inital commit of the hello_world file which provides the function hello_world"`

The next step is to push our changes to the Github:
`git push -set-upstream origin adding_my_functionality`

You can repeat the change, add, commit, push process until you think your code works well and you want to share it.
To share it you create a pull request on github.

If you don't have write access
==============================


