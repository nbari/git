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

Then pick/forward and push **force** your branch:

    git push -u origin -f my_branch

# Autosquash

After creating the branch your fist commit with this:

    git commit --fixup SHAofthecommit -a

Subsequent commits just git commit add etc and for finish:

    git rebase -i master --autosquash

Optional for .gitconfig
   [rebase]
     autoSquash = true
