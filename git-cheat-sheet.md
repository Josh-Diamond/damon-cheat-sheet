## Git Cheat Sheet

First time only - Initialize repository with the following steps:
1. Initialize your repository and link it to github
`git init`
2. Next, we will configure and name the "master" branch, this may be any name you pick, but industry practice is moving towards "main" or using "master" is still a common professional practice. You will only need to do this step ONCE per github account. (so don't repeat unless you make a new github account)
`git config --global init.defaultBranch <name>`
3. Now, we will clone the repository
`git clone <github_URL_of_repository>.git`
ex: `git clone https://github.com/Josh-Diamond/damon-cheat-sheet.git`
4. Now you are ready to code! Change directories into your cloned repository folder (`cd <repo_name>`) then run `code .` to launch the repository in VSCode.
5. Once a file has been created or changes are rendered in an existing file, you can run `git status` to see the file names with changes rendered, waiting to be commited and pushed to your github repository
6. If you would like to operate on a branch other than your global branch (master or main or whatever you named it in step 2), you can run the following command to switch to the specified branch, if it exists, otherwise it will create that branch and switch  you to it. You can also use:
`git checkout -b <branch_name>`
7. To add these changes, we will need to stage them with the following command:
`git add <file_name>` , you may also list specific files you'd like to push changes from with `git add <file_name> <file_name2>`, and if you would like to add ALL changes in all files, you can run `git add .`, this is my prefered method and I use it every time.
8. Now we can commit these staged changes with a message by running the following command:
`git commit -m"<insert_message_here>"` you may also use single quotes, `git commit -m'<insert_message_here>'`, just note that you must be consistent with the quotation syntax(format) you choose.
9. Now, you can write more code if you'd like and to add them, go back to step 6, then continue in order.  If you are finished coding and would like to push your commits to github, you may run the following command:
`git push origin -b <branch_name>`
10. Congratulations! You just successfully pushed code to github!
11. When you are ready to create merge your branch to the master branch you can head back to github

NOTE:
If you are cloning an existing repository, meaning you want to put a copy on your local machine, start at step 3. If you want to work on an existing project, you may skip to step 4 and begin. WITH BOTH ABOVE SCENARIOS DO NOT RUN THE FOLLOWING COMMANDS AGAIN:
`git init`
`git clone <github_url_to_repo>.git`