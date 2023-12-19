1. `git init` -> Powers your folder to be managed by git, and initialises a new empty repository.
    It also creates a .git folder that has all the relevant logic to manage versions of your project.

2. `ls -a`  -> lists all the hidden files.

3. `touch`  -> this will create a new file, just give the file name with extension.

4. `rm -rf` -> to delete a file. -r will delete all the internal files recursively.

5. `working area` -> There can be a bunch of files that are not currently handled by git. It means that changes done
                or to be done in those files are not managed by git yet. A file which is in working area is considered 
                to be not in the staging area. when we do `git status` and we see a bunch of `untracked files` then these
                are actually called to be in working area.   