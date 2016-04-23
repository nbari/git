# git

Add second repo to push (multiple pushurl):

    git remote set-url --add --push origin git@home:gitolite-admin

cat ``.git/config``:

	[remote "origin"]
        url = git@github.com:nbari/git.git
		fetch = +refs/heads/*:refs/remotes/origin/*
		pushurl = git@home:repo-name
