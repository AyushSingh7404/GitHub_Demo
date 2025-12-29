Github cheatsheet link: https://supersimple.dev/courses/git-github-course
In git commit == version

git init

git status

git add file_name

git add folder_name

git add .

git commit -m "Your Commit Message"

git config --global user.email "your_email"

git config --global user.name "your_name"

git log

git commit -m "Version 1" --amend     # To edit a previous commit adding file or correcting commit message

git reset file_name        # To remove things from the staged area (where files are after "git add" command)

git reset folder_name

git reset .

git checkout -- file_name       # To reset the changes in a file and literally remove all the changes

git checkout -- folder_name

git checkout -- .

git checkout commit_hash       # How to go back to any previous version and the git hash is the commit hash of the version where we want it to go which is like this 388cc9b338a1e668835f0a0d964877a4b849f1ea

git log --all   # it is used to show all the logs because if we go to any previous commit then git log will show all commit before that commit not the commits after it

HEAD shows which version are we at

press q to get out of git log

git log --all --graph   # to see branches

git checkout master    # it will switch us to the latest commit

git checkout f7ceecb3df11bc19a6d247f9237279f4af72a4cb file_name

git checkout f7ceecb3df11bc19a6d247f9237279f4af72a4cb folder_name

git checkout f7ceecb3df11bc19a6d247f9237279f4af72a4cb .

When we normally do git checkout and them if we make another commit on top of any previous commit then it used to to  keep making branches of those commit but when we do it like mentioned above then it will simply now it make commit above the last commit like above version 3 we have version 1 updated

# How to make any alias in git of your chossing
git config --global alias.s "status"  So now git s will works same as git status

git config --global alias.cm "commit"
git config --global alias.co "checkout"

# How to delete git completely from a project
rm -rf .git

git remote add origin https://github.com/AyushSingh7404/GitHub_Demo.git   # command to connect local repository to remote repository

git remote   # to check the repository that is connected
git remote -v   # verbose

git remote remove origin  # origin is the repository name and this command is to remove the remote repository connection

git config --global credential.username "your user name"

git push origin master

# Trouble shooting if push doesn't work
git remote add origin https://AyushSingh7404@github.com/AyushSingh7404/GitHub_Demo.git    # Add your username in the url

Or use personal access token and then give it when it asks for password

git push --force origin master   # This is a last resort use it if pull or fetch does not work your push is behind the commit on github but you don't care you need to push this version only (Keep in mind this command will delete all the commit ahead of yours commit)

To make the push command short use this command
git push origin master --set-upstream

The from after it use "git push" ans now github knows the origin and master

git push origin master -f   # will also overwrite the previous commit

git clone https://github.com/AyushSingh7404/GitHub_Demo.git new_github

git fetch

git pull origin master


