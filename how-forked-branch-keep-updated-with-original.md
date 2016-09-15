http://stackoverflow.com/a/31836086/4123375

This answer summarizes the steps found here (https://2buntu.com/articles/1459/keeping-your-forked-repo-synced-with-the-upstream-source/) which will move your fork to the same commit as the parent.

1. Change directory to your local repository.
   * Switch to master branch. If you are not, git checkout master
2. Add the parent as a remote repository, git remote add upstream <repo-location>
3. Issue git fetch upstream
4. Issue git rebase upstream/master
   * At this stage you check that commits what will be merged by typing git status.
5. Issue git push origin master

For more information about these commands, refer to step 3.
