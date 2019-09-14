## GitHub Workflow
### Pushing Data to GitHub
1. `cd` to your local github directory
1. Use alias `gs` or full command `git status` to see the
   untracked or modified files.
1. Use alias `ga <files-you-want-to-add>` or full command
`git add <files-you-want-to-add>` to add the files you want
 to push up to GitHub. Alternatively, use `ga -A` to add all
 untracked/modified files present in repository.
1. Use alias `gc "Your commit message"` or full command
`git commit -m "Your commit message"`, to commit the changes
so they can be pushed.
1. Use alias `gp` or full command `git push`, to commit the changes to
   your repository.

### Fetch and Merge data from Remote to Local Repo
1. `cd` to your local github directory
1. Use alias `gs` to check if any there are any uncommitted changes,
   untracked changes are okay to have. However, _modified_ files will
make git angry. You will either need to follow the [push data to github](pushing-data-to-github)
and add these files to the remote repo, or stash your changes.
Check out [this](https://www.atlassian.com/git/tutorials/saving-changes/git-stash) article for more details.
1. Uses alias `gf` or full command `git fetch` to download the
   changes from the remote to your local repository. Note, although
the changes have been downloaded to your local machine, you will not
be able to see them as they have not been applied yet.
1. Use alias `gm` or full command `git merge` to merge the downloaded
   changes received from `gf`/`git fetch` to you local repository.

### Bonus Info and Commands

#### Markdown
[Markdown Tutorial](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

#### Getting help -- `man`(ual) pages
The terminal despite popular opinion sets you up for success with the
copious amount of documentation available right at your fingertips. To
unlock the power and read to your hearts desires, simply type `man` a
space and then the command you are interested in. For example:
```
man git
man git-add
man git-commit
man git-clone
man git-merge
man man
man xargs
# or if you are in a particularly ready mood
man git git-add git-commit git-clone git-merge man xargs
``` 
You will soon wonder, Austin, how does thou leave thy land of
knowledge? I will respond with, simply press the letter `q`.

You can also search man pages by first opening a manual and then
typing the forward slash, `/`, followed by whatever you would like to
find. Use the letter `n` to go forwards and the capital `N` to go to
prior results.

Pressing the letters `d` and `u` will allow you to skip half a page as
well. That's pretty neat!

#### Gitignore
You can tell git to ignore a certain file extension using a
`.gitignore` file. For example, lets say that we are on macOS and we
have been writing some python scripts to multiply a raster by some
constant. MacOS is notorious for leaving around `.DS_Store` files all
over the place. You don't want to add those files to your repo because
they are of no use to anyone but your computer, so, in the root
directory of you repository, you can create a file named `.gitignore`,
where you can list (each file extension type on a newline) the types
of files that you want git to, you know, ignore. 

#### Choosing a GitHub License
[This](https://choosealicense.com) website is excellent and will explain it better than I ever
could. USE A LICENSE. 


#### Shortcuts and Fudge up fixes
Instead of typing `git add <file1> <file2> <file3>` use the flag `git
add -A` to add all modified and untracked changes.

If you want to reach full wizard status, use you can do a `git add -A`
and a `git commit -m "Some message"` at the same time with the
command: `git commit -a -m "Reaching enlightenment"`


Author: [Austin Raney](mailto:aaraney@crimson.ua.edu)
