1. `git init` -> Powers your folder to be managed by git, and initialises a new empty repository.
   It also creates a .git folder that has all the relevant logic to manage versions of your project.

2. `ls -a` -> lists all the hidden files.

3. `touch` -> this will create a new file, just give the file name with extension.

4. `rm -rf` -> to delete a file. -r will delete all the internal files recursively..

5. `working area` -> There can be a bunch of files that are not currently handled by git. It means that changes done
   or to be done in those files are not managed by git yet. A file which is in working area is considered
   to be not in the staging area. when we do `git status` and we see a bunch of `untracked files` then these
   are actually called to be in working area.

6. `staging area` -> what all files are going to be part of next version that we will create.
   This staging area is the place where git knows what changes will be done from
   last version to the new version.

7. `Repository area` -> This area actually contains the details of all your Previous registered verion.
   and the files in this area, git already manage them and knows their version history.

8. `git add <file>` -> moves file from working area to staging area.

9.`git rm -- cached <file>` -> move file back from staging area to working area.

10. `commit` -> commit is a particular version of the project. It captures a snapshot of the project's staged changes
    and creates a version out of it.

11. `git commit` -> registers staging changes to a commit..

12.`git log` -> list downs all the commits of the repository. If you want to wxit out of git log prompt press `q`.

13. `git restore <file>` -> it removes all files changes from the staging area to be committed. This can be useful, if we did
    some dirty piece of code and now no more want it. Instead of deleting every change line by line, we can restore
    last clean version of the file.

14. `git restore --staged <file>` -> It removes file from changes from staging area to working area.
    this only works if changes are in your staging area.

15. Diff between git rm and git restore
    ans : if you want to move the whole file back to the untracked state, then we do git rm.
    otherwise if we just want the changes to be moved in working area or staging area then we git restore.

16. `git diff commit1 commit2` -> gives the difference of all file changes between two commits.

17. `git commit -m "<message>" -> directly commits your request with message.

18. `git remote` -> list down all the remote connection names.

19. Remote connection -> It help you to link two git repositories for uploading and downloading changes from each otherwise.

20.`git remote add <name of remote > <link of the remote>` : this command helps us to add a new link to the remote
repo and give a name to it.

21. `git remote rm <name of remote>` -> this command deletes a remote connection.

22. `git remote rename <oldname> <newname>` : this command renames the remote connection.

Note: The name of the remote connection is always used to establish communication between the repos.

23. `git add .` : this command will add all files from working repo to staging area.

24. `git add <file1> <file2> <file3>` : this command will add multiple file changes together in the staging area.

25. `git pull <remote name> <branch name>` : downloads latest changes from the branch of the mentioned remote in your local repo.

### Recommended practice to do

- make changes
- git add<file>
- git commit
- git pull
- git push

merge confilts occur when multifle people try to make changes to the same file, and then collaborate.
