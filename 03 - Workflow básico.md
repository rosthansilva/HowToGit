# Workflow de Vencedor

No espirito do trabalho em grupo que trás o git, existe um workflow que vamo sempre repetir.
Agora esse workflow será explicado e com ele os passos

```
git clone <the SSH key for your repository>
# This fetches the GitHub repo to your local machine and starts the tracking process

# You will now make some changes to files inside the repo
# Once you're done, you wanna check what are the changes

git status # git status tell you what are the modified files, as well as new files you've created

git add <file_names> # git add adds the files you want to commit on the stage
# you don't have to add all the files that are changed onto the stage
# for example, you might actually have made a change in one of the files and you prefer the previous version, in that case you don't have to git add the change

# You would probably want to check the git status again to make sure you have added all the correct files
git status
# Now, you would be able to see all the tracked and untracked files. Check for any errors before committing

git commit -m "add meaningful commit message" # this will add a commit message and take a snapshot of your repository with the change you wish to document
# Once you've done that, you might want to check git status again

git status
# double and triple checking is always good, now your command prompt should tell you that there is no untracked files.

# This is all good for you, but if you want to collaborate with others and for others to also see the changes you've made, you'd want to push this commit to GitHub.
# Assuming that you've been working on the master branch, you will do the following
git push origin master # This pushes the changes in the master branch to the remote called origin, which should be your GitHub repo. Sometimes, you're branch is not master and your remote is not origin, you can use the format
# git push <remote_name> <branch_name>

# Now this will become a pull request ready to be merged into the main assuming that there are no conflicts
DEV Community – A constructive and inclusive social network for software developers. With you every step of your journey.

Built on Forem — the open source software t
````

Novo Arquivo
