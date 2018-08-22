GZOSP
========

To initialize your local repository, use this command:

	repo init -u https://github.com/GZOSP/manifest.git -b 9.0

Submitting Patches
------------------

We're open source, and patches are always welcome!
To do this, you will need an account setup with our gerrit server and a changeid hooks.
To add the changeid hook in a project, use the following commands:

	cd <project>
	scp -p -P 29418 <username>@review.gzospgzr.com:hooks/commit-msg ${gitdir}/hooks/

You can also install the hook globally in all local GZOSP projects

	repo forall -c 'gitdir=$(git rev-parse --git-dir); scp -p -P 29418 <username>@review.gzospgzr.com:hooks/commit-msg ${gitdir}/hooks/'

Go have a coffee while this runs

You can send patches by using these commands:

    cd <project>
    git add --all
    git commit
    git push ssh://<username>@review.gzospgzr.com:29418/GZOSP/<project> HEAD:refs/for/<branch>

This will commit your changes into a single commit.
Make sure your git has the changeid hooks added.
If you are going to make extra additions, just repeat steps, but instead of

	git commit

use

	git commit --amend

Gerrit will recognize it as a new patchset.

To view the status of your and others patches, visit [GZOSP Code Review](http://review.gzospgzr.com)
