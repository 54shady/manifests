## How to use this manifest

Init repo

	repo init --repo-url=https://mirrors.tuna.tsinghua.edu.cn/git/git-repo -u git@github.com:54shady/manifests -b master

sync all project code

	repo sync

sync only linuxc project

	repo sync linuxc

checkout a local branch for modify code

1. for example, checkout local branch debug for linuxc project

	repo start debug linuxc

2.	modify the code and push to remote

	cd linuxc
	modify the code base
	git push

3. remove the debug branch

	repo abandon debug linuxc
