# git

Add second repo to push (multiple pushurl):

    git remote set-url --add --push origin git@host:project

# --orphan  Branch

    git checkout --orphan newbranch
    git rm -rf .
    <do work>
    git add your files
    git commit -m 'Initial commit'
