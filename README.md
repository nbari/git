# git

Add second repo to push (multiple pushurl):

    git remote set-url --add --push origin git@host:project

# --orphan  Branch

    git checkout --orphan newbranch
    git rm -rf .
    <do work>
    git add your files
    git commit -m 'Initial commit'

# commit using GPG

    git commit -S -m your commit message

or add on .gitconfig

    [commit]
        gpgsign = true

Squash via rebase:

    git rebase -i origin/master

Then pick/forward

    git push -u origin -f my_branch
