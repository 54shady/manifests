# Repo Usage

## How to use this manifest

Init repo

	repo init --repo-url=https://mirrors.tuna.tsinghua.edu.cn/git/git-repo -u git@github.com:54shady/manifests -b master

sync all project code

	repo sync

sync only linuxc project

	repo sync linuxc

## checkout a local branch for modify code

1. for example, checkout local branch debug for linuxc project

	repo start debug linuxc

2.	modify the code and push to remote

	cd linuxc
	modify the code base
	git push

3. remove the debug branch

	repo abandon debug linuxc

## sync remote different branch

for example, there are two branch in remote manifest(master, and debug)

what if you sync the code base using master first like below

	repo init --repo-url=https://mirrors.tuna.tsinghua.edu.cn/git/git-repo -u git@github.com:54shady/manifests -b master

want to checkout the debug branch

	repo init -b debug
	repo sync

## sync local(git checkout)

what if you delete some files, and just want to checkout local file
like (git checkout)

	repo sync -l
